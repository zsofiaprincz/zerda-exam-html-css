# Exam: HTML & CSS

### Getting Started
 - Fork this repository under your own account
 - Commit your progress frequently and with descriptive commit messages
 - All your answers and solutions should go in this repository

### What can I use?
 - You can use any resource online, but **please work individually**
 - Instead of copy-pasting your answers and solutions, write them in your own words.


# Tasks

## 1. Build a design (~90 minutes) [10 points]
Build the following profile cards according to the design provided.   
Follow the design as closely as possible.   
Commit an HTML and a CSS file to this repository.
![design](exercise-1.png)

### Assets
John Duck | Jane Duck | Pencil icon
--------- | --------- | -----------
![duck](duck.jpg) | ![duck](duck2.jpg) | ![pencil-icon](edit-icon.png)   

### Other data
  - Name font size: 28 pixels
  - Text size: 14 pixels
  - Font family: Arial, sans-serif

### Acceptance criteria
The task is accepted if:
  - The result follows design [2p]
  - The code follows style guide [1p]
  - The CSS & HTML are valid [1p]
  - The HTML considers semantic responsibilities [2p]
  - The code avoids code duplication [2p]
  - The CSS has meaningful and short selectors [2p]

Extra points for if:
  - the result is centered on the page [2p]


## 2. Understand code (~15 minutes) [2 points]
Read the following code snippet:   
What is the distance between the top-left corner of the document body and the yellow box? <br>  <em> top 40px , left 40px </em> <br>
Give a detailed explanation below!  <br> <em>The position of the blue box is absolute which means its child element (defined on the bottom by divs) is positionned absolutely anywhere relative to its parent. The parent element is 20-20 from top left and by positionning the yellow box 20-20 also top left, we define the 20 pixels from the corner of the blue box.</em><br>
Add your answer to this readme file, commit your changes to this repository.
```HTML
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        padding: 0px;
        margin: 0px;
      }
      .foo {
        top: 20px;
        left: 20px;
        width: 100px;
        height: 100px;
        position: absolute;
        background: blue;
      }
      .bar {
        top: 20px;
        left: 20px;
        width: 30px;
        height: 30px;
        position: absolute;
        background: yellow;
      }
    </style>
  </head>
  <body>
    <div class="foo">
      <div class="bar"></div>
    </div>
  </body>
</html>
```
#### Your answer: [2p]


## 3. Explain concepts (~15 minutes) [4 points]
Add your answer to this readme file, commit your changes to this repository.


### Explain the difference between `display: block` and `display: inline` in CSS! What is `display: inline-block`?
#### Your answer: [2p]

### display:block <em>It means the element takes the whole space from left to right in the document flow, it speads out horizontally as far as it can. In more colloquial terms it 'blocks'a whole line in the vertical document flow. By default block level elements are div, p, h1-h6 etc...</em>

### display:inline <em> Inline is the opposite of block in a sense that the element does not take more horizontal space then its element size. Inline lements are placed next to each other in a line. Padding and margin can only be applied vertically, top or bottom padding or margin cannot be applied. The most popular inline elemnts are a, span etc..</em>

### display:inline-block <em> Similar to inline except that we can add top and bottom margins and padding to it, so the element will have effect on the horizontal size of the page.Or the other way around: similar to block except that it sits in the line.</em>



### What is the difference between a `<section>` and an `<article>` element? Name one good example of using an `<article>`.
#### Your answer: [2p]

### section <em> Section tag is used to mark a seperate part in html e.g chapter</em>

#### article <em> Article is a self-contained tag that stands alone in the site and intended to be redistributable. Blog entries, magazine articles are typical article tags. 

