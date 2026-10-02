---
layout: default
title: RStudio Webinars
description: Code, slides, and notebooks from the RStudio webinar archive.
samwiki: true
---

<section class="sw-lede" aria-labelledby="archive-title">
  <div class="sw-lede-copy">
    <h2 id="archive-title">Code and slides from the webinars</h2>
    <p>This repository is the working archive for RStudio webinars: the slides, and the code that was run in the session. It is a numbered set of folders, one webinar each, forked from <a href="https://github.com/rstudio/webinars">rstudio/webinars</a>. Recordings and the original series listing stay on the <a href="https://www.rstudio.com/resources/webinars/">RStudio webinars page</a>. What lives here is the part you can open in the RStudio IDE.</p>
    <p>A folder is the presenter’s project, not an installable package. Most sessions put a slide deck next to the scripts. Decks are PDF or HTML. Code is <code>.R</code>, R Markdown (<code>.Rmd</code>), or a small Shiny app (<code>app.R</code>, or <code>ui.R</code> with <code>server.R</code>). When a folder includes a README, that file is the note for how the demo was meant to be started. The tidyverse session is opened by running <code>Tidyverse-webinar/Tidyverse-webinar.Rmd</code> with Run Document; solution code sits behind a button in the notebook. The Shiny introduction keeps the demo apps under <code>apps/</code> and the slides in <code>intro-to-shiny.PDF</code>.</p>
    <p>The sequence follows the RStudio stack as it was taught. It starts with the grammar of data: <code>dplyr</code>, <code>tidyr</code>, and <code>ggvis</code>, including an interactive document with linked brushing. Reporting runs from knitr and R Markdown through R Notebooks, flexdashboard, bookdown, and blogdown. Shiny is the longest thread: three “how to start” sessions (a template, inputs and outputs, <code>reactive</code>, <code>isolate</code>, <code>observeEvent</code>, <code>eventReactive</code>, and <code>reactiveValues</code>), then modules, gadgets, bookmarking, click and brush events, linked zooming, shinydashboard, and shinytest. Data access is its own track: multi-format import (CSV, Excel, JSON, SPSS, Stata, SQLite, and a Spark sample), <code>readxl</code>, web APIs with <code>httr</code>, scraping, and RStudio professional ODBC drivers for SQL Server, Oracle, PostgreSQL, Redshift, Hive, Impala, Salesforce, and Teradata.</p>
    <p>Several demos are tied to the environment of the day and will not rerun unchanged. The sparklyr taxi notebook analyzes on the order of a billion NYC taxi records and expects a Spark cluster with data already in Hive; the local notebooks only need a local Spark connection. The activity dashboard was shipped without a public API key. packrat, RcppParallel, and covr materials target the package versions current when the webinar was given, mostly between 2014 and 2017. Read the README or the setup script in that folder before installing anything. <code>23-Importing-Data-into-R/setup/00-required-packages.R</code> is one place the dependency list is written down. Two folders share the number 30 (<code>30-Web-APIs</code> and <code>30-sparklyr-rmarkdown</code>); use the name, not the number, when you open a session.</p>
    <p>To use the archive, clone it or download the ZIP from GitHub and open a folder as an RStudio project when an <code>.Rproj</code> is present. Run the <code>.R</code> file, or Knit / Run Document on the <code>.Rmd</code> the slides refer to. Shiny apps start with <code>shiny::runApp()</code> on the app directory. The slides are the PDF or HTML file sitting in the same folder. This page is the index. The files stay in the <a href="https://github.com/sdcastillo/webinars">repository</a>.</p>
  </div>
  <aside class="sw-find" aria-labelledby="folder-title">
    <h2 id="folder-title">In each folder</h2>
    <ul>
      <li><strong>Slides</strong> PDF or HTML deck for that session.</li>
      <li><strong>Scripts</strong> <code>.R</code> files the presenter ran live.</li>
      <li><strong>Notebooks</strong> <code>.Rmd</code> opened with Run Document or Knit.</li>
      <li><strong>Apps</strong> Shiny <code>app.R</code>, or <code>ui.R</code> with <code>server.R</code>.</li>
      <li><strong>Notes</strong> A README, Q&amp;A, or setup script when the demo needed one.</li>
    </ul>
  </aside>
</section>

