# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 201

# Read: 11 - Assorted Topics

## [HTML & CSS]

### Chapter 16: Images (p. 406-427)

#### Basics
Image size can be controlled using the **_height_** and **_width_** properties in CSS. Specifying image size helps the page load faster. You can use classes to make images more uniform.

``` html

<img src="images/photo.jpg" class="large" alt="photo" />

<img src="images/photo.jpg" class="medium" alt="photo" />

<img src="images/photo.jpg" class="small" alt="photo" />

``` css
img.large {
  width: 500px;
  height: 500px;
}

img.medium {
  width: 250px;
  height: 250px;
}

img.small {
  width: 100px;
  height:1500px;
}
```

There are two main ways you can align an image:
1. Add a float to the image
2. Create a float style

To center the image, you can:
1. add a text align center
2. use margin property with left and right values at auto

``` css
img.large {
  width: 500px;
  height: 500px;
  float: right;
}

img.align-center {
  float: right;
}

img.text-align {
  text-align: center;
}

img.align-center {
  display: block;
  margin: opx auto;
}
```

#### Background Images
You can use an image as a background. If your image is too small, it will repeat itself to fill the empty space. There are 4 background repeating options:
* **_repeat_** - this is the default, image repeats vertically and horizontally
* **_repeat-x_** - this repeats the image strictly horizontally
* **_repeat-y_** - this repeats the image strictly vertically
* **_no-repeat_** - this creates no repeating image

The background attachment property controls if the image is fixed or scrolls with the page.
* **_fixed_** - image stays in the same position
* **_scroll_** - image moves up and down as user scrolls through page.

``` css
body {
  background-image: url("images/pattern.gif");
  background-repeat: /*insert repeat property here*/;
  background-attachment: /*insert attachment property here*/;
}
```

##### position
In a non repeating image, you can specify the location of it's placement. Here are the values you can use:
* left top
* left center
* left bottom

* center top
* center center
* center bottom

* right top
* right center
* right bottom
The default second value is center. You can also use percentage values for a more specific position.

``` css
body {
  background-image: url("images/pattern.gif");
  background-repeat: no-repeat;
  background-position: /*insert position property here*/;
}
```

##### Shorthand
short hand values are as followed:
1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position
``` css
div {
  background: #ffffff url("images/pattern.gif") no-repeat top right;
}
```

#### Linking Images and Buttons
A **_rollover_** is when you place your mouse over a button or link i=and it changes to a second style.
A **_sprite_** is when you use an image multyple times for diffrent interfaces.

#### Gradients and background contrasts
Gradients are hard to explain so here is an example. It's pretty easy to figure it out.
``` css
body {
  background: linear-gradient(90deg, rgb(153, 56, 245) 33%, rgb(41, 41, 41) 33%, rgb(41, 41, 41) 66%, rgb(153, 56, 245) 66%);
}
```
You should change the contrast of an image to make text more legible. Or you add a screen in between the text and the image.

### Chapter 19: Practical Information (p. 476-492)

