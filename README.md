# Hi, this is my first website and I'm learning as I go.

My objective is to build 3 very fast performing and simplistic pages that reflect what's on my mind:

* Blog.
* Design Porfolio.
* Gallery, for photographs.

As of right now, only the gallery is functioning well.

## Issues

I'm implementing a responsive gallery (with columns) with responsive images in gallery.html formatted for lazy loading. After 760px the gallery turns into 2 columns, at 1365px 3 columns, at 1920px or higher 4 columns.

<img class="lazyload"
       	src="placeholder.jpg"
        data-srcset="image-360w.jpg 360w,
                     image-512w.jpg 512w,
                     image-750w.jpg 750w"
        data-src="image-750w.jpg"
        sizes="(min-width:761px) 50vw,
               (min-width:1366px) 33.3vw,
               (min-width:1921px) 25vw"
        alt="Description">

In "sizes" I set a min-width at where the 2nd columns appears and it works. But the rest, the several min-widths for each column break point, are not working for me, it loads the biggest every time (I'm not using a Retina Display and have tested in Safari, Firefox and Chrome). Maybe I'm completely overlooking something simple, as I'm very new to this.

I will be testing using the <picture> tag or CSS instead when I have the time. Not sure how lazy loading will work in that case.
