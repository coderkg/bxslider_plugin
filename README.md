The Responsive jQuery Content Slider

This is my implementation of bxslider in GHOST.


** Link required files & Call the bxSlider **

Add the additional directories/files to the directory [assets] and [partials]

Add the following two lines to the [default.hbs] file just before the closing `</body>` tag.

    <!-- jQuery bxslider in partials -->
    {{> bxslider}}


Restart ghost for changes to take effect.


bxslider configuration options are set in javascript files located in [assets/bxslider/options]. These are referenced from [partials/bxslider.hbs] to initialise the instance.

Refer to http://bxslider.com/ for full documentation and options available in bxslider.  Also have a look at the readme.md in [assets/bxslider].


** Create HTML markup **

Create a `<ul class="bxslider">` element, with a <li> for each slide. Slides can contain images, video, or any other HTML content!

e.g.
```html
ul class="bxslider">
  <li><img src="/images/pic1.jpg" /></li>
  <li><img src="/images/pic2.jpg" /></li>
  <li><img src="/images/pic3.jpg" /></li>
  <li><img src="/images/pic4.jpg" /></li>
</ul>
```
Images can be uploaded into ghost by using the existing image markup method ![]().  This will place the image file in the image storage area.  Alternatively you can place images in a storage area on the server manually.  The links can then be used in the HTML markup for the bxslider.  The markup used for uploading the image files can then be deleted, DON'T delete the image in the preview just the text markup. Images that need to be removed in the future will have to be deleted on the server manually.


 
