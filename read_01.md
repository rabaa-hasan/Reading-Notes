# SMACSS and Responsive Web Design
## Responsive Web Design
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

![desktop](https://learn.shayhowe.com/assets/images/courses/advanced-html-css/responsive-web-design/food-sense.png)

### Responsive vs. Adaptive vs. Mobile
Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. With responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors. A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference.
Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users.
Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.

### Flexible Layouts
Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

#### Flexible Grid
Below we have a parent division with the class of container wrapping both the section and aside elements. The goal is to have have the section on the left and the aside on the right, with equal margins between the two.
### HTML
```
<div class="container">
  <section>...</section>
  <aside>...</aside>
</div>

```
### CSS
```
.container {
  width: 538px;
}
section,
aside {
  margin: 10px;
}
section {
  float: left;
  width: 340px;
}
aside {
  float: right;
  width: 158px;
}

```

### Media Queries
Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. 

### Mobile First
One popular technique with using media queries is called mobile first. The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

The mobile first approach also advocates designing with the constraints of a mobile user in mind. Before too long, the majority of Internet consumption will be done on a mobile device. Plan for them accordingly and develop intrinsic mobile experiences.

```
/* Default styles first then media queries */
@media screen and (min-width: 400px)  {...}
@media screen and (min-width: 600px)  {...}
@media screen and (min-width: 1000px) {...}
@media screen and (min-width: 1400px) {...}

```

### Viewport
Mobile devices generally do a pretty decent job of displaying websites these days. Sometimes they could use a little assistance though, particularly around identifying the viewport size, scale, and resolution of a website. To remedy this, Apple invented the viewport meta tag.

![viewPort](https://learn.shayhowe.com/assets/images/courses/advanced-html-css/responsive-web-design/without-viewport.png)

### Flexible Media
The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

```
img, video, canvas {
  max-width: 100%;
}

```

![flexible](https://s3-us-west-2.amazonaws.com/s.cdpn.io/29841/chicago.jpg)

## Float
Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.

![float](https://i1.wp.com/css-tricks.com/wp-content/uploads/2021/03/print-layout.png?w=540&ssl=1)

![web layout](https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/03/web-text-wrap.png?w=540&ssl=1)

### What are floats used for?
Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

![float](https://i2.wp.com/css-tricks.com/wp-content/uploads/2021/03/web-layout.png?w=540&ssl=1)

### Clearing the Float
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.

### The Great Collapse
One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing. This isn’t always obvious if the parent doesn’t contain any visually noticeable background, but it is important to be aware of.

![collapse](https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/03/collapse.png?w=540&ssl=1)

