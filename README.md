


# Pure Media - Progressive Lazyloading using lazysizes library.

<p align="center">
  <img src="screenshots/screenshot.jpg" style="max-width:200px;">
</p>

<blockquote>Pure Media is a javascript library for Progressive Image Loading with a blur effect to reduce the page load time of your website. This library uses lazysizes(lazyload) to defer offscreen images. This adds padding to add height to the element.</blockquote>

### Requirements
1. Lazysizes

### Demo

https://localnetwork.github.io/pure-media/index.html


### Note: Good only for non-transparent image.

### How to use

1. Link files to your site or application (add `<script>` to bottom of page)

  ```html
  <link rel="stylesheet" href="dist/css/pure-media.css">
  <script src="dist/js/pure-media.js"></script>
  ```

2. Set markup 

  ```html
  <figure class="graf-figure">
    <div class="aspectRatioPlaceholder">
      <div class="aspectRatioPlaceholder-fill"></div>
      <div class="progressiveMedia lazyload" data-width="1920" data-height="1080">
        <img class="progressiveMedia-thumbnail" src="small-image-path" alt="" />
        <canvas class="progressiveMedia-canvas"></canvas>
        <img class="progressiveMedia-image lazyload" data-src="original-image-path" alt="" />
      </div>
    </div>
  </figure>
  ```

3. Add `src` small-image-path for class  `.progressiveMedia-thumbnail` 

  ```html
  <img class="progressiveMedia-thumbnail" src="small-image-path" alt="" />
  ```

4. Set `data-src="path"` original-image-path for class `.progressiveMedia-image` 

  ```html
  <img class="progressiveMedia-image lazyload" data-src="original-image-path" alt="" />
  ```

5. And finally set original image size (width, height) that you used in `data-src="path"` to `data-width` and `data-height` for class `.progressiveMedia`. For example:

  ```html
  <div class="progressiveMedia lazyload" data-width="1920" data-height="1080">
  ```


## TODO: 
- AJAX Support

Credits to <a href="https://halcyonwebdesign.com.ph/" target="_blank">Halcyon Web Design</a> for development time.
<br>
