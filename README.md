# Bootstrap4Demo
This repo is part of the lectures on Software Engineering at the DHBW Karlsruhe.

## Cheat Sheet 
During the e-Portfolio, we created a Cheat-Sheet you can find as CheatSheetClass.html.
To have a fully documented Cheat-Sheet, I can recomened the following pages:
* [hackerthemes.com](https://hackerthemes.com/bootstrap-cheatsheet/)
* [officiall Bootstrap Docu](http://getbootstrap.com/docs/4.0/components/alerts/)

## Presentation
To get a brief overview of Bootstrap 4, find the presentation attached to the repo.

## Tutorial
1. First things first: Clone this Repo or copy the StarterTemplate.html. This Template is just an basic HTML5 Page, with Bootstrap CSS and JS included via CDN.
2. The most important Bootstrap Class is the `container`. So just start by adding a div with the class of conatiner.
3. Inside this div. make another one with the class of `page-header`. Inside this div, put a h1. By now, you body should look like this:
```html
<div class="container">
  <div class="page-header">
    <h1>Hello</h1>
  </div>
</div>
  ```
4. It's easy to align and float text in Bootstrap. Therefore, you can use the classes of `text-left`, `text-center` and `text-right`. You can applie them like this:
```html
 <p class="text-left">Im left</p>
      <p class="text-right">im right</p>
      <p class="text-center">im in the center</p>
      <hr>
      <div class="float-md-left">Left</div>
      <div class="float-md-right">right</div>
      <div class="clearfix"></div>
      
 ```
 By now, your Website should look like this:
 
 
 ![alt text](https://github.com/Toaster996/Bootstrap4Demo/blob/master/pictures/align.PNG "Align Text")
 
 
5. The unique thing about Bootstrap is the Bootstrap Grid System. In the presentation, you'll find further details, but simply said, it looks at a Website as a 12-col Grid. With the class of `row`, you can start this grid.
```html
<div class="row">
        <div class="col-md-8">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam provident in maiores saepe soluta iusto molestias illum reprehenderit, odio minus?</div>
        <div class="col-md-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi accusantium qui doloribus natus deserunt ipsa esse amet eum saepe blanditiis.</div>
        <div class="col-md-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi accusantium qui doloribus natus deserunt ipsa esse amet eum saepe blanditiis.</div>
      </div>
```
This is an example of the Grid System. The Website is devided in one large 8-col part and two samller 2-col parts. You can devide them the way you want.

6. To create a Navbar, just grab the content from the navbar.html and put it at the top of your page-body. This is a navbar, that collapses, when you screen-size is less than medium. Then, you get the iconic Hamburger-button. It's easy to modify this navbar the way you want it to be. For example, you can add the class `navbar-dark` and change the backgroudcolorclass to `bg-dark` as well as `bg-primary`. You can use all Bootstrap colors introduced in the presentation or custon CSS-Colors. `fixed-top` and `fixed-botton` will possition the navbar fixed at the bottom or top.

7. A common Bootstrap-object is the `jumbotron`. Gues what, you need the class of `jumbotron` for a div. You can use jumbotron inside and outside of containers, i recomend to use it outside at the top, right under the navbar.
An example Jumbotron could look like this:
```html
<div class="jumbotron">
          <div class="container">
            <h1>
              Welcome to my Website!
            </h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti, debitis.</p>
          </div>
        </div>
```

Your Jumbotron in the End should lokk similar to this:
 
 ![alt text](https://github.com/Toaster996/Bootstrap4Demo/blob/master/pictures/jumbotron.PNG "Jumbotron")

8. In todays Webistes, Buttons are really important. Therefore, Bootstrap has a bunch of Buttonclasses. The basic Buttonclass is `btn`, but you can modyfiy it using `btn-primary` or `btn-secondary`. Bootstrap4 introduced the outline-buttons. You can use them in the same way, `btn-outline-primary`. 
Examples would look like this
```html
<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-primary">Primary</button>

<!-- Secondary, outline button -->
<button type="button" class="btn btn-secondary">Secondary</button>

<!-- Indicates a successful or positive action -->
<button type="button" class="btn btn-success">Success</button>

<!-- Contextual button for informational alert messages -->
<button type="button" class="btn btn-info">Info</button>

<!-- Indicates caution should be taken with this action -->
<button type="button" class="btn btn-warning">Warning</button>

<!-- Indicates a dangerous or potentially negative action -->
<button type="button" class="btn btn-danger">Danger</button>

<!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
<button type="button" class="btn btn-link">Link</button>

<button type="button" class="btn btn-outline-primary">Primary</button>
<button type="button" class="btn btn-outline-secondary">Secondary</button>
<button type="button" class="btn btn-outline-success">Success</button>
<button type="button" class="btn btn-outline-info">Info</button>
<button type="button" class="btn btn-outline-warning">Warning</button>
<button type="button" class="btn btn-outline-danger">Danger</button>
```

9. Another important element is the page-footer. Therefore, we use the tag `<footer class="footer bg-dark">` with the class of footer. We can also use the bg-class just like in every other element, to change the background-color. 
Inside this footer, we need several divs. To make the footer, we need the container and a grid system with only one columm. The `text-center` class is the one you already used to align text. 
```html
 <footer class="footer bg-dark mt-3">
      <div class="container">
        <div class="row">
          <div class="col text-center text-light p-4">
            Contact Us!
          </div>
        </div>
      </div>
    </footer>
```
You footer should look like this:
 
 ![alt text](https://github.com/Toaster996/Bootstrap4Demo/blob/master/pictures/footer.PNG "Footer")
 
One interesting point in this footer are the classes `p-4` and `mt-3`. Those are new Bootstrap4 Classes. To mave a padding or margin around an element, you can just wirte `p-[1-5]` vor padding and `m-[1-5]` for margin. You might also need the ability to only add paddings or margins add the top, right, bootom or left. Therefore, you can use classes like `mt-3`, which adds a margin of 3 at the top.

