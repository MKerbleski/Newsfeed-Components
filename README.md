# Newsfeed-Components

In this project we are going to be building a news feed reader. The goal is to have a collapsing menu, and expandable news articles. The HTML and CSS is already done for you, you simply need to connect the pieces. After the CSS is connected it is time to move on to building out our components using Javascript. We will be adding common functionality and styling to build reusable components.

### Need to know:
* CSS:
  * import
* Javascript:
  * ES6 classes and the constructor function.
		
### Setup
  * Run `less-watch-compiler` from the top level of the Newsfeed-Components folder. 
  * Open index.html in your browser

### Part 1: The Menu

* Import menu.less from the correct path into index.less (follow the lead for header if you’re not sure how to write the correct path)
* Select the menu and menu button elements from the HTML. Look at the HTML code to determine the class names of both.
* Write a callback function that adds and removes a class to the menu when called. Hint: Look in the Menu.less file for the name of the class. 
* Look at the LESS and determine what Is happening when the classes are added or removed. Pass the callback to a click event listener on the button.


### Part 2: The Articles

* Make sure the Article LESS rules are being applied to the page.
* Look over the LESS to see what is happening, but don’t change anything yet.
* USelect all articles. Map over the array creating individual instances of the Article class.
* Within the Article class, set properties for the element, and expandButton.
* Add text to the expand button reading: ‘Click to Expand’
* Add a click event to the expand button (or entire article if you need to at first), pass the click event the ‘expandArticle’ method.
* Within the expand article method add or remove the open class from the article. (Check the LESS for the correct class name)

### Part 3: Add Articles

* Now that we have our components built, add a few articles of your own to the HTML. Notice how our javascript code automatically selects the new articles and adds the styling and functionality we just built to them. This is the power of components. Write the code once and add as many components as you want all while maintaining the functionality we built!

### Stretch Goals:

If you complete the main goals of the page let's play around with some cool animation libraries

A few things to check out: 
* Native CSS Animations. 
  * CSS has the ability to animate elements using a number of different properties. Check out `transform` and `transition`, and `animate`. A word of warning, these CSS properties will act differently on different browsers, so always read and see if you need a `browser prefix` in order to animate properly. 
  * https://css-tricks.com/almanac/properties/a/animation/
* jQuery
  * jQuery is an extrememly popular javascript library, in fact most of the native DOM manipulation we know and love, came from the jQuery library. It is worth getting a little familiar with it. The jQuery library is massive, and part of it is an animation library. jQuery gives us a fantastic method called `.animate()`. There are also simpler methods such as `slideDown` `slideUp`, `slideToggle`, `show`, `hide` and more.
  * http://www.jquery.com
* GSAP
  * Greensock Animation Platform, is by far the most powerful of the three. It is intuitive and easy to use, and you will be amazed at the results.
  * https://greensock.com/gsap

Note: Just a reminder the stretch goals are just extra practice using the tools we have learned. These are not required. Only parts 1-3 are required portions of the project. If you do not get to the stretch goals, don't worry.

* Animation: There are many ways to animate elements on the screen corresponding to user interactions.  Read the documentation of the animation platform of your choise. Animate all of the components on click.
  * Animation Goal #1. Animate the menu opening: You will need to change the CSS for the menu in order to acheive this. Get the menu to slide in from the left side of the screen. And slide out when the button is clicked. Bonus: Get the menu to slide back out when the user clicks anywhere on the screen other than the menu. 
  * Animation Goal #2 Animate the article opening. This one is a bit trickier. You will need to change the CSS for this component as well. Animate the component so that it slides open and slides closed on each click. Update the text in the expand button to read `'Click to Expand'` or `'Click to Close'` depending on the state of the article. 

* Close Button

  Add a close (or 'read') button to each Article component. When clicked the article will dissapear.

* Component Constructor
  
  Create a function that builds Article components. You are not expected to finish this. This goal is simply an exercise in thinking about how you would implement a function that took some data, created a new Article from it, and appended it to the HTML (without actually writing anything in the HTML file). This is a difficult concept to undertake, but even thinking about how you would implement it will give you a better understanding of how we use frameworks in upcoming sprints. 

* Implement a way to write your own articles using the Component Constructor and some input fields. 