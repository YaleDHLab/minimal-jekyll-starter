# Note: This repository has been archived
This project was developed under a previous phase of the Yale Digital Humanities Lab. Now a part of Yale Library’s Computational Methods and Data department, the Lab no longer includes this project in its scope of work. As such, it will receive no further updates.


# Minimal Jekyll Starter

This repository contains minimal boilerplate for building a Jekyll site with a custom theme.

## Quickstart

First clone the application and install the Ruby dependencies:

```
git clone https://yaledhlab/minimal-jekyll-starter
cd minimal-jekyll-starter
bundle install
```

Then start the server:

```
bundle exec jekyll serve
```

The application will then be hosted on `http://localhost:4000`. Here is the 404 page:

![App preview](./_includes/assets/images/preview.png?raw=true)

## CSS Files

All css assets are included in `_includes/assets/css`. To add additional css files, just place those CSS files in that directory then add them to the bundled and minified css for the application by adding the following line to `_includes/assets/css/app.css`:

```
{% include assets/css/my-new-css-file.css %}
```

The new stylesheet will then be included in the bundled and minified output. This minified stylesheet is inlined into rendered pages to reduce network requests (google.com does this too).

## JS Files

All js assets are included in `_includes/assets/js`. To add new js files, just add those JS files to that directory and then add them to the bundled ad minified js for the application by adding the following line to `_includes/assets/js/app.js`:

```
{% include assets/js/my-new-js-file.js %}
```

Like the CSS for this app, the JS will be minified and rendered inline on the page to reduce the number of network requests required to render each page.
