[![Build Status](https://travis-ci.org/accesslint/accesslint.js.svg)](https://travis-ci.org/accesslint/accesslint.js)

# Accessibility Warnings for Your Website

accesslint.js warns you of accessibility errors in your website.

## Usage

Download the
[latest release](https://github.com/accesslint/accesslint.js/releases/latest)
and include the javascript in your page at the end of the `<body>` tag.

```
<script src="accesslint.js" type="text/javascript">
```

Open the page and watch your browser's JavaScript console for warnings.

![Firefox JavaScript console with accessibility warnings](https://cloud.githubusercontent.com/assets/108163/15451467/c36dd858-1f91-11e6-9c5f-7a945c7b38f7.png)

## How it works

accesslint.js runs assertions from the
[aXe-core](https://github.com/dequelabs/axe-core) accessibility library wherever
you include the script once on page load, and again for each DOM change event.

This feature gives you feedback on new content introduced via AJAX, for example,
or updates to a single page app.

## Development

### Setup

    $ bin/setup

### Testing

    $ gulp

### Building

#### Development

    $ gulp build-dev # build and watch for changes

#### Production

    $ gulp build
