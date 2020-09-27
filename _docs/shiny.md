---
permalink: /docs/shiny/
layout: single
title: "Shiny Projects"
---

[Shiny](https://shiny.rstudio.com/) is an R package for building interactive web applications, it's a good approach for dynamic data visualization, especially applying 
for daily updated data. As a big fan of shiny, developing my own shiny is not a big ideal right now. However, there are lots of tricks that must be known for shiny developers like me.

Here I list bunch of shiny apps, some of them are developed by myself, some are cooperated with our team. (Code review on [Github](https://github.com/sisi-huang).) Have a look at a shiny app, please click on the corresponding image.


* Asian Restaurants in Berlin

It's my first self-developed shiny, to record asian restaurants I've visited in Berlin. 
The structure of shiny is `ui.R` and `server.R`, understanding functions from R package 
[`leaflet`](https://rstudio.github.io/leaflet/) is the main core of this shiny app.

[![Asian Restaurants in Berlin](/assets/images/sc-1.png)](https://sisihuang.shinyapps.io/interactivemap/)


* CausalQueries Demo

CausalQueries Demo is a Shiny app for making, updating and querying binary causal models, which is to promote understanding of R package [`CausalQueries`](https://github.com/macartan/CausalQueries). This shiny app bases on the typical shiny structure, which are contained in multiple scripts called `ui.R`, `server.R` and `ui_helper.R`.

[![CausalQueries Demo](/assets/images/sc-2.png)](https://eos.wzb.eu/ipi/CausalQueries/)

* DDWizard

DDWizard as the most complex shiny app I've scripted, which is a cooperated project. 
I really appreciated all contributions and efforts from [DeclareDesign](https://declaredesign.org/about/) team. DDWizard is a web interface that lets you select any design from a growing library of templates, the [DesignLibrary](https://cran.r-project.org/web/packages/DesignLibrary/DesignLibrary.pdf), customize them, and interrogate them. All without ever having to write any R code.

[![DDWizard](/assets/images/sc-3.png)](https://eos.wzb.eu/ipi/DDWizard/)

* Covid-19 Shiny (will be released soon!)



