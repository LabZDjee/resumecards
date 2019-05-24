# My 9-card Résumé

This project for a quick *résumé* (I was in a rush to get one), forked from '[resume cards](http://ellekasai.github.io/resumecards)' by [Elle Kasai](http://ellekasai.com) ![](https://avatars0.githubusercontent.com/u/2410692?v=2&s=60)

There you can go in all details how to install and design this [Jekyll](https://jekyllrb.com), [Liquid](https://shopify.github.io/liquid) static pages stored as [GitHub Pages](https://pages.github.com)...

Many thanks and credit to *Elle* for this design I dared to derive and adapt to my likes :slightly_smiling_face:

## List of Changes Made from *Elle*'s Project

- `_includes/nav.html`: my contacts
- `_includes/scripts.html`: removed *twitter* script
- `_data/resume.yml`: identity, presentation header, avatar, and color scheme
- `index.html`: see section below
- `stylesheets/resumecards.scss`: `@media print`... `@page size` **A4**, some edits in `.modal-body` to have a more distinctive `<a>` display, menu as flex, redefined font, card height, padding, particularly in `@media print`
- stored a lot of temporary stuff in `/_work` folder and added this folder as an exclude in `_config.yml` and `.gitignore`
- changed fonts to simply: `Arial, Helvetica, sans-serif`

### Modifications in `index.html`

- removed `site.data.resume.demo` sections (and associated flag in `_data/resume.yml`)
- added link `<rel='shortcut icon' type='image/x-icon' href='{{ "/favicon.ico" | prepend: site.baseurl }}'>` in `<head>` after `favicon.ico` created and stored along `index.html`
- added a `title` to image and consequently a `photoTitle` in `/_data/resume.yml`
- added a `phoneticName` in  `/_data/resume.yml` to be displayed near name
- heavily reworked the navigation section (added a colophon as a markdown include for credits and stuff)
- added `pdfLocalUrl` in `/_data/resume.yml` to give location of stored résumé in pdf in the project and have a button in navigation section
- merged `subheading` and `duration` on a single line

## Installation / Tests Quickstarter

### Prerequisites

`ruby`, `rubygems`, `bundler`

### Installation

`bundle install`

### Run Tests

`bundle exec jekyll serve --watch`

### Deploy in GitHub Pages

As branch `gh-branch` (as can be seen in [settings](https://github.com/LabZDjee/resumecards/settings) / Github Pages Source)

URL: https://labzdjee.github.io/resumecards





