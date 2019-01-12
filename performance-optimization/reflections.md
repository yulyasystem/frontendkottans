## Web Performance Optimization 

Things which suprise me in performance checklist article that you should keep in mind too many things and tools to keep your page optimizated. Such things as PRPL pattern, REST, responsive images and more. 

`` To guarantee high performance, as developers, we need to find ways to write and deploy less JavaScript.``

After reading this article I have got a little stress, it might be entire course on this article :)

Ways to optimize JS:

* minification, it makes code take around 30-40% less size
* use `async, defer`. These attributes let the browser know that scripts can be downloaded in the background without interrapting the document parsing. `async` asks the browser to load scripts asyncronously and `defer` tells the browser to download the script asynchronously and execute it only after the document is parsed
* code splitting, it is needed a bundler like webpack
* remove unused code

Ways to optimize CSS:

* minify 
* critical CSS

Ways to optimize networking staff:
* tranfer fewer data over network => minimify HTML
* compress text by Gzip or Brotli, the first one compreses data you send to the client, it reduces by 60-80%, but stay unreadable
* CDN 

Images:
* use proper formats, svg is best for icons or logos, jpg for photos, png for raster graphics
* compression, jpg by decreasing image dimensions, do not let browser download unnecessarily large file, use progressive JPEG, it starts rendering in bad quality but improves as img being loaded, use interlaced PNG

Fonts:
* fallback fonts
* `font-display` property adjust the way custom font is applied, for example `font-display: fallback` browser wil immediately render available font.

The course from Udacity was easy. The new was CCSOM it is like the DOM but for css, it allows to modify styles dynamically. 

More specific rules reqire more work in CSS. 

![image of udacity ](https://github.com/yulyasystem/kottans-frontend/blob/master/performance-optimization/performance.png)

In Browser Rendering Optimization course new for me was RAIL. Every app has its own lifecycle and performance fits into them in different ways