<section class="sw-section" id="tracks" aria-labelledby="tracks-title">
  <div class="sw-section-head">
    <h2 id="tracks-title">Where to start <span class="sw-pill">5 tracks</span></h2>
    <p>Folders are numbered in series order. These five groups are the ones the archive keeps returning to. Each card opens a representative session on GitHub; the rest of that track is in the sibling folders.</p>
  </div>
  <div class="sw-grid">
    <article class="sw-card">
      <div class="sw-card-top">
        <h3 class="sw-name"><a href="https://github.com/sdcastillo/webinars/tree/master/01-Grammar-and-Graphics-of-Data-Science">Grammar and reporting</a></h3>
        <span class="sw-lang">dplyr · rmarkdown</span>
      </div>
      <p class="sw-desc">dplyr, tidyr, and ggvis, then knitr, R Markdown, notebooks, flexdashboard, bookdown, blogdown, and the tidyverse visualization session.</p>
      <p class="sw-meta">Folders 01–02, 12–13, 22, 24–25, 37–39, 41, 46</p>
      <div class="sw-actions">
        <a class="sw-btn sw-btn-source" href="https://github.com/sdcastillo/webinars/tree/master/01-Grammar-and-Graphics-of-Data-Science">Source</a>
      </div>
    </article>
    <article class="sw-card">
      <div class="sw-card-top">
        <h3 class="sw-name"><a href="https://github.com/sdcastillo/webinars/tree/master/08-How-to-start-with-Shiny-Part-1">Shiny</a></h3>
        <span class="sw-lang">shiny</span>
      </div>
      <p class="sw-desc">Three “how to start” sessions, then modules, gadgets, bookmarking, interactive graphics, shinydashboard, and shinytest.</p>
      <p class="sw-meta">Folders 03, 07–10, 16, 19, 29, 33, 47–48</p>
      <div class="sw-actions">
        <a class="sw-btn sw-btn-source" href="https://github.com/sdcastillo/webinars/tree/master/08-How-to-start-with-Shiny-Part-1">Source</a>
      </div>
    </article>
    <article class="sw-card">
      <div class="sw-card-top">
        <h3 class="sw-name"><a href="https://github.com/sdcastillo/webinars/tree/master/23-Importing-Data-into-R">Getting data in</a></h3>
        <span class="sw-lang">import · httr</span>
      </div>
      <p class="sw-desc">CSV, Excel, JSON, SPSS, Stata, and SQLite; readxl; web APIs; scraping; a hotel-site case study; and professional ODBC drivers.</p>
      <p class="sw-meta">Folders 11, 23, 30–32, 36, 40, 50–51</p>
      <div class="sw-actions">
        <a class="sw-btn sw-btn-source" href="https://github.com/sdcastillo/webinars/tree/master/23-Importing-Data-into-R">Source</a>
      </div>
    </article>
    <article class="sw-card">
      <div class="sw-card-top">
        <h3 class="sw-name"><a href="https://github.com/sdcastillo/webinars/tree/master/30-sparklyr-rmarkdown">sparklyr</a></h3>
        <span class="sw-lang">spark</span>
      </div>
      <p class="sw-desc">Local Spark connections, dplyr verbs on Spark, and the cluster notebooks for extension, advanced features, and deployment modes.</p>
      <p class="sw-meta">Folders 14, 30-sparklyr-rmarkdown, 42–45</p>
      <div class="sw-actions">
        <a class="sw-btn sw-btn-source" href="https://github.com/sdcastillo/webinars/tree/master/30-sparklyr-rmarkdown">Source</a>
      </div>
    </article>
    <article class="sw-card">
      <div class="sw-card-top">
        <h3 class="sw-name"><a href="https://github.com/sdcastillo/webinars/tree/master/15-RStudio-essentials">IDE and servers</a></h3>
        <span class="sw-lang">rstudio</span>
      </div>
      <p class="sw-desc">Projects, git, debugging, packages, packrat, addins, profiling, covr, RcppParallel, RStudio Server Pro, Shiny Server Pro, and Connect.</p>
      <p class="sw-meta">Folders 04, 06, 15, 17–18, 20–21, 26–28, 34–35</p>
      <div class="sw-actions">
        <a class="sw-btn sw-btn-source" href="https://github.com/sdcastillo/webinars/tree/master/15-RStudio-essentials">Source</a>
      </div>
    </article>
  </div>
</section>

<section class="sw-section" id="run" aria-labelledby="run-title">
  <div class="sw-section-head">
    <h2 id="run-title">Run a session</h2>
    <p>Clone the repository, or use Download ZIP on the GitHub page. Then open one numbered folder.</p>
  </div>
  <ul>
    <li>If the folder contains an <code>.Rproj</code>, open that project in RStudio so the working directory matches the demo.</li>
    <li>Install only the packages that session names. Early ggvis notes need the development version from the date of the webinar; later folders pin a tighter set in a setup script or README.</li>
    <li>For a script, source or step through the <code>.R</code> file. For a notebook, open the <code>.Rmd</code> and use Run Document or Knit. For Shiny, call <code>shiny::runApp()</code> on the app directory (<code>runApp("activity-dashboard/")</code> in the shinydashboard session).</li>
    <li>Read the PDF or HTML slides beside the code. A few sessions point at slides hosted elsewhere (bookdown, blogdown, packrat); the folder README has that URL.</li>
    <li>Treat cluster, database, and API demos as records of the live session. sparklyr’s Hive example, the ODBC driver scripts, and the activity dashboard need infrastructure this repository does not include.</li>
  </ul>
</section>
