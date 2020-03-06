---
layout: default
title: Helpful Links
---

* **Make a map that will take csv files:** [Github](https://github.com/CloudCannon/bakery-store-jekyll-template/blob/data-files/contact.html) or [video tutorial](https://learn.cloudcannon.com/jekyll/introduction-to-data-files/?h=jekyll%20open%20data) that doesn't really apply but might help somehow
* **The jekyll maps plugin we looked at today:** [Github](https://github.com/ayastreb/jekyll-maps) or [website](https://ayastreb.me/jekyll-maps/)
* **Data files (from Jekyll docs):** <https://jekyllrb.com/docs/datafiles/>
* **[Deploying with GitHub pages vs. Netlify](https://www.netlify.com/github-pages-vs-netlify/)**
* **[Liquid filters for Jekyll](https://jekyllrb.com/docs/liquid/filters/)**

**Below goes to show one can do tables using data from \_data files using markdown as well:**


| Alma mater |  PR articles  | Total |
|-------|-------|------|
| University of Alberta |  {% for libs in site.data.librarians %}{% if libs.MLS_Inst == "University of Alberta" and libs.PR_Journal >=1 %}+{{ libs.PR_Journal }}{% endif %}{% endfor %} |  |
| McGill University |{% for libs in site.data.librarians %}{% if libs.MLS_Inst == "McGill University" and libs.PR_Journal >=1 %}+{{ libs.PR_Journal }}{% endif %}{% endfor %}   |   |
