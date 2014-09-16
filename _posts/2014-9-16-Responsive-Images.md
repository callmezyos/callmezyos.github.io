---
layout: post
title: 9-16-2014 Blog Post
---

## Why Responsive Pages are both Useful and Difficult to Use
Responsive images are needed because not everyone viewing a webpage could be using the same device. Having said that, different
devices have different resolutions and thats not even including the devices that have high defination screens. So with today's day
in age web developers need to be able to plan for what device people may be using to view the said webpage.

They are also difficult to use because at least for myself, different media queries are used for different things. Once again,
speaking frankly for myself, I am not that strong of a programmer so trying to get a hold of everything has been a challenege.
Another reason that Responsive Images are difficult because the developer has to create several media queries to try and cover
sort of devices that may be used in viewing the webpage.

### Responsive Images Using CSS

```
/* tablet */
  @media (min-width: 768px) {
    .page-heading {
      font-size: 28px;
    }

    .frisbee {
      font-size: 30px;
      background-image: url('frisbee-tablet.jpg');
      width: 420px;
      height: 420px;
      background-size: 420px 420px;
    }
  }

  /* high res tablet */
  @media (-webkit-min-device-pixel-ratio: 2) and (min-width: 768px),
    (min-resolution: 192dpi) and (min-width: 768px) {

    .frisbee {
      background-image: url('frisbee-tablet@2x.jpg');
    }
  }
```

### Responsive Images Using PictureFill

```
 <script type="text/javascript">
  document.createElement('picture');
  </script>

  <script scr="picturefill.js" async></script>
```
