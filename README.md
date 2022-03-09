# ADF to Markdown converter

Building off the work from [`md-to-adf`](https://github.com/b-yond-infinite-network/md-to-adf), this module does the opposite, taking an object in Atlassian Document Format, and outputting Markdown.

## ⚠️⚠️ BEWARE ⚠️⚠️

ADF is a superset of Markdown. It contains more functionality than Markdown can capture. Any unsupported elements (e.g. mentions, panels, etc.) will simply be discarded.

## Usage

``` javascript
const adf2md = require('adf-to-md');

// const adfObject = ...
const markdown = adf2md(adfObject);
```