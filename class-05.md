#  HTML Images; CSS Color & Text
## Choosing Images for Your Site
A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.

## Tips for Selecting the Perfect Images for Your Website
* __The Value of Uniqueness__ : Many companies and designers turn to stock photo sites when they are searching for images to use on websites. The benefit of these websites is that they have an impressive selection of images to choose from and the pricing on those images is usually very reasonable.

* __Custom Images__ :Of course, a surefire way to ensure that the images you use your site are unique is to hire a professional photographer to take custom shots just for you.

* __Be Aware of Licensing__ :When downloading images from stock photo sites, one thing to be mindful of is the licensing under which those images are offered. Three common licenses you will encounter are Creative Commons, Royalty Free, and Rights Managed.

* __Image Size__ :it is important to determine what size you need an image to be so that you can find files that will work within those specifications and which will also work well across various devices and screen sizes. 

## Storing Images on Your Site
If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.
## Adding Images
To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:
* __src__ : This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
* __alt__ :This provides a text description of the image which describes the image if you cannot see it.

![alt](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML/alt-text.png)

* __title__  : You can also use the title attribute with the `<img>` element to provide additional information about the image.

![title](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML/image-with-title.png)

* __height__ :This specifies the height of the image in pixels.
* __width__ :This specifies the width of the image in pixels.

The images you use on your website should be saved at the same width and height that you want them to appear on the page.

* __align__ :The align attribute can take these horizontal values: 
    1. left 
    2. right
    3. top
    4. middle 
    5. bottom

## Where you place the image in the code
it is important because browsers show HTML elements in one of two ways:
1. Block elements always appear on a new line.
2. Inline elements sit within a block level element and do not start on a new line.

## Three Rules for Creating Images
1. Save images in the right format
2. Save images at the right size
3. Use the correct resolution

## Cropping Images
When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

## JPEG vs PNG vs GIF — which image format to use and when?
* __JPEG__ is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality.

![jpeg](https://miro.medium.com/max/700/1*HnECuWHjR2g4V7RAGmdmrg.jpeg)

* __PNG__ is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper.

![png](https://miro.medium.com/max/700/1*sD2tU56l8y1jF4BPQdWNYA.png)

* __GIF__ is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. 

![gif](https://miro.medium.com/max/700/1*RC1_APSn_bNGP4dYpR9MJw.gif)


# Colors in CSS 
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

1. rgb values :  `p {color: rgb(100,100,90);}`
2. hex codes : `h2 {color: #ee3e80;}`
3. color names : `h1 {color: DarkCyan;}`
4. RGBA Color Values : it's just like RGB, except with the addition of a fourth value: the alpha channel. `<li style="background-color: rgba(255, 0, 0, 1)"></li>`
5. HSL: The HSL color model is one of the least used, but gaining traction because can be more intuitive to use when working with shades and color adjustments.
`hsl(240, 100%, 90%)`
6. HSLA: HSLA is simply the HSL color model with the addition of an alpha channel. This works exactly the same way as the alpha channel in RGBA.
`h1 {background-color: hsla(240, 25%, 50%, .5);}`


Color pickers can help you find the color you want.

It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).

CSS3 also allows you to specify colors as a RGBA ,HSL values, with an optional opacity value. It is known as HSLA.

## Text in CSS 
### Typeface Terminology
Typeface vs. Font
This is how the two have traditionally been defined and distinguished from one another:

Typeface: The design of a collection of glyphs (e.g. letters, numbers, symbols)

Font: A specific size, weight, or style of a typeface (e.g. regular, bold, italic)

#### Typeface Terminology:
1. Serif : Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
2. Sans-Serif
Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

![serif](https://i2.wp.com/css-tricks.com/wp-content/uploads/2019/02/s_FB64E0419C360FFF493C6558F3D017A34BD0F14D3B3A1B417EB66C07CF44FFD2_1548860551288_serifvssans.png?ssl=1)

3. Monospace : Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

![mono](https://i0.wp.com/css-tricks.com/wp-content/uploads/2019/02/monospace.jpg?ssl=1)


![pic](Screenshot(5).png)

When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.
`body {font-family: Georgia, Times, serif;}`

The font-size property enables you to specify a size for the font.
`body {font-family: Arial, Verdana, sans-serif; font-size: 12px;}`

You may have noticed that programs such as Word, Photoshop and InDesign offer the same sizes of text.

### Units of Type Size
![size](Screenshot(6).png)

You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.

You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

