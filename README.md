# Georgia EPD-IT Logos and Icons

Branding files for use by Georgia EPD.

## EPD logo

The new EPD logo and icon are available in SVG and PNG formats.

![](epd-icon/epd-icon.svg)

## Seal of Georgia 

Available in flat color (vector and bitmapped) and  gold (bitmapped only). The vector file originally came from [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Seal_of_Georgia.svg), which work was released into the public domain by the original author.

![Georgia seal in white](georgia-seal/White/Seal_of_Georgia_white_128x128.png)
![Georgia seal in gold](georgia-seal/Gold/Seal_of_Georgia_gold_128x128x32.png)

## Favicons

To set the shortcut icon for a website:

* Copy the assets in the "favicon/" folder into the root of your application. 
* Copy the appropriate lines from the "_head-snippet.html" file into the `<head>` section of your HTML document.
* Update the "site.webmanifest" file to set the `name` and `short_name` properties.

### DEV/UAT Favicons

To optionally enable alternate favicons for DEV/UAT environments, use the contents of the "favicon-env" folder instead. Don't forget that there are three "site.webmanifest" files to update.

![Favicon examples](favicon-examples.png)
