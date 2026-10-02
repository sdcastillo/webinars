RStudio webinars
================

This repository contains materials that have been used in RStudio webinars. It is a numbered set of folders, one webinar each, forked from [rstudio/webinars](https://github.com/rstudio/webinars). Recordings and the original series listing stay on the [RStudio webinars page](https://www.rstudio.com/resources/webinars/).

You can clone this repository with git, or download the entire content as a zip file from the GitHub page.

A folder is the presenter’s project, not an installable package. Most sessions put a slide deck next to the scripts. Decks are PDF or HTML. Code is `.R`, R Markdown (`.Rmd`), or a small Shiny app (`app.R`, or `ui.R` with `server.R`). When a folder includes a README, that file is the note for how the demo was meant to be started. The tidyverse session is opened by running `Tidyverse-webinar/Tidyverse-webinar.Rmd` with Run Document; solution code sits behind a button in the notebook. The Shiny introduction keeps the demo apps under `apps/` and the slides in `intro-to-shiny.PDF`.

The sequence follows the RStudio stack as it was taught. It starts with the grammar of data: `dplyr`, `tidyr`, and `ggvis`, including an interactive document with linked brushing. Reporting runs from knitr and R Markdown through R Notebooks, flexdashboard, bookdown, and blogdown. Shiny is the longest thread: three “how to start” sessions (a template, inputs and outputs, `reactive`, `isolate`, `observeEvent`, `eventReactive`, and `reactiveValues`), then modules, gadgets, bookmarking, click and brush events, linked zooming, shinydashboard, and shinytest. Data access is its own track: multi-format import (CSV, Excel, JSON, SPSS, Stata, SQLite, and a Spark sample), `readxl`, web APIs with `httr`, scraping, and RStudio professional ODBC drivers for SQL Server, Oracle, PostgreSQL, Redshift, Hive, Impala, Salesforce, and Teradata.

Several demos are tied to the environment of the day and will not rerun unchanged. The sparklyr taxi notebook analyzes on the order of a billion NYC taxi records and expects a Spark cluster with data already in Hive; the local notebooks only need a local Spark connection. The activity dashboard was shipped without a public API key. packrat, RcppParallel, and covr materials target the package versions current when the webinar was given, mostly between 2014 and 2017. Read the README or the setup script in that folder before installing anything. `23-Importing-Data-into-R/setup/00-required-packages.R` is one place the dependency list is written down. Two folders share the number 30 (`30-Web-APIs` and `30-sparklyr-rmarkdown`); use the name, not the number, when you open a session.

To use the archive, open a folder as an RStudio project when an `.Rproj` is present. Run the `.R` file, or Knit / Run Document on the `.Rmd` the slides refer to. Shiny apps start with `shiny::runApp()` on the app directory. The slides are the PDF or HTML file sitting in the same folder.

* **Slides.** PDF or HTML deck for that session.
* **Scripts.** `.R` files the presenter ran live.
* **Notebooks.** `.Rmd` opened with Run Document or Knit.
* **Apps.** Shiny `app.R`, or `ui.R` with `server.R`.
* **Notes.** A README, Q&A, or setup script when the demo needed one.

Tracks, in series order:

* **Grammar and reporting.** Folders 01–02, 12–13, 22, 24–25, 37–39, 41, 46. dplyr, tidyr, ggvis, knitr, R Markdown, notebooks, flexdashboard, bookdown, blogdown, recipes, and the tidyverse.
* **Shiny.** Folders 03, 07–10, 16, 19, 29, 33, 47–48. Interactive documents, dashboards, modules, gadgets, bookmarking, graphics, and shinytest.
* **Getting data in.** Folders 11, 23, 30–32, 36, 40, 50–51. Import, readxl, web APIs, scraping, a hotel-site case study, and database drivers.
* **sparklyr.** Folders 14, 30-sparklyr-rmarkdown, 42–45. Local connections and the cluster notebooks.
* **IDE and servers.** Folders 04, 06, 15, 17–18, 20–21, 26–28, 34–35. Projects, git, packrat, addins, profiling, covr, RcppParallel, RStudio Server Pro, Shiny Server Pro, and Connect.
