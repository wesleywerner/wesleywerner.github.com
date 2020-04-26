# Materialize Projects Page

This Jekyll site is a custom build using [materializecss.com](https://materializecss.com).

The ideology behind the structure of this site pivots around the origin of blogging before it was called that: Web logs, and before that: Development logs.

Developers like us keep a journal of progress made on our projects, things learned, design notes, future warnings to oneself about caveats, and so on.

The main premise are Project Pages, each which may have changelogs associated, development notes or devlogs attached.

## Links

Listing of resources relating to the technologies used to generate this site:

* [Jekyll-Bootstrap][]
* [Jekyll Docs][]

## Quick Start

* [Install Ruby and Jekyll][Jekyll Installation]
* Exec `jekyll serve`, the localhost URL will be printed to stdout.

```
$ jekyll serve
Configuration file: ./_config.yml
            Source: .
       Destination: ./_site
      Generating... done in 0.551 seconds.
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```

If you are running jekyll in WSL and experience lock-ups, try running with the `--force_polling` flag.

## CSS

There are light and a dark stylesheets, choose the one you want with the `options.style` setting.

You can customize the colors in `assets/css/light.scss` and `assets/css/dark.scss` respectively.

## Search

Duckduckgo search is integrated, to generate your search url go to https://duckduckgo.com/search_box and copy the `src` url that is generated into the `options.search.url` in `_config.yml`.

### Directory Structure

```
.
├── assets
│   └─────────> Css themes and materialize JavaScript
├── _includes
│   └─────────> Jekyll templates
├── _layouts
│   └─────────> Page layouts
├── _posts
│   └─────────> Changelogs live here
├── projects
│   └─────────> Your projects live here
├── _sass
│   └─────────> Materialize sass sources
└── _site
    └─────────> Your built site
```

### Options

These options are available in the `_config.yml` file:

* `options.changelog_heading_text`: The heading text for your devlogs/changelogs on the project page.
* `options.links`: List of links displayed in the footer.
* `'options.copyright_text`: Copyright text in the footer.

### Navigation Pages

To include any page in the main navigation links, add the `group: navigation` front matter. `about.markdown` uses this for example.

### Projects

To create a new project:

* mkdir projects/fizzbuzz
* touch projects/fizzbuzz/index.md

Add this front matter:

```
---
layout: project
title: "FizzBuzz"
description: "Prints fizz, buzz or fizzbuzz."
thumb: /projects/fizzbuzz/thumb.png
links: ["title 1", "https://example.com", "title 2", "https://example.com]
status: prototype
---
```

### Status Badges

Projects can display a development status badge, this is done with the `status` front-matter. You can make up any status you like, some statuses show up with particular color and tooltip text. You can define these in `_config.yml` under the `options.status_badges` list.

The projects on the index page are grouped and sorted by their badges, thus reorder the `status_badges` list to suit your needs.

## Journals and Changelogs

Projects can link to multiple changelogs, this is done by creating a new post using the `changelog` layout and setting the `project` front matter to the name of the project it relates to.

```
touch _posts/2000-01-02-journal-entry.md
```

With the front matter:

```
---
layout: changelog
title: "milestone 3 changes"
description: ""
project: FizzBuzz
---
```
