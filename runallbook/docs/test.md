---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(launch:thebe)=
# test

```{code-cell} ipython3
var1="hello world!"
```

```{python tags=c("hide-input")}
print(var1)
```
```{code-cell} ipython3
:tags: ["full-width"]
print("This is a test.")
```

```{code-cell} ipython3
:tags: ["hide-input"]
print(var1)
```

```{code-cell} ipython3
:tags: ["remove-input"]
print(f"This is a test. {var1}")
```
```{code-cell} ipython3
:tags: ["margin"]
print("Margin code")
```

```{code-cell} ipython3
:tags: ["output_scroll"]
for ii in range(100):
  print("This is a test.")
```
