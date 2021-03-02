# Transforms
The `transform` property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

## Transform Syntax
```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

## 2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. 

### 2D Rotate
used to rotate an element , values (0 - +-360).

```
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

```

### 2D Scale
used to change the appeared size of an element , default values 1 , values larger than 1 make the element larger , and vlues between 0 and 1 make the element smaller.

```
 .box { transform: scale(0.5); transform: scale(1.5); }
```

### 2D Translate
used to change the position of an element , in both x and y directions.

```
.box-1 {
  transform: translateX(-10px);
}
```

### 2D Skew
used to distort the element , in both the horizontal and vertical axizes.

```
.box-1 {
  transform: skewX(5deg);
}
```

# Transitions

a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including :
* transition-property
* transition-duration
* transition-timing-function
* transition-delay

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```

## CSS3 TRANSITIONS
CSS transitions allows you to change property values smoothly, over a given duration.

![transitions css](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

To create a transition effect, you must specify two things:

* the CSS property you want to add an effect to
* the duration of the effect

```
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}
```

#### Specify the Speed Curve of the Transition
The transition-timing-function property can have the following values:

* ease - specifies a transition effect with a slow start, then fast, then end slowly (this is default)
* linear - specifies a transition effect with the same speed from start to end
* ease-in - specifies a transition effect with a slow start
* ease-out - specifies a transition effect with a slow end
* ease-in-out - specifies a transition effect with a slow start and end
* cubic-bezier(n,n,n,n) - lets you define your own values in a cubic-bezier function


```
#div1 {transition-timing-function: linear;}
#div2 {transition-timing-function: ease;}
#div3 {transition-timing-function: ease-in;}
#div4 {transition-timing-function: ease-out;}
#div5 {transition-timing-function: ease-in-out;}
```


![transition](https://coursework.vschool.io/content/images/size/w2000/2016/08/transition_example2.png)

