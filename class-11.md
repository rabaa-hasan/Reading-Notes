## Flash
Since the late 1990s, Flash has been a very popular tool for creating animations, and later for playing audio and video in websites.

### Flash Time Line
![flash](Screenshot(136).png)

![flash1](Screenshot(138).png)

## Controlling sizes of images in CSS
```
img.large {
width: 500px;
height: 500px;}
```

# Images CSS
## AligNing images Using CSS

1. The float property is added to the class that was created to represent the size of the image (such as the small class in our example).

2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page.

```
img.align-left {
float: left;
margin-right: 10px;}
```

## Centering images Using CSS

1. On the containing element, you can use the text-align property with a value of center.

2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

```
img.align-center {
display: block;
margin: 0px auto;}
```

## Background Images
The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page.

`body {background-image: url("images/pattern.gif");}`

### Repeating Images
`background-repeat`
`background-attachment`

`repeat-x`
The image is repeated horizontally only (as shown in the first example on the left).

`repeat-y `
The image is repeated vertically only.

`no-repeat`
The image is only shown once.

`fixed`
The background image stays in the same position on the page.

`scroll`
The background image moves up and down as the user scrolls up and down the page.

```
body {
background-image: url("images/tulip.gif");
background-repeat: no-repeat;
background-attachment: fixed;}
```

## Background Position
`background-position`

* left top
* left center
* left bottom
* center top
* center center
* center bottom
* right top
* right center
* right bottom

## shorthand
`background`

The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property.

1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

## IMAGE Rollovers & Sprites 
Using CSS, it is possible to create a link or button that changes to a second style when a user moves their mouse over it (known as a rollover) and a third style when they click on it.

## Contrast of background images
![image](Screenshot(140).png)

# Practical Information
## Search Engine Optimization (SEO)
SEO is a huge topic and several books have been written on the subject. 

## On-Page SEO
![practical](Screenshot(142).png)

## How to Identify Keywords and Phrases
1. Brainstorm
2. Organize
3. Research
4. Compare
5. Refine
6. Map

Search engine optimization helps visitors find your sites when using search engines.

Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.

To put your site on the web, you will need to obtain a domain name and web hosting.

FTP programs allow you to transfer files from your local computer to your web server.

Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).

## HTML5 video and audio
The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.
