# svg_update_v5
Treehouse Front End Web Development Project 8

### Project Overview

-   #### Background

    -   In `styles.css`, use the `background.svg` file to create a tiled background on the `body` of the site, as shown on the mockup.
    
 ````
 body {
  margin: 0;
  padding: 0;
  text-align: center;
  font-family: 'Roboto Slab', serif;
  font-weight: 300;
  color: #111;
  /* Step one: match the mock image background using the background svg */
  background: #edeff0 url('svgs/background.svg') repeat;
}
 ````

-   #### Menu

    -   Create a navigation menu to match the mockups using the supplied SVGs.
    -   When a user hovers over a nav menu item, use CSS to change the color of both the text AND the inline SVG.
    
````
<nav>
  <ul>
    <li>
      <a href="#">
        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="24" class="nav__svg" viewBox="0 0 28 24" ><path d="M28 7.1C28 4.2 25.5 0 20.7 0 15.8 0 14 6.6 14 6.6S12.2 0 7.3 0C2.5 0 0 4.2 0 7.1c0 2.1-.6 3.7 4.2 8.7C6.3 18 9.7 19.7 14 24c4.3-4.3 7.8-6 9.8-8.1 4.8-5 4.2-6.7 4.2-8.8z"/></svg>
        Home
      </a>
    </li>
    <li>
      <a href="#">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" class="nav__svg" viewBox="0 0 24 24">
          <path d="M19.5 7.1C19.3 3.2 16 0 12.1 0c-2 0-3.9.8-5.3 2.2-1.3 1.3-2.1 3-2.3 4.9V8c.3 9.3 6.2 15 6.9 15.7.2.2.4.3.7.3.2 0 .5-.1.7-.3.7-.6 6.5-6.4 6.8-15.6-.1-.2-.1-.9-.1-1zM9 7.5c0-1.7 1.3-3 3-3s3 1.3 3 3-1.3 3-3 3-3-1.3-3-3z"
            />
        </svg>
        Visit Us
      </a>
    </li>
    <li>
      <a href="#">
      <svg xmlns="http://www.w3.org/2000/svg" width="28" height="24" class="nav__svg" viewBox="0 0 28 24">
        <path d="M10.1 22.5c1.5.7 3.1 1 4.8 1 6.5 0 11.8-5.3 11.8-11.8C26.6 5.3 21.3 0 14.8 0S3.1 5.3 3.1 11.8c0 1.8.4 3.5 1.1 5-.1.1-3.9 4.8-2.5 6.2l.5.5c1.5 1.5 7.7-.8 7.9-1z"
           />
      </svg>
      Contact
    </a>
    </li>
  </ul>
</nav>
````

-   #### Logo

    -   Insert the SVG logo image (`logo.svg`) to match the mockup using the inline SVG method.
