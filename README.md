# Session 2 - CSS
### _CSS Recap_
CSS (Cascading Style Sheet) adds styling to your html structure.
Styles can be applied in a number of ways, however they all follow `property: value` pattern.

Each property: value pair must end with a semicolon (;).

### _Applying CSS_
There are three ways CSS can be written: inline styling, internal and external style sheets.

##### _Inline_:
Inline styling is applied directly to the element by using the `style` property e.g. `<div style="color: red;"></div>`.

##### _Internal Style Sheet_:
Internal style sheets are initialised in the `<style></style>` tags within the document's <head>. Internal style sheets allow for better readability as the CSS can be broken into lines: 
`<head>
	<style>
		h1 {
			color: red;
		}
	</style>
</head>`

With this method, entire elements (h1, h2, div) can be selected and have styles applied to them. It is also possible to create your own custom classes and Ids (I'll come back to these in a bit) for a fuly customised webpage.

_Note_:

With html5 the `<style></style>` tags have a `scoped` attribute which allows styles such as media queries to be applied 'inline'- however this is only currently supported in Firefox.

##### _External Style Sheet_:
The final way (and the way you should probably be using the most) is by using an external CSS file which is then linked to the html document.
Just like with the internal style sheet, whole elements and custom classes / Ids are selectable.

To select the appropriate CSS file, you must know the file location and the path to the file either from the current html file or from the root (main) folder of the website.

##### _Absolute Links_:
An absolute link notes the full path from the root folder.
In my case, if I wanted to link the CSS file 'exercise1.css' by an absolute path, I would use `D:/Work/GitHub/CFG-Instructor-Example/css/exercise1.css`. Starting at my D drive, the file path works it's way up to the CSS file in a logical progression. This is equivalent to putting in a website's URL and following the file path along until the CSS file is reached.


##### _Relative Links_:
There are two types of links: root-relative and document-relative.

A root relative link starts at the ultimate root of the file structure. Taking the same example as before, I could link to exercise1.css with `/Work/GitHub/CFG-Instructor-Example/css/exercise1.css`.

On the other hand, document relative links (they're really directory relative links) start from the current document (directory) and as such, need a little more thinking about as most of the time, the progression is not going to be linear. For example, if I once again link to exercise1.css (but this time using a document relative link) I would get: `../css/exercise1.css`. To me, this is a lot more pleasing to the eye. While this may look  complicated at first, the only 'special' thing here are the two dots (..) at the beginning. `..` indicates that the current directory needs to be moved up by one. From there, the current directory then 'selects# the CSS folder and then the file within it. The full process (using absolute paths) might look something like this:

		1. D:/Work/GitHub/CFG-Instructor-Example/html
		2. D:/Work/GitHub/CFG-Instructor-Example/
		3. D:/Work/GitHub/CFG-Instructor-Example/css
		4. D:/Work/GitHub/CFG-Instructor-Example/css/exercise1.css


Finally, you might be wondering how you would access another file in the same directory. This is simply achieved by typing out the file name. For instance, if I wanted to access exercise2.html from exercise1.html I would write `href="exercise2.html"`. The same behaviour can also be achieved by writing `href="./exercise2.html"`. In this case the dot (.) points to the same directory and the slash (/) gives access to it. While it is not necessary to write it like this, you will probably come across it at some point - for me, the dot slash notation just allows me to see where I'm starting from more easily.

In short:

1. .  = This location
2. .. = Up a directory

_Note_:
It is entirely valid to combine relative path 'dot' notation if you so wish. For example: `./../css/exercise1.css`.

### _Classes vs Ids_
As covered in week 1, CSS classes are created in the stylesheets by a leading dot (.). Similarly, Ids are created with a leading hash (#).

The main difference between class and id selectors is that an id can only be used _once_ per page (it needs to be unique) while a class can be used multiple times.

The main difference for me is that ids allowed user to be instantly scrolled to a specific part of the page.

### _Note_
During the lesson, a few of you asked what the point of the `type="text/css"` actually does in the link tag. 


# Homework
This exercise is an extension of the work set in Week 1. The premise of it once again asks you to modify some given content so that it looks like the solution image. The main purpose of this exercise is to show off some the various CSS selectors you can use (for a full list of CSS selectors please find the reference material [here](https://www.w3schools.com/cssref/css_selectors.asp "CSS Selectors")).

Your CSS may or may not look completely different to the one I have provided - this doesn't matter in the slightest as long as the page looks the same. As you will learn, there is no real incorrect way of writing CSS. As you get better you will simply find ways of styling elements more efficiently and with greater ease. 

_Final Note_:

When looking at the example solutions, you might notice that the `html`, `head` and `body` tags are all aligned on the same line. This is due to the way my text editor auto-indents and is the general accepted way of indentation. If you'd like to read up on why this is the case Scott Granneman provides a thorough but concise explanation [here](https://www.granneman.com/webdev/coding/formatting-and-indenting-your-html/#what-about-the-basic-structure "HTML Indentation")

Both of the next two CSS selectors do exactly the same thing,
however the former is using a specific CSS selector property while the 
latter uses a class assigned in the html.

Just remember that there are multiple ways to achieve the same thing - a list of all the CSS selectors can be found [here](https://www.w3schools.com/cssref/css_selectors.asp "CSS Selectors")
