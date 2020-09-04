---
title: Library of Political Texts (poltextr)
author: ''
date: '2020-07-05'
slug: poltextr
categories:
  - Code
  - Documentation
tags:
  - R
subtitle: 'Currently Under Construction'
summary: 'A Library of Assorted Political Texts that can be easily accessed in R'
authors: []
lastmod: '2020-07-05T15:45:40-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

<IMG src="/package/poltextr.png" align=right border=20px HSPACE=”50” VSPACE=”50”>

To easily access any textual data that I use in my research in R, I created an R package that stores the corpuses.

## Installation

```r
library(devtools)
install_github("lin-jennifer/poltextr")
library(poltextr)
```

## Access Data

To see which datasets are available in the package, run the following:

```r
data(package="poltextr")
```

In this package, metadata files contain details about the speakers and they are labelled with `_meta` at the end of the data name.

To load a corpus, run

```r
data(dnc16) # Loads DNC speeches from 2016
```

Metadata files are loaded in as `.csv` files and can be called as a data frame by running

```r
data(dnc16_meta) # Loads DNC metadata from 2016
```

# Library Contents

## National Convention Speeches

### Years Included (and Parties)
- 2020 (Democrat and Republican)
- 2016 (Democrat and Republican)

## Political Party Platforms

*Feature is Still in the Works*

### Categories

- Democrat Party Platform
- Republican Party Platform

## Presidential Debates

*Feature is Still in the Works*

### Election Years
- 2016