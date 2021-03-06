[toc]

### TODO
 * FAQ
 * ~~docs/requirements~~
 * Manual 
   * Existing manual pages have been ported
	* Needs to be proof read & checked against Fs version 1 
   * Administration & Contributions need to be created
 * ~~Real world users list~~ Currently only public facing Flyspray installs - no way to check the others
 * Team
 * Link & header colors
 * ~~The manual pagination styling~~
   * ~~Fix links - long names overflow~~
 * Where to store the stable download?
 * make the /news (news.html) page
 * Write the current news posts

### Running localy
See [Github Pages](https://help.github.com/articles/using-jekyll-with-pages#installing-jekyll)
[Github Pages Guide](https://pages.github.com/)

### Manual Pages

All manual pages are store in the `_manual` folder.
Files are named `name_here.md`.
Manual pages url: `/manual/page-name`

Each page must contain the following at the top of the page:

 * manual - The section of the manual this document belongs to. 
 * Valid options for manual:
  * `start` - Getting Started 
  * `proj`  - Projects 
  * `user`  - User Management 
  * `tasks` - Tasks 
  * `admin` - Administration 
  * `cont`  - Contributions
 * order - The order this page should appear in the manual index. Sorted low to high.

```
---
layout: manual
title: Your title here
manual: tasks
order: 50
---

Content goes here
```

#### Translating the manual

### News

News items go into the `_posts` folder.
Files are names `2014-8-25-title.md` replace the year-month-day with news item date.

Each news item must contain the following at the top of the page:
 * Update the date variable
 * The summary is used on the home page
 
```
---
layout: news
title: News title here
category: news
date: 2014-08-25 20:00:00
summary: "Summary for the home page"
---

News goes here
```
### Other Pages
There are three types of pages each type lives in its own folder:
 * `docs`: Live in the `_docs` folder. Url: /docs
 * `community`: Live in the `_community` folder Url: /community
 * `devel`: Live in the `_devel` folder. Url: /devel

Each page must contain the following at the top:
 * order - (Optional) The order this page should appear in the sidebar. Sorted low to high. If this variable is not set the page will not be listed in the sidebar.
 
```
---
layout: page
title: Title here
order: 10
---

Content here
```


- - -



Using a modified version of [jekyll docs template](http://bruth.github.io/jekyll-docs-template)