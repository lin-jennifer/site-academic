---
date: "2021-03-15T00:00:00Z"
draft: false
lastmod: "2021-03-15T00:00:00Z"
linktitle: R Workshop$:$ Pipes and `ggplot`
summary: R Workshop on pipes and `ggplot`
menu:
  Rggplot:
    name: Overview
    weight: 1
title: R Workshop$:$ Pipes and `ggplot`
toc: false
type: docs
weight: 1
---

## Overview

The goal of this workshop is to increase efficiency and comfort with common commands in packages from the tidyverse series, specifically dplyr and ggplot. The workshop will focus on familiarizing attendees with the basics of each package and the use of pipes to streamline code. This session will also briefly touch on time and spatial data to demonstrate how these basic commands can be applied to address more complex issues.

## Learning Goals

1. Increase coding proficiency with `tidyverse` packages, specifically `dplyr` and `ggplot`.
2. Develop skills necessary to communicate results clearly with data visualization tools
3. Apply your knowledge to answer your own research questions.

## Workshop Data

To complement this workshop, I prepared a cleaned version of the 2018 Cooperative Elections Studies (formerly the Cooperative Congressional Elections Studies) dataset. The data can be accessed from my website or by cloning the workshop GitHub repository. We will largely focus on select variables in each of the sections below but here is a guide to all the variables that I included in the file along with a brief description.

|Variable|Description|
|:-------|:----------|
|`starttime`|Start Time|
|`endtime`|End Time|
|`caseid`|Respondent ID|
|`region`|Region in country|
|`county`|County Name|
|`countyfips`|County FIPS Code|
|`state`|State Abbreviations|
|`inputstate`|State FIPS Code|
|`gender`|Respondent Gender|
|`birthyr`|Year of Birth|
|`votereg`|Registered to vote?|
|`pid3`|Party ID 3 categories|
|`amtDonate`|Amount donated to politics|
|`appTrump`|Approval of Trump|
|`appCongress`|Approval of Congress|
|`appSupremeCourt`|Approval of Supreme Court|
|`vote16`|Vote Choice in 2016|
|`ideo3`|Ideology 3 category|
|`Age`|Respondent Age|

You may access the data and all the course materials in the section below.

# Course Materials

- Course Handout ([PDF](./Plpes_ggplot_Rhandout.pdf))
- GitHub (https://github.com/lin-jennifer/ggplot-workshop)
- Slides ([PDF](./Presentation.pdf))
- Data ([CSV](CCES18_subset.csv))
