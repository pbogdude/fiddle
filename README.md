# bin or fiddle?

This repository demonstrates how to reconfigure one of 
[Mike Bostock's blocks](https://bl.ocks.org/mbostock/4062045) so that it opens in JSFiddle.neg and JSBin.com

# bin

Click on <http://jsbin.com>, then replace the default HTML contents by copying and pasting the contents of ```bin.html``` from this repo.

Note: ````bin.html```` loads the data directly from [Mike Bostock's block](https://bl.ocks.org/mbostock/4062045). Otherwise, there's no difference between ````bin.html```` and Mike's ````index.html````.

For instructions on loading a gist into JSBin, see: <https://jsbin.com/help/import-gists>

For instructions on sharing your bin, see: <https://jsbin.com/help/share-latest-bin>

# fiddle

To collaborate on the same fiddle, click this link:

http://jsfiddle.net/gh/get/library/pure/umbcvis/fiddle/tree/master/#&togetherjs=ssUKvErAf6

To simply open this repo in JSFIddle, click:

<http://jsfiddle.net/gh/get/library/pure/umbcvis/fiddle/tree/master/>

The files used by JSFiddle:

* demo.html (html without boilerplate tags: doctype, html, meta, etc.)
* demo.css (CSS only)
* demo.js (JavaScript only)
* demo.details (for configuring remote resources, such as d3.v4.min.js)
* miserables.json (served from the master branch)

This demo applies <a href="http://doc.jsfiddle.net/use/github_read.html" target="_blank">JSfiddle guidelines</a> to [Mike Bostock's force-directed graph visualization](https://bl.ocks.org/mbostock/4064025).  Several important modifications show up in ```demo.js```:

* window.onload -- the callback contains all the code from the block
* svg -- the ```viewBox``` attribute and CSS ```width: 100%``` allow it to fit in the JSFiddle frame
* miserables.json -- served from this github project's website

#### github project site

The same files open with index.html (not used by JSFiddle) at the github project site:

<https://umbcvis.github.io/fiddle/>

See the [Github documentation](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/)
for guidance on configuring gh-pages to serve files from the master branch.
