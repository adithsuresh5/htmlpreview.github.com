GitHub & BitBucket HTML Preview
-------------------------------

Many GitHub repositories don't use GitHub Pages to host their HTML files. **GitHub & BitBucket HTML Preview** allows you to render those files without cloning or downloading whole repositories. It is a client-side solution using a CORS proxy to fetch assets.

If you try to open raw version of any HTML, CSS or JS file in a web browser directly from GitHub, all you will see is a source code. GitHub forces them to use the "text/plain" content-type, so they cannot be interpreted. This script overrides it by using a CORS proxy.

## Usage

In order to use it, just prepend this fragment to the URL of any HTML file: **[https://adithsuresh5.github.io/htmlpreview/?](https://adithsuresh5.github.io/htmlpreview/?)** e.g.:

 - https://adithsuresh5.github.io/htmlpreview/?https://github.com/twbs/bootstrap/gh-pages/2.3.2/index.html
 - https://adithsuresh5.github.io/htmlpreview/?https://github.com/documentcloud/backbone/blob/master/examples/todos/index.html

What it does is: load HTML using CORS proxy, then process all links, frames, scripts and styles, and load each of them using CORS proxy, so they can be evaluted by the browser.

**GitHub & BitBucket HTML Preview** was tested under the latest Google Chrome and Mozilla Firefox.