````
<h1 class="logo__text">Paw Print Kennels</h1>
<svg id="Layer_1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 140 120" class="logo">
  <style>
    .st1 {
      fill: #eaaa7f
    }

    .st2 {
      fill: #f4c6a6
    }
  </style>
  <ellipse cx="70.4" cy="69.9" rx="50.4" ry="50.1" fill="#ba8058" />
  <path class="st1" d="M.6 62.5c.2-1.5.7-2.7 1.5-3.5s1.9-1.2 3.1-1.1c1.2.1 2.1.6 2.8 1.6.7 1 .9 2.2.8 3.7l-.2 2.2 1.6.2.5-1.6 1.8.2-.6 6.1-1.8-.2-.1-1.6-7.7-.7-.5 1.6-1.8-.2.1-1.6.5-5.1zm5.7 2.7l.2-2.2c.1-.6-.1-1.1-.4-1.5-.3-.4-.7-.6-1.2-.7-.5 0-.9.1-1.3.4-.4.3-.6.8-.7 1.4l-.2 2.2 3.6.4zM11.2 58.3l.1-.8-8.4-6.7 1-3.1 10.7-.7.4-.8 1.7.5-1.4 4.4-1.6-.5.1-.7h-1.3l-1.2 3.8 1.1.8.4-.6 1.6.5-1.4 4.4-1.8-.5zm-1.6-5.8l.8-2.5-3.8.2v.1l3 2.2zM15.9 28.2l-.4.8 7.4 7.1-1.5 2.5-7-2v.1l5.1 5.1-1.5 2.6-9.8-3.1-.6.7L6 41l2.7-4.4 1.6.9-.4 1.2 5.1 1.9v-.1l-5.4-5.4 1.3-2.1 7.2 2.2v-.1L14 31.7l-.8.9-1.6-.9 2.7-4.4 1.6.9zM25.3 16.4c1.2-1 2.3-1.5 3.5-1.5 1.2 0 2.2.4 3 1.3.8.9 1.1 2 .9 3.1-.2 1.2-.9 2.3-2 3.2L29 24.1l1.1 1.2 1.4-.8 1.2 1.4-4.7 4-1.2-1.4 1-1.3-5-5.9-1.4.8-1.2-1.4 1.2-1 3.9-3.3zm2.2 5.9l1.7-1.4c.5-.4.8-.9.8-1.4.1-.5-.1-.9-.4-1.3-.3-.4-.7-.6-1.3-.6-.5 0-1 .2-1.5.6l-1.7 1.4 2.4 2.7zM36.8 8.7c1.3-.7 2.5-1 3.6-.8 1.1.2 1.9.7 2.4 1.7.3.6.4 1.2.3 1.7-.1.6-.4 1.2-.8 1.8.7-.2 1.4-.1 1.9.2.5.3.9.7 1.3 1.3l.3.6.9-.3.9 1.6-2.9 1.5c-.3 0-.6-.1-.8-.4l-.6-.9-.4-.7c-.3-.5-.6-.8-1-.9-.4-.1-.8 0-1.3.2l-1.6.9 1 1.9 1.5-.5.9 1.6-5.4 2.9-.9-1.6 1.2-1-3.7-6.8-1.5.5-.9-1.6 1.3-.7 4.3-2.2zm1.1 5.5l1.5-.8c.5-.3.8-.6 1-1 .1-.4.1-.8-.1-1.2-.2-.4-.5-.6-1-.7-.4-.1-.9 0-1.4.3l-1.5.8 1.5 2.6zM44.9 6.8l-.6-1.7 5.9-2 .6 1.7-1.4.8 2.6 7.3 1.6-.2.6 1.7-5.9 2-.6-1.7 1.4-.8-2.6-7.3-1.6.2zM66.5 0l.3 1.8-1.5.5 1.5 9.7-3 .5-5.7-6.6H58l.8 5.2 1.6.1.3 1.8-6.1.9-.3-1.8 1.5-.5L54.6 4 53 3.9l-.3-1.8 1.6-.2 3-.5L63 7.9h.1l-.8-5.1-1.6-.1-.3-1.8 4.5-.7 1.6-.2zM81.1.9l-.3 3.8-2.3-.2V3l-1.9-.1-.6 7.5 1.6.4-.1 1.8-6.2-.5.1-1.8 1.6-.2.6-7.5-1.9-.1-.3 1.5-2.3-.2.3-3.8 11.7.9zM89 4.5l.7-1.7L95 4.9l-.7 1.7-1.2-.1-1 2.5.9.2 2.7-2.1-.6-.4.7-1.7 5.1 2-.7 1.7-1.2-.1-3.6 2.3 1.1 5.1.9.6-.6 1.7-5.1-2 .6-1.7.6.1-.6-3.2-1-.4-.9 2.4 1 .7-.7 1.8-5.4-2.1.6-1.7 1.6.3 2.8-7.2-1.3-.8zM97.1 18.6l1-1.5 1.5.6 4.2-6.5-1.2-1.1 1-1.5 1.3.9 7.3 4.7-2 3.1-1.9-1.2.6-1.2-2.8-1.8-1.4 2.2 4 2.6-1 1.6-4-2.6-1.6 2.4L105 21l.8-1.1 1.9 1.2-2 3-8.6-5.5zM125.1 26.3l-1.3 1.3-1.3-.9-7.1 6.9-2.1-2.1 2-8.5h-.1l-3.8 3.7.9 1.4-1.3 1.3-4.3-4.4 1.3-1.3 1.3.9L115 19l-.9-1.4 1.3-1.3 1.1 1.1 2.1 2.1-2 8.4h.1l3.7-3.6-.9-1.4 1.3-1.3 3.2 3.3 1.1 1.4zM134 40.9l-1.6.9-1.1-1.2-8.5 4.9-1.5-2.6 4-7.7-4.5 2.6.5 1.5-1.6.9-3.1-5.3 1.6-.9 1.1 1.2 6.7-3.9-.5-1.5 1.6-.9.8 1.4 1.5 2.6-4 7.7 4.5-2.6-.5-1.5 1.6-.9 2.3 4 .7 1.3zM123.7 47.3l1.7-.5.8 1.4 7.4-2.3-.2-1.6 1.7-.5.5 1.5 2.6 8.3-3.5 1.1-.7-2.2 1.3-.5-1-3.2-2.5.8 1.4 4.5-1.8.6-1.4-4.5-2.7.9 1 3.2 1.3-.3.7 2.2-3.5 1.1-3.1-10zM127.1 58.3l1.8-.2.5 1.6 7.7-.9.1-1.6 1.8-.2.2 1.6.3 3 .2 1.6-1.8.2-.5-1.6-7.5.9.4 3h1.5l.3 2.3-3.8.4-1.2-10.1zM131 76.3c.4 0 .7-.1 1-.4.3-.3.5-.9.8-1.7.4-1.5.9-2.6 1.5-3.3.6-.7 1.4-1 2.5-.9 1 .1 1.8.6 2.4 1.5.6.9.8 2.1.7 3.5-.1 1.5-.5 2.6-1.3 3.4-.7.8-1.7 1.1-2.8 1h-.1l.2-2.9c.5 0 .9-.1 1.2-.3.3-.3.5-.7.5-1.4 0-.6 0-1.1-.2-1.3-.2-.3-.5-.5-.8-.5-.4 0-.7.1-1 .4-.3.3-.5.9-.8 1.9-.4 1.4-.9 2.5-1.5 3.2-.6.7-1.4 1-2.5.9-1.1-.1-1.9-.6-2.5-1.5-.6-1-.8-2.2-.7-3.7.1-1.6.5-2.8 1.3-3.7.7-.9 1.7-1.2 2.9-1.1h.1l-.2 2.9c-.6 0-1 .1-1.3.5-.3.4-.4.9-.5 1.6 0 .7 0 1.2.2 1.5.3.1.6.3.9.4z"
  />
  <g>
    <path class="st2" d="M80.4 45.2c0 5.7-4.6 6.8-10.3 6.8-5.7 0-10.3-1.1-10.3-6.8S64.4 35 70.1 35c5.7 0 10.3 4.6 10.3 10.2zM45.7 83.1c0-13.4 11-18.1 24.4-18.1s24.4 4.7 24.4 18.1-15.1 21.6-24.4 21.6c-8.9 0-24.4-8.2-24.4-21.6zM104 64.1c-4 4-8.1 1.5-12.1-2.5s-6.5-8-2.5-12 10.5-4 14.6 0c4 4 4 10.5 0 14.5zM51.5 49.6c4 4 1.5 8-2.5 12s-8.1 6.5-12.1 2.5-4-10.5 0-14.5 10.5-4 14.6 0z"
    />
  </g>
