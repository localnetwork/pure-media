# Medium - Progressive Image Loading + Lazysizes (Lazyloading Images)

Medium is a tiny, pure JavaScript library for Progressive Image Loading with a blur effect to reduce the page load time; as seen on [Medium](https://medium.com/designing-medium/image-zoom-on-medium-24d146fc0c20) and the [lazyload functionality](https://github.com/aFarkas/lazysizes). 

### Demo

Download and extract the file and see index.html to see the demo.

### How

1. Link files to your site or application (add `<script>` to bottom of page)

  ```html
  <link rel="stylesheet" href="css/style.css">
  <script src="pure-media.js"></script>
  ```

2. Set markup 

  ```html
  <div class="aspectRatioPlaceholder">
    <div class="aspectRatioPlaceholder-fill"></div>
    <div class="progressiveMedia lazyload" data-width="1920" data-height="1080">
      <img class="progressiveMedia-thumbnail" src="small-image-path" alt="" />
      <canvas class="progressiveMedia-canvas"></canvas>
      <img class="progressiveMedia-image lazyload" data-src="original-image-path" alt="" />
    </div>
  </div>
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

