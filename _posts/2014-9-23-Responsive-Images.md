---
layout: post
title: Responsive Images!
---

Human beings are visual creatures and we tend to gravitate towards visuals rather than words. Humans are self-centered, always asking what is there for me. So the role of the developer and designer is to create an experience that will create visually appealing websites with good content for the user. 

Responsive images are a crucial part of a website’s success. Just picture a site full of blocks of text would you bother reading it? Wouldn’t you get a headache from reading so much content without allowing your eyes a rest? I’m sure there’s a way to showcase images in web design and sure there is!


###This is how you would implement responsive images using CSS

First you need to create a class in CSS follow by the different attributes that will allow you to have a better control over the image. You can also use these attributes: ``` background-repeat```, ```background-position```, ```background-color```. 

```
.someclass {
        background-image: url('image.jpg');
        height:400px;
}
```
In your HTML the class you created above is then inserted in a class tag wherever you want the image to appear. 

```
<header class="someclass">
// text or whatever content
</header>
```

WOOLA! The image will appear in the header portion of the page because that's where I placed the class tag. Sadly you can only do so much with background images and sometimes you need find another solution. 

###This is how you would implement responsive images using a Polyfill called Picturefill.

Picturefill works like the good-old img tag but the Picturefill gives you more control than the ```img``` tag. 

In order for the browser to understand the picture tag you need to add a two pieces of script to the ```head``` of your page:

``` 
<script>
// Picture element HTML5 shiv
document.createElement("picture");
</script>
``` 
``` 
<script src="picturefill.js" async></script>
``` 

Now you are ready to use the ``` picture``` tag to implement responsive images to your site. 
   
   
    <picture>
      <source media="(min-width: 1024px)" srcset="images-desktop.jpg, images-desktop@2x.jpg 2x"></source>
      <source media="(min-width: 768px)" srcset="images-tablet.jpg, images-tablet@2x.jpg 2x"></source>
      <img srcset="images-mobile.jpg, images-mobile@2x.jpg 2x" alt="some-text!">
    </picture>

***If you're going mobile first, you must supply your sources from largest to smallest.***

Here are more reasons why responsive images are important!

Picture yourself browsing a site in your mobile phone in your basement. I bet you are pulling your hair out, right? You bet! Most likely the site is taking forever to load because the Internet connection is poor in most basements. That is why responsive images are important because it allows the developer to control what pair of images the browser is going to download. Responsive images also help “maintain” the site layout. If the images are too big it may potentially break the layout design. Responsive images plays an important role in web design, not only it loads different size images according the device size, it also helps the designer art direct the type of images each break point will showcase allowing the user to experience a better site. 

The web is always evolving as new technology allows developers to control the creation of the web in a more efficient way. After all, every developer and designer wants their work to be seen and enjoy by many. Little by little we create a better web. 


