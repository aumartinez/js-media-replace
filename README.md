# js-media-replace
A JS media replacement script

## How to use it

Include the script to the HTML footer bottom scripts.

## What it does

In our Team we work with a CMS that uses a set of flags (special characters) encoding to embedded templated elements 
or call to media files like images or videos.

We usual call an image like: <code>&t;img src="^media_src_image.png^" /&gt;</code>, then the CMS script will replace this flag
adding the image file route dinamically.

In our local preproduction enviroment we can mimic this behavior with this script and save time, since there is no requirement 
to manually replace every image call in the HTML code.
