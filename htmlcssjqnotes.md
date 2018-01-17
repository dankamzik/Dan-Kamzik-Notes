Creating a comment:

```html
<!-- comment
Ending a comment:
content-->

Creating a style; changing text color:
<h2 style="color: blue">

Creating a style; changing text color with CSS (top of page)
  <style>
  h2 {color: red;}
  </style>

CSS class declaration:
  <style>
  .blue-text {
    color: blue;
  }
  </style>

Apply a class to an HTML element like this:
<h2 class="blue-text">CatPhotoApp</h2>

*remember that multiple elements can be declared as "blue-text"*

Importing fonts:
to import a font (say off of google) simply put the font's call to the top of the code page. Then you can call the name of the imported font later on in your code.

ADDING IMAGES TO YOUR WEBSITE
Add images to your website by using the img element, and point to a specific image's URL using the src attribute.
*All img elements must have an alt attribute*
Example:
<img src="https://www.your-image-source.com/your-image.jpg" alt="Author standing on a beach with two thumbs up. ">

SIZING AN IMAGE
*CSS has a property called width that controls an element's width. Just like with fonts, use px (pixels) to specify the image's width.*
For example, create a CSS class called "larger-image" that gives HTML elements a width of 500 pixels:
<style>
  .larger-image {
    width: 500px;
  }
</style>
*This is just like any other style code piece. However, if you are going to declare the picture a class name, then you must make sure that the code recognizes the picture as that class name by inputting a class="larger image" statement*

ADDING IN BORDERS
*CSS borders have properties like style, color and width*
Example:
<style>
  .thin-red-border {
    border-color: red;
    border-width: 5px;
    border-style: solid;
  }
</style>

*Remember that you can apply multiple classes to an element by separating each class with a space within its class attribute.*
Example:
<img class="class1 class2">

ADDING ROUNDED BORDERS WITH A BORDER RADIUS

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 10px;
  }

CREATING A CIRCLE BORDER
  *Begin as you would create any other border, then change the BORDER RADIUS to 50%. Forget about the pixels.*

LINKING TO EXTERNAL PAGES WITH ANCHOR ELEMENTS
*This adds in a URL to bring a user to another page, gallery, etc. You can specify what the clickable link will say as well.*
Example:
<p>Here's a <a href="http://freecodecamp.org"> link to Free Code Camp</a> for you to follow.</p>

NEST AN ANCHOR ELEMENT WITHIN A PARAGRAPH
*All you need to do here is create a <p> element around your existing <a> element. Everything that comes before the URL will be unclickable text, anything after it will be clickable text.*

MAKE DEAD LINKS USING THE HASH SYMBOL
Sometimes you want to add <a> elements to your website before you know where they will link.
This is also handy when you're changing the behavior of a link using jQuery.
Replace the value of your a element's href attribute with a #, also known as a hash symbol, to turn it into a dead link.
Example:
<p>Click here for <a href=#>cat photos</a></p>

MAKE AN IMAGE INTO A CLICKABLE LINK
Nest your image within an <a> element. Here's an example:
<a href="#"><img src="https://bit.ly/fcc-running-cats" alt="Three kittens running towards the camera."></a>

CREATE A BULLETED UNORDERED LIST
Drop an <ul> element into your code where you would put any <p> element, then specify the contents of that list with a <li> elent.
Unordered lists start with a <ul> element. Then they contain some number of <li> elements.
Example:
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>

CREATE AN ORDERED list
Ordered lists start with a <ol> element. Then they contain some number of <li> elements.
  Example:
  <ol>
    <li>Garfield</li>
    <li>Sylvester</li>
  </ol>

CREATE A TEXT FIELD
Text inputs are a convenient way to get input from your user.
Example:
<input type="text">
*Note that input elements are self-closing*

ADD PLACEHOLDER TEXT TO A TEXT FIELD
Example:
<input type="text" placeholder="this is placeholder text">

CREATE A FORM ELEMENT
You can build web forms that actually submit data to a server using nothing more than pure HTML. You can do this by specifying an action on your form element.
Example:
<form action="/url-where-you-want-to-submit-form-data"></form>
Nest your text field in a form element like this:
Example:
<form action="/submit-cat-photo">
<input type="text" placeholder="cat photo URL">
</form>

ADD A SUBMIT BUTTON TO THE FORM
Clicking this button will send the data from your form to the URL you specified with your form's action attribute.
Example submit button:
<button type="submit">this button submits the form</button>
Nest your button inside of your from for it to work:
Example:
<form action="/submit-cat-photo">
  <input type="text" placeholder="cat photo URL">
  <button type="submit">submit</button>
</form>

USE HTML5 TO REQUIRE A FIELD
You can require specific form fields so that your user will not be able to submit your form until he or she has filled them out.
If you wanted to make a text input field required, you can just add the word "required" within your input element.
Example:
<input type="text" required>

CREATE A SET OF RADIO BUTTONS:
You can use radio buttons for questions where you want the user to only give you one answer.
*Radio buttons are a type of input*
Each of your radio buttons should be nested within its own label element.
All related radio buttons should have the same name attribute.
Example:
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>

CREATE A SET OF CHECKBOXES
Forms commonly use checkboxes for questions that may have more than one answer.
Checkboxes are a type of input
Each of your checkboxes should be nested within its own label element.
All related checkbox inputs should have the same name attribute.
Creating a checkbox is much like creating a radio button.
Example:
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<label><input type="checkbox" name="personality"> Evil</label>

CHECK RADIO BUTTONS AND CHECKBOXES BY DEFAULT
You can set a checkbox or radio button to be checked by default using the checked attribute.
To do this, just add the word "checked" to the inside of an input element.
Example:
<input type="radio" name="test-name" checked>

NEST MANY ELEMNTS WITHIN A SINGLE DIV ELEMENT
The div element, also known as a division element, is a general purpose container for other elements.
The div element is probably the most commonly used HTML element of all. It's useful for passing the CSS of its own class declarations down to all the elements that it contains.
Just like any other non-self-closing element, you can open a div element with <div> and close it on another line with </div>.
Example:
<div>
<p>Things cats love:</p>
<ul>
  <li>cat nip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>
</div>

GIVE A BACKGROUND COLOR TO A DIV ELEMENT
You can set an element's background color with the background-color property.
If you wanted an element's background color to be green, you'd put this within your style element, and then name your <div> class the same:
    .green-background {
      background-color: green;
    }
Example:
*In style section*
.silver-background {
background-color: silver;
}
*In the beginning of your <div> section*
  <div class="silver-background">
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
</div>

SET THE ID OF AN ELEMENT
In addition to classes, each HTML element can also have an id attribute.
There are several benefits to using id attributes, and you'll learn more about them once you start using jQuery.
id attributes should be unique. Browsers won't enforce this, but it is a widely agreed upon best practice. So please don't give more than one element the same id attribute.
Here's an example of how you give your h2 element the id of cat-photo-app:
<h2 id="cat-photo-app">

USE AN ID ATTRIBUTE TO STYLE AN ELEMENT
One cool thing about id attributes is that, like classes, you can style them using CSS.
Here's an example of how you can take your element with the id attribute of cat-photo-element and give it the background color of green.
In your style element section, input:
#cat-photo-element {
  background-color: green;
}
*Note that inside your style element, you always reference classes by putting a . in front of their names. You always reference ids by putting a # in front of their names*
In the section you want to style, you add:
id="cat-photo-form"

ADJUSTING THE PADDING, MARGIN AND BORDER OF AN ELEMENT
In your style sheet, you can adjust whatever parameters you wish to for your boxes.
Example:
<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 10px;
  }

  .red-box {
    background-color: red;
    padding: 20px;
  }

  .green-box {
    background-color: green;
    padding: 20px;
  }
</style>

ADD A NEGATIVE MARGIN TO AN ELEMENT
An element's margin controls the amount of space between an element's border and surrounding elements.
If you set an element's margin to a negative value, the element will grow larger.
Example:
<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 10px;
  }

  .red-box {
    background-color: red;
    padding: 20px;
    margin: -15px;
  }

  .green-box {
    background-color: green;
    padding: 20px;
    margin: 20px;
  }
</style>

ADD DIFFERENT PADDING TO EACH SIDE OF AN ELEMENT
Sometimes you will want to customize an element so that it has different padding on each of its sides.
CSS allows you to control the padding of an element on all four sides with padding-top, padding-right, padding-bottom, and padding-left properties.
Example:

<style>
  .injected-text {
    margin-bottom: -25px;
    text-align: center;
  }

  .box {
    border-style: solid;
    border-color: black;
    border-width: 5px;
    text-align: center;
  }

  .yellow-box {
    background-color: yellow;
    padding: 10px;
  }

  .red-box {
    background-color: red;
    padding-top: 40px;
    padding-right: 20px;
    padding-bottom: 20px;
    padding-left: 40px;
  }

  .green-box {
    background-color: green;
    padding-top: 40px;
    padding-left: 40px;
    padding-bottom:20px;
    padding-right:20px;
  }
</style>
*It is important to note that the MARGIN and BORDER can be changed in the same way, using the MARGIN keyword and BORDER keyword*

USE CLOCKWISE NOTATION TO SPECIFY THE PADDING OF AN ELEMENT
Instead of specifying an element's padding-top, padding-right, padding-bottom, and padding-left properties, you can specify them all in one line, like this:
padding: 10px 20px 10px 20px;
These four values work like a clock: top, right, bottom, left, and will produce the exact same result as using the side-specific padding instructions.
*Note that this same clockwise notation can be used for MARGIN and BORDER as well*

STYLE THE HTML BODY ELEMENT
Every HTML page has a body element.
We can prove that the body element exists here by giving it a background-color of black.
We can do this by adding the following to our style element:
    body {
      background-color: black;
    }

INHERIT STYLES FROM THE BODY ELEMENT
You can style your body element just like any other HTML element, and all your other elements will inherit your body element's styles.
Example:
<style>
  body {
    color: green;
    font-family: Monospace; }

</style>
<h1>
  <p>Hello World!</p>
  </h1>
*The above code will display green- colored monospace font in your h1 paragraph*

PRIOITIZE ONE STYLE OVER ANOTHER
Sometimes your HTML elements will receive multiple styles that conflict with one another.
For example, your h1 element can't be both green and pink at the same time.
Example:
<style>
  body {
    background-color: black;
    font-family: Monospace;
    color: green;}
  .pink-text {color: pink;}
</style>
<h1 class=pink-text>Hello World!</h1>
*In the above code, the text will be displayed as pink, overruling the green class setting*

OVERRIDE STYLES IN SUBSEQUENT CSS
what can we do to override our pink-text class above?
Create an additional CSS class called blue-text that gives an element the color blue. Make sure it's below your pink-text class declaration.
The order of the class declarations in the "style" section are what is important. The second declaration will always take precedence over the first. Because .blue-text is declared second, it overrides the attributes of .pink-text
Example:

<style>
  body {
    background-color: black;
    font-family: Monospace;
    color: green;
  }
  .pink-text {
    color: pink;
  }
  .blue-text{
    color:blue;
  }
</style>
<h1 class="pink-text blue-text">Hello World!</h1>

OVVERRIDE CLASS DECLARATIONS BY STYLING ID ATTRIBUTES
Let's override your pink-text and blue-text classes, and make your h1 element orange, by giving the h1 element an id and then styling that id.
Example:

<style>
  body {
    background-color: black;
    font-family: Monospace;
    color: green;
  }
  .pink-text {
    color: pink;
  }
  .blue-text {
    color: blue;
  }
  #orange-text {
  color: orange;
}
</style>
<h1 class="pink-text blue-text" id="orange-text">Hello World!</h1>

OVERRIDE CLASS DECLARATIONS WITH INLINE STYLES:
There are other ways that you can override CSS. Do you remember inline styles?
Use an in-line style to try to make our h1 element white.
Example:
<style>
  body {
    background-color: black;
    font-family: Monospace;
    color: green;
  }
  #orange-text {
    color: orange;
  }
  .pink-text {
    color: pink;
  }
  .blue-text {
    color: blue;
  }
</style>
<h1 id="orange-text" class="pink-text blue-text" style="color: white">Hello World!</h1>

OVERRIDE ALL OTHER STYLES BY UNSING IMPORTANT
There's one last way to override CSS. This is the most powerful method of all. But before we do it, let's talk about why you would ever want to override CSS.
In many situations, you will use CSS libraries. These may accidentally override your own CSS. So when you absolutely need to be sure that an element has specific CSS, you can use !important
Example:
<style>
  body {
    background-color: black;
    font-family: Monospace;
    color: green;
  }
  #orange-text {
    color: orange;
  }
  .pink-text {
    color: pink !important;
  }
  .blue-text {
    color: blue;
  }
</style>
<h1 id="orange-text" class="pink-text blue-text" style="color: white">Hello World!</h1>
*!important was used in the pink class, overruling any other conflicting code*

USE HEX CODE FOR SPECIFIC COLORS
In CSS, we can use 6 hexadecimal digits to represent colors, two each for the red (R), green (G), and blue (B) components. For example, #000000 is black and is also the lowest possible value.
Example:
#000000
*this is black*
Example:

<style>
  body {
    background-color: #000000;
  }
</style>

Example:
<style>
  .red-text {
    color: #FF0000;
  }
  .green-text {
    color: #00FF00;
  }
  .dodger-blue-text {
    color: #2998E4;
  }
  .orange-text {
    color: #FFA500;
  }
</style>

<h1 class="red-text">I am red!</h1>

<h1 class="green-text">I am green!</h1>

<h1 class="dodger-blue-text">I am dodger blue!</h1>

<h1 class="orange-text">I am orange!</h1>

ABBREVIATED HEX CODES
Many people feel overwhelmed by the possibilities of more than 16 million colors. And it's difficult to remember hex code. Fortunately, you can shorten it.
For example, red's hex code #FF0000 can be shortened to #F00. This shortened form gives one digit for red, one digit for green, and one digit for blue.
This reduces the total number of possible colors to around 4,000. But browsers will interpret #FF0000 and #F00 as exactly the same color.
Example:
<style>
  .red-text {
    color: #F00;
  }
  .fuchsia-text {
    color: #F0F;
  }
  .cyan-text {
    color: #0FF;
  }
  .green-text {
    color: #0F0;
  }
</style>

<h1 class="red-text">I am red!</h1>

<h1 class="fuchsia-text">I am fuchsia!</h1>

<h1 class="cyan-text">I am cyan!</h1>

<h1 class="green-text">I am green!</h1>

USE RGB VALUES TO DETERMINE ELEMENT COLOR
Another way you can represent colors in CSS is by using RGB values.
The RGB value for black looks like this:
rgb(0, 0, 0)
The RGB value for white looks like this:
rgb(255, 255, 255)
Instead of using six hexadecimal digits like you do with hex code, with RGB you specify the brightness of each color with a number between 0 and 255.
Example:

<style>
  body {
    background-color: rgb(0, 0, 0);
  }
</style>

Example:

<style>
  .red-text {
    color: rgb(255, 0, 0);
  }
  .orchid-text {
    color: rgb(218, 112, 214);
  }
  .sienna-text {
    color: rgb(160, 82, 45);
  }
  .blue-text {
    color: 	rgb(0, 0, 255);
  }
</style>

<h1 class="red-text">I am red!</h1>

<h1 class="orchid-text">I am orchid!</h1>

<h1 class="sienna-text">I am sienna!</h1>

<h1 class="blue-text">I am blue!</h1>

USE RESPONSIVE DESIGN WITH BOOTSTRAP FLUID CONTAINERS
This time, we'll style it using the popular Bootstrap responsive CSS framework.
Bootstrap will figure out how wide your screen is and respond by resizing your HTML elements - hence the name Responsive Design.
With responsive design, there is no need to design a mobile version of your website. It will look good on devices with screens of any width.
You can add Bootstrap to any app by adding the following code to the top of your HTML:
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css"/>

MAKE IMAGES MOBILE RESPONSIVE
With Bootstrap, all we need to do is add the "img-responsive" class to your image. Do this, and the image should perfectly fit the width of your page.
Example:
<a href="#"><img class="img-responsive" src="https://bit.ly/fcc-running-cats" alt="Three running cats."></a>

CENTER TEXT WITH BOOTSTRAP
Bootstrap, we can center our heading element to make it look better. All we need to do is add the class text-center to our h2 element.
*Remember that you can add several classes to the same element by separating each of them with a space, like this:
<h2 class="red-text text-center">your text</h2>

CREATE A BOOTSTRAP BUTTON
Bootstrap has its own styles for button elements, which look much better than the plain HTML ones.
Example:
<button type="submit" class="btn">Like</button>

CREATE A BLOCK ELEMENT BOOTSTRAP BUTTON
Normally, your button elements with a class of btn are only as wide as the text that they contain.
By making them block elements with the additional class of btn-block, your button will stretch to fill your page's entire horizontal space and any elements following it will flow onto a "new line" below the block.
Example:
<button class="btn btn-block">Like</button>

COLORING BUTTONS IN BOOTSTRAP
Example:
<button class="btn-primary btn btn-block">Like</button>

CALL OUT OPTIONAL BUTTON ACTIONS WITH BUTTON INFO
The btn-info class is used to call attention to optional actions that the user can take.
Example:
<button class="btn btn-block btn-primary btn-info">Info</button>

WARN YOUR USERS OF A DANGEROUS ACTION
Bootstrap comes with several pre-defined colors for buttons. The btn-danger class is the button color you'll use to notify users that the button performs a destructive action.
Example:
<button class="btn btn-block btn-danger">Delete</button>

USE THE BOOTSTRAP GRID TO ALIGN ELEMENTS SIDE BY SIDE
Bootstrap uses a responsive grid system, which makes it easy to put elements into rows and specify each element's relative width. Most of Bootstrap's classes can be applied to a div element.
The col-md-* class is used. Here, md means medium, and * is a number specifying how many columns wide the element should be. In this case, the column width of an element on a medium-sized screen, such as a laptop, is being specified.
Example:
<div class="row">
  <div class="col-xs-4">
  <button class="btn btn-block btn-primary">Like</button>
</div>
 <div class="col-xs-4">
  <button class="btn btn-block btn-info">Info</button>
  </div>
  <div class="col-xs-4">
  <button class="btn btn-block btn-danger">Delete</button>
  </div>
</div>

DITCH CUSTOM CSS FOR BOOTSTRAP
We can clean up our code and make our Cat Photo App look more conventional by using Bootstrap's built-in styles instead of the custom styles we created earlier.
Don't worry - there will be plenty of time to customize our CSS later.
Basically, you just go down your markup and change out any CSS and replace it with bootstrap element names.

USE SPANS FOR INLINE ELEMENTS
You can use spans to create inline elements.
By using the span element, you can put several elements together, and even style different parts of the same element differently.
<p>Things cats <span class= "text-danger">love:</span></p>

CREATE A CUSTOM HEADING
Remember, Bootstrap uses a responsive grid system, which makes it easy to put elements into rows and specify each element's relative width. Most of Bootstrap's classes can be applied to a div element.
Below is an example of how to place your heading and first image in the same row.
Example:
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<div class="row">
  <div class="col-xs-8">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>
<div class="container-fluid">
  <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
</div>
  <div class="col-xs-4">
  <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back. "></a>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera. ">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>

  ADD FONT AWESOME ICONS TO OUR BUTTONS
  Font Awesome is a convenient library of icons. These icons are vector graphics, stored in the .svg file format. These icons are treated just like fonts. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.
  You can add Font Awesome to any app just by including it by adding the following code to the top of your HTML:
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css"/>
The i element was originally used to make other elements italic, but is now commonly used for icons. You add the Font Awesome classes to the i element to turn it into an icon, for example:
<i class="fa fa-info-circle"></i>
Below is an example of adding a fa thumbs up icon to the Like button in your code:
 <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i>Like</button>

 RESPONSIVELY STYLE RADIO BUTTONS
 You can use Bootstrap's col-xs-* classes on form elements, too! This way, our radio buttons will be evenly spread out across the page, regardless of how wide the screen resolution is.
 Example:
 <div class="row">
  <div class="col-xs-6"><label><input type="radio" name="indoor-outdoor"> Indoor</label></div>
  <div class="col-xs-6"><label><input type="radio" name="indoor-outdoor"> Outdoor</label></div>
  <div class="col-xs-6"><label><input type="checkbox" name="personality"> Loving</label></div>
  <div class="col-xs-6"><label><input type="checkbox" name="personality"> Lazy</label></div>
  <div class="col-xs-6"><label><input type="checkbox" name="personality"> Crazy</label></div>
</div>

STYLE TEXT INPUTS AS FORM CONTROL
You can add the fa-paper-plane Font Awesome icon by adding <i class="fa fa-paper-plane"></i> within your submit button element.
Example:
<form action="/submit-cat-photo">
  <div class="row">
    <div class="col-xs-6">
      <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    </div>
    <div class="col-xs-6">
      <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    </div>
  </div>
  <div class="row">
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Loving</label>
    </div>
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Lazy</label>
    </div>
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Crazy</label>
    </div>
  </div>
  <input class="form-control" type="text" placeholder="cat photo URL" required>
  <button class="btn btn-primary" type="submit"><i class="fa fa-paper-plane"></i>Submit</button>
</form>

LINE UP FORM ELEMENTS RESPONSIVELY WITH BOOTSTRAP
get your form input and your submission button on the same line. We'll do this the same way we have previously: by using a div element with the class row, and other div elements within it using the col-xs-* class.
<div class="row">
    <div class="col-xs-6">
      <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    </div>
    <div class="col-xs-6">
      <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    </div>
  </div>
  <div class="row">
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Loving</label>
    </div>
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Lazy</label>
    </div>
    <div class="col-xs-4">
      <label><input type="checkbox" name="personality"> Crazy</label>
    </div>
  </div>
  <div class="row">
    <div class="col-xs-7">
  <input type="text" class="form-control" placeholder="cat photo URL" required>
  </div>
  <div class="col-xs-5">
  <button type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button>
  </div>
</div>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

CREATING A BOOTSTRAP LAYOUT FROM SCRATCH

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


CREATE A BOOTSTRAP HEADLINE
Example:
<h3 class="text-primary text-center">jQuery Playground</h3>

HOUSE YOUR PAGE WITHIN A BOOTSTRAP CONTAINER FLUID DIV
Example:
<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
</div>

CREATE A BOOTSTRAP ROW
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
  </div>

</div>

SPLIT YOUR BOOTSTRAP ROW
Now that we have a Bootstrap Row, let's split it into two columns to house our elements.
Create two div elements within your row, both with the class col-xs-6.
Example:

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
    </div>
    <div class="col-xs-6">
    </div>
  </div>
</div>

CREATE BOOTSTRAP WELLS
Bootstrap has a class called "well" that can create a visual sense of depth for your columns.
Nest one div element with the class "well" within each of your col-xs-6 div elements.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
      </div>
    </div>
  </div>
</div>

ADD ELEMENTS WITHIN YOUR BOOTSTRAP WELLS
Now we're several div elements deep on each column of our row. This is as deep as we'll need to go. Now we can add our button elements.
Nest three button elements within each of your well div elements.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn"></button>
        <button class="btn"></button>
        <button class="btn"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn"></button>
        <button class="btn"></button>
        <button class="btn"></button>
      </div>
    </div>
  </div>
</div>

APPLY THE DEFAULT BOOTSTRAP BUTTON STYLE
Bootstrap has another button class called btn-default.
Apply both the btn and btn-default classes to each of your button elements.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
  </div>
</div>

CREATE A CLASS TO TARGET WITH JQUERY SELECTORS
Not every class needs to have corresponding CSS. Sometimes we create classes just for the purpose of selecting these elements more easily using jQuery.
Give each of your button elements the class target.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

ADD ID ATTRIBUTES TO BOOTSTRAP ELEMENTS
Recall that in addition to class attributes, you can give each of your elements an id attribute.
Each id must be unique to a specific element and used only once per page.
Let's give a unique id to each of our div elements of class well.
Remember that you can give an element an id like this:
<div class="well" id="center-well">
Give the well on the left the id of left-well. Give the well on the right the id of right-well.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

LABEL BOOTSTRAP WELLS
For the sake of clarity, let's label both of our wells with their ids.
Above your left-well, inside its col-xs-6 div element, add a h4 element with the text #left-well.
Above your right-well, inside its col-xs-6 div element, add a h4 element with the text #right-well.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6"><h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6"><h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

GIVE EACH ELEMENT A UNIQUE ID
We will also want to be able to use jQuery to target each button by its unique id.
Give each of your buttons a unique id, starting with target1 and ending with target6.
Make sure that target1 to target3 are in #left-well, and target4 to target6 are in #right-well.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button id="target1" class="btn btn-default target"></button>
        <button id="target2" class="btn btn-default target"></button>
        <button id="target3" class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button id="target4" class="btn btn-default target"></button>
        <button id="target5" class="btn btn-default target"></button>
        <button id="target6" class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>

LABEL BOOTSTRAP BUTTONS
Just like we labeled our wells, we want to label our buttons.
Give each of your button elements text that corresponds to its id's selector.
Example:
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

USE COMMENTS TO CLARIFY CODE
When we start using jQuery, we will modify HTML elements without needing to actually change them in HTML.
Let's make sure that everyone knows they shouldn't actually modify any of this code directly.
Remember that you can start a comment with <!-- and end a comment with -->
Example:
<!--only chnage code above this line-->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

LEARN HOW SCRIPT TAGS AND DOCUMENT READY WORK
Before we can start using jQuery, we need to add some things to our HTML.
First, add a script element at the top of your page. Be sure to close it on the following line.
Your browser will run any JavaScript inside a script element, including jQuery.
Inside your script element, add this code: $(document).ready(function() { to your script. Then close it on the following line (still inside your script element) with: });
We'll learn more about functions later. The important thing to know is that code you put inside this function will run as soon as your browser has loaded your page.
This is important because without your document ready function, your code may run before your HTML is rendered, which would cause bugs.
Example:
<script>$(document).ready(function() {});</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET HTML ELEMENTS WITH JQUERY USING SELECTORS
Now we have a document ready function.
Now let's write our first jQuery statement. All jQuery functions start with a $, usually referred to as a dollar sign operator, or as bling.
jQuery often selects an HTML element with a selector, then does something to that element.
For example, let's make all of your button elements bounce. Just add this code inside your document ready function:
$("button").addClass("animated bounce");
Note that we've already included both the jQuery library and the Animate.css library in the background so that you can use them in the editor. So you are using jQuery to apply the Animate.css bounce class to your button elements.
Example:

<script>
  $(document).ready(function() {$("button").addClass("animated bounce");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET ELEMENTS BY CLASS USING JQUERY
You see how we made all of your button elements bounce? We selected them with $("button"), then we added some CSS classes to them with .addClass("animated bounce");.
You just used jQuery's .addClass() function, which allows you to add classes to elements.
First, let's target your div elements with the class well by using the $(".well") selector.
Note that, just like with CSS declarations, you type a . before the class's name.
Then use jQuery's .addClass() function to add the classes animated and shake.
For example, you could make all the elements with the class text-primary shake by adding the following to your document ready function:
$(".text-primary").addClass("animated shake");
Example:

<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce"); $(".well").addClass("animated shake");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET ELEMENTS BY ID USING JQUERY
You can also target elements by their id attributes.
First target your button element with the id target3 by using the $("#target3") selector.
Note that, just like with CSS declarations, you type a # before the id's name.
Then use jQuery's .addClass() function to add the classes animated and fadeOut.
Example:
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut")
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

DELETE YOUR JQUERY FUNCTIONS
Delete all three of these jQuery functions from your document ready function, but leave your document ready function itself intact.
Example:
<script>
  $(document).ready(function() {
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET THE SAME ELEMENT WITH JQUERY SELECTORS
Now you know three ways of targeting elements: by type: $("button"), by class: $(".btn"), and by id $("#target1").
Although it is possible to add multiple classes in a single .addClass() call, let's add them to the same element in three separate ways.
Using .addClass(), add only one class at a time to the same element, three different ways:
Add the animated class to all elements with type button.
Add the shake class to all the buttons with class .btn.
Add the btn-primary class to the button with id #target1.
*Note* You should only be targeting one element and adding only one class at a time. Altogether, your three individual selectors will end up adding the three classes shake, animated, and btn-primary to #target1.
Example:
<script>
  $(document).ready(function() {$("button") .addClass("animated"); $(".btn") .addClass("shake"); $("#target1") .addClass("btn-primary");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

REMOVE CLASSES FROMAN ELEMENT USING JQUERY
In the same way you can add classes to an element with jQuery's addClass() function, you can remove them with jQuery's removeClass() function.
Here's how you would do this for a specific button:
$("#target2").removeClass("btn-default");
Let's remove the btn-default class from all of our button elements.
Example:
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut");
    $("#target1").removeClass("btn-default");
    $("#target2").removeClass("btn-default");
    $("#target3").removeClass("btn-default");
    $("#target4").removeClass("btn-default");
    $("#target5").removeClass("btn-default");
    $("#target6").removeClass("btn-default");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

CHANGE THE CSS OF AN ELEMENT USING JQUERY
We can also change the CSS of an HTML element directly with jQuery.
jQuery has a function called .css() that allows you to change the CSS of an element.
Here's how we would change its color to blue:
$("#target1").css("color", "blue");
This is slightly different from a normal CSS declaration, because the CSS property and its value are in quotes, and separated with a comma instead of a colon.
Example:
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut");
    $("button").removeClass("btn-default");
    $("#target1").css("color", "red");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

DISABLE AN ELEMENT USING JQUERY
You can also change the non-CSS properties of HTML elements with jQuery. For example, you can disable buttons.
When you disable a button, it will become grayed-out and can no longer be clicked.
jQuery has a function called .prop() that allows you to adjust the properties of elements.
Here's how you would disable all buttons:
$("button").prop("disabled", true);
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

CHANGE TEXT INSIDE AN ELEMENT USING JQUERY
Using jQuery, you can change the text between the start and end tags of an element. You can even change HTML markup.
jQuery has a function called .html() that lets you add HTML tags and text within an element. Any content previously within the element will be completely replaced with the content you provide using this function.
Here's how you would rewrite and emphasize the text of our heading:
$("h3").html("<em>jQuery Playground</em>");
jQuery also has a similar function called .text() that only alters text without adding tags. In other words, this function will not evaluate any HTML tags passed to it, but will instead treat it as the text you want to replace the existing content with.
Change the button with id target4 by emphasizing its text.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target4").html("<em>#target4</em>");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

REMOVE AN ELEMENT USING JQUERY
jQuery has a function called .remove() that will remove an HTML element entirely
Remove element target4 from the page by using the .remove() function.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

USE appendTo TO MOVE ELEMENTS WITH JQUERY
Let's try moving elements from one div to another.
jQuery has a function called appendTo() that allows you to select HTML elements and append them to another element.
For example, if we wanted to move target4 from our right well to our left well, we would use:
$("#target4").appendTo("#left-well");
Move your target2 element from your left-well to your right-well.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

CLONE AN ELEMENT USING JQUERY
In addition to moving elements, you can also copy them from one place to another.
jQuery has a function called .clone() that makes a copy of an element.
For example, if we wanted to copy target2 from our left-well to our right-well, we would use:
$("#target2").clone().appendTo("#right-well");
This involves sticking two jQuery functions together. This is called "function chaining" and it's a convenient way to get things done with jQuery.
Clone your target5 element and append it to your left-well.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET THE PARENT OF AN ELEMENT USING JQUERY
Every HTML element has a parent element from which it inherits properties.
For example, your jQuery Playground h3 element has the parent element of <div class="container-fluid">, which itself has the parent "body".
jQuery has a function called parent() that allows you to access the parent of whichever element you've selected.
Here's an example of how you would use the parent() function if you wanted to give the parent element of the left-well element a background color of blue:
$("#left-well").parent().css("background-color", "blue")
Give the parent of the #target1 element a background-color of red.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red")
  });
</script>
<!-- Only change code above this line. -->
<body>
  <div class="container-fluid">
    <h3 class="text-primary text-center">jQuery Playground</h3>
    <div class="row">
      <div class="col-xs-6">
        <h4>#left-well</h4>
        <div class="well" id="left-well">
          <button class="btn btn-default target" id="target1">#target1</button>
          <button class="btn btn-default target" id="target2">#target2</button>
          <button class="btn btn-default target" id="target3">#target3</button>
        </div>
      </div>
      <div class="col-xs-6">
        <h4>#right-well</h4>
        <div class="well" id="right-well">
          <button class="btn btn-default target" id="target4">#target4</button>
          <button class="btn btn-default target" id="target5">#target5</button>
          <button class="btn btn-default target" id="target6">#target6</button>
        </div>
      </div>
    </div>
  </div>
</body>

TARGET THE CHILDREN OF AN ELEMENT USING JQUERY
Many HTML elements have children which inherit their properties from their parent HTML elements.
For example, every HTML element is a child of your body element, and your "jQuery Playground" h3 element is a child of your <div class="container-fluid"> element.
jQuery has a function called children() that allows you to access the children of whichever element you've selected.
Here's an example of how you would use the children() function to give the children of your left-well element the color of blue:
$("#left-well").children().css("color", "blue")
Give all the children of your #right-well element a color of orange.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange")
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET A SPECIFIC CHILD OF AN ELEMENT USING JQUERY
jQuery uses CSS Selectors to target elements. "target:nth-child(n)"" css selector allows you to select all the nth elements with the target class or element type.
Here's how you would give the third element in each well the bounce class:
$(".target:nth-child(3)").addClass("animated bounce");
Make the second child in each of your well elements bounce. You must target the children of element with the target class.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $(".target:nth-child(2)").addClass("animated bounce");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

TARGET EVEN/ODD NUMBERED ELEMENTS USING JQUERY
You can also target all the even-numbered elements.
Here's how you would target all the odd-numbered elements with class target and give them classes:
$(".target:odd").addClass("animated shake");
***Note that jQuery is zero-indexed, meaning that :odd selects the second element, fourth element, and so on. You begin counting from ZERO.***
Try selecting all the even-numbered elements and giving them the classes of animated and shake.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $("#left-well").children().css("color", "green");
    $(".target:nth-child(2)").addClass("animated bounce");
    $(".target:even").addClass("animated shake");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

USE JQUERY TO MODIFY THE ENTIRE PAGE
Time to tear shit down.
jQuery can target the "body" element as well.
Here's how we would make the entire body fade out:
$("body").addClass("animated fadeOut");
But let's do something more dramatic. Add the classes animated and hinge to your body element.
Example:
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $("#left-well").children().css("color", "green");
    $(".target:nth-child(2)").addClass("animated bounce");
    $(".target:even").addClass("animated shake");
    $("body").addClass("animated hinge");
  });
</script>
<!-- Only change code above this line. -->
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

WHAT IS A CSS PREPROCESSOR?
A preprocessor is a program that takes one type of data and converts it to another type of data. In the case of HTML and CSS, some of the more popular preprocessor languages include Haml and Sass . Haml is processed into HTML and Sass is processed into CSS.


```
