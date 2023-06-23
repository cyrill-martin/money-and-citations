# Data Visualization
This repository contains the files of the DaVi term project as part of my Certificate of Advanced Studies in Statistical Data Analysis & Data Visualization at the Swiss Distance University of Applied Sciences.

## Reproduce Locally
In order to reproduce the visualizations locally, a local web server is required so that the data can be loaded from the CSV file.

1. Clone repository with `git clone https://github.com/cyrill-martin/stats-and-dataviz.git`
2. Navigate to the individual files in the cloned repository
3. Start local server in repository
   For example:
   - with [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) for Visual Studio Code
   - or with `python3 -m http.server`
   - Etc.
4. Call up the URL of the local web server in the browser

## Files

### .CSV
The CSV file contains the basic data for the visualizations.

### .HTML
The HTML file contains the HTML template for the website, a lot of JavaScript code for the actual visualizations and for handling the click events on the page, and a few specific styles.

The site is essentially based on [Vue.js](https://vuejs.org/) for the dynamics in the template and the handling of events, and on [D3.js](https://d3js.org/) for the generation of the visualizations. Both libraries are simply integrated into the page using an import map.

```html
<script type="importmap">
  {
    "imports": {
      "vue": "https://unpkg.com/vue@3/dist/vue.esm-browser.js",
      "d3": "https://cdn.skypack.dev/d3@7.1.1"
    }
  }
</script>
```

### .CSS
The CSS file contains a few minimal styles and a simple grid system for rendering on the web.

### .MD
This is the file that is being read here, with the explanations for the other files.
