
```ruby
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Magazine</title>
    <link
      href="https://fonts.googleapis.com/css?family=Anton%7CBaskervville%7CRaleway&display=swap"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://use.fontawesome.com/releases/v5.8.2/css/all.css"
    />
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <main>
      <section class="heading">
        <header class="hero">
          <img
            src="https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png"
            alt="freecodecamp logo"
            loading="lazy"
            class="hero-img"
          />
          <h1 class="hero-title">OUR NEW CURRICULUM</h1>
          <p class="hero-subtitle">
            Our efforts to restructure our curriculum with a more project-based
            focus
          </p>
        </header>
        <div class="author">
          <p class="author-name">
            By
            <a href="https://freecodecamp.org" target="_blank" rel="noreferrer"
              >freeCodeCamp</a
            >
          </p>
          <p class="publish-date">March 7, 2019</p>
        </div>
        <div class="social-icons">
          <a href="https://www.facebook.com/freecodecamp/">
            <i class="fab fa-facebook-f"></i>
          </a>
          <a href="https://twitter.com/freecodecamp/">
            <i class="fab fa-twitter"></i>
          </a>
          <a href="https://instagram.com/freecodecamp">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="https://www.linkedin.com/school/free-code-camp/">
            <i class="fab fa-linkedin-in"></i>
          </a>
          <a href="https://www.youtube.com/freecodecamp">
            <i class="fab fa-youtube"></i>
          </a>
        </div>
      </section>
      cc
      <section class="text text-with-images">
        <article class="brief-history">
          <h3 class="list-title">A Brief History</h3>
          <p>Of the Curriculum</p>
          <ul class="lists">
            <li>
              <h4 class="list-subtitle">V1 - 2014</h4>
              <p>
                We launched freeCodeCamp with a simple list of 15 resources,
                including Harvard's CS50 and Stanford's Database Class.
              </p>
            </li>
            <li>
              <h4 class="list-subtitle">V2 - 2015</h4>
              <p>We added interactive algorithm challenges.</p>
            </li>
            <li>
              <h4 class="list-subtitle">V3 - 2015</h4>
              <p>
                We added our own HTML+CSS challenges (before we'd been relying on
                General Assembly's Dash course for these).
              </p>
            </li>
            <li>
              <h4 class="list-subtitle">V4 - 2016</h4>
              <p>
                We expanded the curriculum to 3 certifications, including Front
                End, Back End, and Data Visualization. They each had 10 required
                projects, but only the Front End section had its own challenges.
                For the other certs, we were still using external resources like
                Node School.
              </p>
            </li>
            <li>
              <h4 class="list-subtitle">V5 - 2017</h4>
              <p>We added the back end and data visualization challenges.</p>
            </li>
            <li>
              <h4 class="list-subtitle">V6 - 2018</h4>
              <p>
                We launched 6 new certifications to replace our old ones. This was
                the biggest curriculum improvement to date.
              </p>
            </li>
          </ul>
        </article>
        <aside class="image-wrapper">
          <img
            src="https://cdn.freecodecamp.org/testable-projects-fcc/images/random-quote-machine.png"
            alt="image of the quote machine project"
            loading="lazy"
            class="image-1"
            width="600"
            height="400"
          />
          <img
            src="https://cdn.freecodecamp.org/testable-projects-fcc/images/calc.png"
            alt="image of a calculator project"
            loading="lazy"
            class="image-2"
            width="400"
            height="400"
          />
          <blockquote class="image-quote">
            <hr />
            <p class="quote">
              The millions of people who are learning to code through freeCodeCamp
              will have an even better resource to help them learn these
              fundamentals.
            </p>
            <hr />
          </blockquote>
          <img
            src="https://cdn.freecodecamp.org/testable-projects-fcc/images/survey-form-background.jpeg"
            alt="four people working on code"
            loading="lazy"
            class="image-3"
            width="600"
            height="400"
          />
        </aside>
      </section>
    </main>
  </body>
</html>
```
```ruby
*,
::before,
::after {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

body {
  font-family: 'Baskervville', serif;
  color: linen;
  background-color: rgb(20, 30, 40);
}

h1 {
  font-family: 'Anton', sans-serif;
}

h2, h3, h4, h5, h6 {
  font-family: 'Raleway', sans-serif;
}

a {
  text-decoration: none;
  color: linen;
}

main {
  display: grid;
  grid-template-columns: minmax(2rem, 1fr) minmax(min-content, 94rem) minmax(2rem, 1fr);
  row-gap: 3rem;
}

img {
  width: 100%;
  object-fit: cover;
}

hr {
  margin: 1.5rem 0;
  border: 1px solid rgba(120, 120, 120, 0.6);
}

.heading {
  grid-column: 2 / 3;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  row-gap: 1.5rem;
}

.text {
  grid-column: 2 / 3;
  font-size: 1.8rem;
  letter-spacing: 0.6px;
  column-width: 25rem;
  text-align: justify;
}

.hero {
  grid-column: 1 / -1;
  position: relative;
}

.hero-title {
  text-align: center;
  color: orangered;
  font-size: 8rem;
}

.hero-subtitle {
  font-size: 2.4rem;
  color: orangered;
  text-align: center;
}

.author {
  font-size: 2rem;
  font-family: "Raleway", sans-serif;
}

.author-name a:hover {
  background-color: #306203;
}

.publish-date {
  color: rgba(255, 255, 255, 0.5);
}

.social-icons {
  display: grid;
  font-size: 3rem;
  grid-template-columns: repeat(5, 1fr);
  grid-auto-flow: column;
  grid-auto-columns: 1fr;
  align-items: center;
}

.first-paragraph::first-letter {
  font-size: 6rem;
  color: orangered;
  float: left;
  margin-right: 1rem;
}

.quote {
  color: #00beef;
  font-size: 2.4rem;
  text-align: center;
  font-family: "Raleway", sans-serif;
}

.quote::before {
  content: '" ';
}

.quote::after {
  content: ' "';
}

.text-with-images {
  display: grid;
  grid-template-columns: 1fr 2fr;
  column-gap: 3rem;
  margin-bottom: 3rem;
}

.lists {
  list-style-type: none;
  margin-top: 2rem;
}

.lists li {
  margin-bottom: 1.5rem;
}

.list-title, .list-subtitle {
  color: #00beef;
}

.image-wrapper {
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: repeat(3, min-content);
  gap: 2rem;
  place-items: center;
}

.image-1, .image-3 {
  grid-column: 1 / -1;
}

@media only screen and (max-width: 720px) {
  .image-wrapper {
    grid-template-columns: 1fr;
  }
}

@media only screen and (max-width: 600px) {
  .text-with-images {
    grid-template-columns: 1fr;
  }
}

@media only screen and (max-width: 550px) {
  .hero-title {
    font-size: 6rem;
  }
  
  .hero-subtitle,
  .author,
  .quote,
  .list-title {
    font-size: 1.8rem;
  }
  
  .social-icons {
    font-size: 2rem;
  }

  .text {
    font-size: 1.6rem;
  } 
}

@media only screen and (max-width:420px){
  .hero-title{
    font-size:4.5rem;
  }
}
```
![Screenshot 2023-07-02 185012](https://github.com/huizi135/ALLAboutProgramming/assets/91324319/994fab11-64aa-4c65-879a-a857ee4d4503)
![Screenshot 2023-07-02 185140](https://github.com/huizi135/ALLAboutProgramming/assets/91324319/875ec002-b01f-4c3c-b1f4-9ed788676ca0)

<! DOCTYPE html>

<html lang=”en”>

<head>

<meta charset=”utf-8” >

<meta name=”viewport” content=”width=device-width, initial-scale=1.0”>

</head>

<body></body>

Now you can style the layout of your grid. CSS Grid is similar to Flexbox in that it has a special property for both the parent and child elements.

Use the `minmax` function to make your columns responsive on any device. The `minmax` function takes two arguments, the first being the minimum value and the second being the maximum. These values could be a length, percentage, `fr`, or even a keyword like `max-content`.

Your magazine will have three primary sections. You already set the overall layout in the `main` rule, but you can adjust the placement in the child rules.

One option is the `grid-column` property, which is shorthand for `grid-column-start` and `grid-column-end`. The `grid-column` property tells the grid item which grid line to start and end at.

Remember that the `grid-column` property determines which columns an element starts and ends at. There may be times where you are unsure of how many columns your grid will have, but you want an element to stop at the last column. To do this, you can use `-1` for the end column.

The CSS `repeat()` function is used to repeat a value, rather than writing it out manually, and is helpful for grid layouts. For example, setting the `grid-template-columns` property to `repeat(20, 200px)` would create 20 columns each `200px` wide.

The `object-fit` property tells the browser how to position the element within its container. In this case, `cover` will set the image to fill the container, cropping as needed to avoid changing the aspect ratio.

If you wanted to add more social icons, but keep them on the same row, you would need to update `grid-template-columns` to create additional columns. As an alternative, you can use the `grid-auto-flow` property.

This property takes either `row` or `column` as the first value, with an optional second value of `dense`. `grid-auto-flow` uses an auto-placement algorithm to adjust the grid layout. Setting it to `column` will tell the algorithm to create new columns for content as needed. The `dense` value allows the algorithm to backtrack and fill holes in the grid with smaller items, which can result in items appearing out of order.

Much like Flexbox, with CSS Grid you can align the content of grid items with `align-items` and `justify-items`. `align-items` will align child elements along the column axis, and `justify-items` will align child elements along the row axis.

Give the `.soci`

The `place-items` property can be used to set the `align-items` and `justify-items` values at the same time. The `place-items` property takes one or two values. If one value is provided, it is used for both the `align-items` and `justify-items` properties. If two values are provided, the first value is used for the `align-items` property and the second value is used for the `justify-items` property.

The `gap` property is a shorthand way to set the value of `column-gap` and `row-gap` at the same time. If given one value, it sets the `column-gap` and `row-gap` both to that value. If given two values, it sets the `row-gap` to the first value and the `column-gap` to the second.

