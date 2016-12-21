# Georgia EPD-IT Logos and Icons

Branding files for use by Georgia EPD-IT

## EPD logo

New EPD logo/icon provided by Erin Ruoff. Available in SVG and PNG.

![](https://bytebucket.org/gaepdit/ga-epd-brand/raw/master/dist/logos/epd-icon.svg)

## Seal of Georgia 

Available in gold (bitmapped only) and flat color (vector). Vector file originally came from [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Seal_of_Georgia.svg), which work was released into the public domain by the original author.

![](https://bytebucket.org/gaepdit/ga-epd-brand/raw/master/dist/logos/Seal_of_Georgia_white.svg)

## How to use

* The `src` directory contains original source files.
* The `dist` directory contains generated and optimized files for use in production.

Run `npm install --save ga-epd-brand` to include these files as a dependency in your project. Add a gulp task in `gulpfile.js` to copy the desired files to the appropriate destination. For example,

```js
var paths = {
    webRoot: './wwwroot/',
    assetsRoot: './wwwroot/assets/',
    gaBrand: './node_modules/ga-epd-brand/dist/**/*',
    gaFavicons: './node_modules/ga-epd-brand/dist/epd-favicons/*',

};

gulp.task('brand.copyFiles', function () {
    return gulp.src([paths.gaBrand, '!' + paths.gaFavicons])
        .pipe(gulp.dest(paths.assetsRoot));
});

gulp.task('brand.copyFavicons', function () {
    return gulp.src(paths.gaFavicons)
        .pipe(gulp.dest(paths.webRoot));
});
```

## Favicons

To use the new epd icon as a shortcut icon in a website, first copy all of the assets in the `dist/epd-favicons/` folder into the webroot. Then copy the following lines into the `<head>` section of your HTML pages:

```html
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png?v=69kRrvbXdL">
<link rel="icon" type="image/png" href="/favicon-32x32.png?v=69kRrvbXdL" sizes="32x32">
<link rel="icon" type="image/png" href="/favicon-16x16.png?v=69kRrvbXdL" sizes="16x16">
<link rel="manifest" href="/manifest.json?v=69kRrvbXdL">
<link rel="mask-icon" href="/safari-pinned-tab.svg?v=69kRrvbXdL" color="#5bbad5">
<link rel="shortcut icon" href="/favicon.ico?v=69kRrvbXdL">
<meta name="theme-color" content="#e5f6fa">
```
