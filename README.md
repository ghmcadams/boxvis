HTML Box Visualizer
====================

A pure JavaScript based CSS / HTML element visualizer / debugger.  Similar to Chrome's developer tools, this allows you to visualize an element and all of its layout properties in one place.  Add it to any page and move the mouse around the screen.  This tool has no effect on the functionality of your application, but still displays information on any element you mouse over.

## Features

- Display a box around any element you hover over without effecting the functionality of the page
- Display lines showing the margins, borders, and padding of an element
- Display a popover containing information about the element (tagName, id, classes, and dimensions)
- Options (by src attribute querystring) to turn off lines or boxes

## Usage

Add the script to the page using a simple javascript element.  It will be automatically added to the page and start working.  In order for the options to work, add one of the following to the querystring of the src attribute of your script element.

- noln (EX: &lt;script src="....../debugcss.js?noln"&gt;&lt;/script&gt;): this will turn off lines
- nobg (EX: &lt;script src="....../debugcss.js?nobg"&gt;&lt;/script&gt;): this will turn off boxes

## Known limitations

- Does not support psuedo elements (no mouseover events)

## Unknown limitations

I have manually tested this on the following platforms / browsers:

- Mac OS: Chrome Version 53.0.2785.143
- Mac OS: Firefox
- Windows 10: Edge 38.14393.0.0
- Windows 10: Chrome
- Windows 10: IE 11
- Windows 10: Firefox 37.01 & 40.03

## Bookmarklet

Include this link in your toolbar to include boxvis into any page (content security permitting):

```javascript
javascript:(function(){document.body.appendChild(document.createElement('script')).src='//cdn.rawgit.com/ghmcadams/boxvis/master/debugcss.js';})();
```

## Screenshots

![Usage on Nodejs.org](screenshot.png?raw=true)
