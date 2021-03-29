# Flexbox and Templating
## Javascript Templating
Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

## Mustache
![m](https://miro.medium.com/max/700/1*P9q0tkeaRY2l1JOXaVKAig.png)

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

It is referred to as "logic-less" because there are no if statements, else clauses, or for loops. There are only tags. Some tags are replaced with a value, some nothing ,and other a series of values.

Mustache.js is an implementation of the mustache template system in JavaScript. It is considered the base for JavaScript templating

```
Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn
```

![me](https://miro.medium.com/max/700/1*LbqYj87xlazySm6wE0Q2lA.png)

### Mustache-Express
If you intend you use mustache with Node and Express, you can use mustache-express. 

## Flexbox CSS
### Flexbox properties
The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

### Properties for Flex
#### display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
```
.container {
  display: flex; /* or inline-flex */
}
```

#### Align Items

* flex-start: Items align to the top of the container.

* flex-end: Items align to the bottom of the container.

* center: Items align at the vertical center of the container.

* baseline: Items display at the baseline of the container.

* stretch: Items are stretched to fit the container.

#### Flex Direction

* row: Items are placed the same as the text direction.

* row-reverse: Items are placed opposite to the text direction.

* column: Items are placed top to bottom.

* column-reverse: Items are placed bottom to top.

#### Order

Sometimes reversing the row is not enough. We need to use the Order property to individual items. By default items have a value of 0, but we can set to a positive or negative interger.
Align Self

This property accepts the same values as align-items and it is a value for a specific item.

#### Flex Wrap

* nowrap: Every item is fit to a single line.

* wrap: Items wrap around to additional lines.

* wrap-reverse: Items wrap around to additional lines in reverse.

* Flex Flow

The two properties of flex-direction and flex-wrap are often used together and the shorthand property is flex-flow.

#### Align Content

* flex-start: Lines are packed at the top of the container.
* flex-end: Lines are packed at the bottom of the container.
* center: Lines are packed at the vertical center of the container.
* space-between: Lines display with equal spacing between them.
* space-around: Lines display with equal spacing around them.
* stretch: Lines are stretched to fit the container.