---
layout: post
title: "rmarkdown test"
category: posts
---

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<style>
.dcl__index-module__console--2YAI1, .dcl__index-module__editor--m_p4P {font-size: 15px !important; }
.lm_header .lm_tab .lm_title {font-size: 15px !important;}
.dcl__Button-module__extra-small--2toEt, .dcl__Button-module__small--1VJc5 {font-size: 15px;}
</style>
</head>
        <body>
        	<script type="text/javascript" src="//cdn.datacamp.com/dcl-react.js.gz"></script>
          <script type="text/javascript" src="https://cdn.datacamp.com/datacamp-light-latest.min.js"></script>
			<div data-datacamp-exercise data-lang="r">
        	<code data-type="sample-code">
          ## Cleaning

          For the remainder of the report, we will look only at data from the year 1995. We aggregate our data by location, using the *R* code below.

          ```{r}
          library(nasaweather)
          library(dplyr)

          year <- 1995

          means <- atmos %>%
            filter(year == year) %>%
            group_by(long, lat) %>%
            summarize(temp = mean(temp, na.rm = TRUE),
                   pressure = mean(pressure, na.rm = TRUE),
                   ozone = mean(ozone, na.rm = TRUE),
                   cloudlow = mean(cloudlow, na.rm = TRUE),
                   cloudmid = mean(cloudmid, na.rm = TRUE),
                   cloudhigh = mean(cloudhigh, na.rm = TRUE)) %>%
            ungroup()
          ```

</code>
</div>
</body>
</html>