</svg>
````
    -   Ensure the logo SVG is the styled to the same size as the mockup example (140px x 120px).
````
/* Step three (b): Ensure the logo SVG is styled to the same size as the mockup example
(140px x 120px). */
.logo {
  width: 140px;
  height: 120px;
  transform-origin: 50% 50%;
  transition: all 3s;
}
/* Extra credit: Add a CSS transition effect to the logo hover state  */
.logo:hover {
  transform: rotateY(360deg);
}
````
    -   At a page width of less than 425 pixels, remove the text from the logo and add an H1 tag that contains the logo text.
````
.st1 {
  visibility: hidden;
}

.logo__text {
  visibility: visible;
  color: #EAAA7F;
}

@media (min-width: 425px) {
  .st1 {
    visibility: visible;
  }

 .logo__text {
   visibility: hidden;
 }
}
````

-   #### Dog Images

    -   Use the `corgi.svg` to create a `<symbol>` element for corgis in the the `index.html` file
    -   Use the `<use>` element to recreate four copies of the corgi svg in the layout of index.html matching the mockup
````
<svg width="170" height="170">
    <use xlink:href="#corgi" class="corgi__whole" />
    <use xlink:href="#corgiBody" class="corgi__body--sable" />
    <use xlink:href="#whiteSpace" class="corgi__white" />
    <use xlink:href="#noseAndEyes" class="corgi__nose" />
    <use xlink:href="#brows" class="corgi__brows" />
  </svg>
<span>Sable</span>
````
    -   Use the 'currentColor' CSS value to make the body of each corgi unique, matching the mockup
````
.corgi__collar span {
  display: block;
  padding-right: 40px;
  text-align: center;
}

.hidden {
  display: none;
}

.corgi__body--sable {
  color: #B97F5B;
}

.corgi__body--fawn {
  color: #E9AA82;
}

.corgi__body--red {
  color: #834B29;
}

.corgi__body--stone {
  color: #52595E;
}

.corgi__nose {
  color: #2D3339;
}

.corgi__brows {
  color: #D8805C;
}

.kennel {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
````
