---
title: "NCF (Mark)Down"
author: Jennifer Lin
date: '2020-04-30'
slug: ncfdown
categories: ["Code"]
tags: ["R", "R Markdown"]
subtitle: ''
summary: 'R Markdown template using New College of Florida inspired colors'
authors: []
lastmod: '2020-04-30'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
links:
- name: GitHub
  url: https://github.com/lin-jennifer/ncfdown
  icon_pack: fab
  icon: github
- name: Demo
  url: https://lin-jennifer.github.io/ncfdown/
---

*This template was made based off the style created by [Yan Holtz](https://github.com/holtzy) in the [epuRate](https://github.com/holtzy/epuRate) template. Thank you for your inspiration and assistance in creating this template*

## Demo

See it in action here: https://lin-jennifer.github.io/ncfdown/

## Using this Template

Install this template using `devtools`

```
library(devtools)
install_github("lin-jennifer/ncfdown")
library(ncfdown)
```

By downloading the package, the source for the template can be accessed by using `File` &rarr; `New File` &rarr; `R Markdown` &rarr; `From Template`

## Package Options

For this package, there are several options under the `output:` category on the `YAML`:

1. `ncf`: This option provides a basic structure for HTML documents knitted out of an R Markdown document. Simply note `ncfdown::ncf` under the output option to activate this template. 
2. `ncfweb`: Consult the [R Studio Handbook](https://bookdown.org/yihui/rmarkdown/rmarkdown-site.html) for how to create a website. This option provides a design for an R Markdown based website. It differs from the `ncf` option in three ways:
    1. Author and Date in footer only rather than under the title
    2. Removes code folding option and code folding button on the upper-right-hand corner on each page
    3. Removes GitHub triangle in upper right-hand corner

To switch between the two versions of this package, simply edit the `YAML` such that the one under `ncf`:

```
output:
  ncfdown::ncf:
    toc: TRUE
    number_sections: FALSE
    code_folding: "hide"
```

would become this under `ncfweb`:

```
output:
  ncfdown::ncfweb:
    toc: TRUE
    number_sections: FALSE
```

## Contributing to this Package

To help me improve this package, please reach out using the following methods:

1. Email: [jenniferlin2025@u.northwestern.edu](mailto:jenniferlin2025@u.northwestern.edu)
2. Send a message via the [Contact](https://lin-jennifer.github.io/#contact) tab
3. Open a pull request on the project GitHub: https://github.com/lin-jennifer/ncfdown
