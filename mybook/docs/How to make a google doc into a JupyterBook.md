# How to make a google doc into a JupyterBook



1. Install necessary software
    * <span style="text-decoration:underline;">Docs to Markdown</span> Google Add-on
    * `pip install -U jupyter-book`
2. Make sure your google doc is organized
    * H1 headings will become separate pages for the JupyterBook
    * Example structure (pages will be Home, 1. Install DeepProfiler, etc.):
![alt_text](images/image1.png "image_tooltip")

    * How to indicate code? Courier new or monospaced fonts
    * How to indicate notes? (also warning, tip, important) - check out example pages
3. Convert the Google doc to markdown
    * Go to Add-ons > Docs to Markdown > Convert
    * Check the boxes for **Suppress info comment** and **Use reckless mode**
    * Hit the blue “Markdown” button
4. Paste into Atom and save as markdown file (.md)
    * Get rid of any warnings at the top of the page
5. Run my script to generate JupyterBook files


```
md2Book(filepath, delim="\n# ", bookName="mybook", numbered=False, savePath="same", makeTOC=True, Landing=1)

```



6. **Download and fix image refs**
    * Download images from Google doc File > Download > Web page
    * Images will have names where the number doesn’t correspond to order. Change the image files to be correct
    * Images should be located in **docs/images/** and should have names like “image1.png”
7. Add a config file
    * Should be added in /mybook folder
    * Here’s a good example: [Configuration reference](https://jupyterbook.org/customize/config.html)
8. Build the book
    * In terminal, navigate to folder containing mybook/


```
jupyter-book build --all mybook/
```


