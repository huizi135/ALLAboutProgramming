```ruby
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Ferris Wheel</title>
    <link rel="stylesheet" href="./styles.css">
  </head>
  <body>
    <div class="wheel">
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>

      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
    </div>
  </body>
</html>
```
```ruby
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
  position: absolute;
  height: 55vw;
  width: 55vw;
  max-width: 500px;
  max-height: 500px;
  animation-name: wheel;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}

.line {
  background-color: black;
  width: 50%;
  height: 2px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform-origin: 0% 0%;
}

.line:nth-of-type(2) {
  transform: rotate(60deg);
}
.line:nth-of-type(3) {
  transform: rotate(120deg);
}
.line:nth-of-type(4) {
  transform: rotate(180deg);
}
.line:nth-of-type(5) {
  transform: rotate(240deg);
}
.line:nth-of-type(6) {
  transform: rotate(300deg);
}

.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
  position: absolute;
  border: 2px solid;
  transform-origin: 50% 0%;
  animation: cabins 10s ease-in-out infinite;
}

.cabin:nth-of-type(1) {
  right: -8.5%;
  top: 50%;
}
.cabin:nth-of-type(2) {
  right: 17%;
  top: 93.5%;
}
.cabin:nth-of-type(3) {
  right: 67%;
  top: 93.5%;
}
.cabin:nth-of-type(4) {
  left: -8.5%;
  top: 50%;
}
.cabin:nth-of-type(5) {
  left: 17%;
  top: 7%;
}
.cabin:nth-of-type(6) {
  right: 17%;
  top: 7%;
}

@keyframes wheel {
   0% {
     transform: rotate(0deg);
   }
   100% {
     transform: rotate(360deg);
   }
}

@keyframes cabins {
  0% {
    transform: rotate(0deg);
  }
  25% {
    background-color: yellow;
  }
  50% {
    background-color: purple;
  }
  75%{
    background-color:yellow;
  }
  100% {
    transform: rotate(-360deg);
  }
}
```
![Screenshot 2023-07-02 185323](https://github.com/huizi135/ALLAboutProgramming/assets/91324319/b1651253-2186-4055-b649-dd289ae9c113)

The `transform-origin` property is used to set the point around which a CSS transformation is applied. For example, when performing a `rotate` (which you will do later in this project), the `transform-origin` determines around which point the element is rotated.

The `@keyframes` at-rule is used to define the flow of a CSS animation. Within the `@keyframes` rule, you can create selectors for specific points in the animation sequence, such as `0%` or `25%`, or use `from` and `to` to define the start and end of the sequence.

The `animation-iteration-count` property sets how many times your animation should repeat. This can be set to a number, or to `infinite` to indefinitely repeat the animation. Your Ferris wheel should never stop, so set the `.wheel` selector to have an `animation-iteration-count` of `infinite`.

The `animation-timing-function` property sets how the animation should progress over time. There are a few different values for this property, but you want the Ferris wheel animation to run at the same rate from start to finish. Set the `animation-timing-function` to `linear` in your `.wheel` selector.
