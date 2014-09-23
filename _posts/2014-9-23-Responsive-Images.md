---
layout: post
title: Responsive Images!
---

Human beings are visual creatures and we tend to gravitate towards visuals rather than words. Humans are self-centered, always asking what is there for me. So the role of the developer and designer is to create an experience that will create visually appealing websites with good content for the user. 

Responsive images are a crucial part of a website’s success. Just picture a site full of blocks of text would you bother reading it? Wouldn’t you get a headache from reading so much content without allowing your eyes a rest? I’m sure there’s a way to showcase images in web design and sure there is!

You can implement responsive images by using CSS or using a Picturefill. 

This is how you would implement responsive images using CSS

First you need to create a class in CSS follow by the different attributes that will allow you to have a better control over the image. You can also use these attributes: background-repeat, background-position, background-color. 

```
.someclass {
        background-image: url('image.jpg');
        height:400px;
}
```

In your HTML the class you created above is then inserted in a class tag wherever you want the image to appear. 
```
<header class="someclass">
  <h1>some-text</h1>
</header>

```
WOOLA! The image will appear in the header portion of the page because that's where I placed the class tag. 
