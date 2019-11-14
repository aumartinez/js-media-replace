# js-media-replace
A JS media replacement script

## How to use it

Include the script **media-sub.js** to the HTML footer bottom scripts.

## What it does

In our Team we work with a CMS that uses a set of flags (special characters) encoding to embedd templated elements 
or call to media files like images or videos.

We usual call an image like: <code>&lt;img src="^media_src_image.png^" /&gt;</code>, then the CMS script will replace this flag
adding the image file route dinamically.

In our local preproduction enviroment we can mimic this behavior with this script and save time, since there is no requirement 
to manually replace every image call in the HTML code. Just make sure there is an img folder in the local file location, and the script will replace the above to something like: <code>&lt;img src="img/image.png" /&gt;</code>. The script will also pull background images included in the CSS file stylesheet.

While using this script, you may notice in the browser console a list of error messages, this is normal, since the browser will first read the HTML, try to pull the image and since it will not find anything in "^media_src_image.png^", it will throw a "not found" error message.

See a working example at: https://accedo-gps.000webhostapp.com/demo/js-media-replace/index.html

Check in the console the error messages and page source code with the original image flags.
