Download Link: https://assignmentchef.com/product/solved-cinf362-week-5-css-part-ii
<br>
<strong>Agenda</strong>

<ul>

 <li>More Fun With CSS

  <ul>

   <li>Box Model</li>

   <li>Positioning with CSS</li>

   <li>CSS Positioning Exercises</li>

   <li>CSS Evaluation Initial Post &amp; Response</li>

  </ul></li>

 <li>Next Week</li>

</ul>




<h2>More Fun With CSS</h2>

<strong>Box Model</strong>

Every element in HTML can be considered as a box. Each of these boxes takes up a certain amount of space on our page relative to the other boxes. Also, the spacing inside of these boxes can vary depending on the content inside of them. The box model in CSS is a way to understand how HTML is laid out and uses certain properties to help achieve this goal. It is comprised of <strong>three</strong> main properties. The properties are padding, border, and margin which all impact how elements are spaced out on a page:

The <u>padding</u> property handles the space between the content and the border around that content.

The <u>border</u> property handles borders which wraps around the padding and content.

The <u>margin</u> property handles space outside of the border and wraps up the border, padding, and content.

In the image above, I have used Google Chrome’s “Inspect Element” feature (F12 or right-click and select it) to view the HTML/CSS in a page. On the left side of the inspector, the HTML structure is viewable. On the right side, there is a multi-colored box which depicts the CSS box model in action. The orange area represents the margin (16px default for paragraphs in Chrome). The border is depicted by the yellow area. Lastly, the green area is the padding which separates the content from the border. The links below cover the CSS Box Model in greater detail and explain things like inline vs block level elements as well. The CSS slides on Blackboard also provide a quick glimpse into these topics and should be reviewed.

<u>Additional Reading</u>

<ul>

 <li><a href="https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model">https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model</a></li>

 <li><a href="https://css-tricks.com/the-css-box-model/">https://css-tricks.com/the-css-box-model/</a></li>

</ul>

<strong>Positioning with CSS</strong>

There are numerous ways to position HTML elements using CSS. Position, float, flexbox, grid, and other properties allow us to place our elements, but each one has its strengths and weaknesses. I will explain the position and float properties and provide links to some of the other ones as well. For this course, most of you will probably use the float property since position is harder to implement for a site with more content. Flexbox and grid are also great methods and were more recently implemented in the CSS specs. They can accomplish more things but can be complicated in some instances.

<u>Float Property</u>

This property takes content and aligns it to either the left or right side of a container. The content is removed from the normal document flow, but text content and inline elements will wrap around it. Block level elements will appear on the next available line. To prevent unwanted wrapping of content, you would have to clear your floats. This means you use the clear property on the element which wraps your floated elements. There are many methods to clear floats but the best one I have found is here: <a href="https://css-tricks.com/snippets/css/clear-fix/">https://css-tricks.com/snippets/css/clear-fix/</a>

To use the clear fix in the link above, you need to wrap all floated elements in a parent container (div usually). Then you target that parent container’s before/after and apply the styles as depicted. The example link provided below demonstrates how to do this with multiple rows of content.

<u>Position Property</u>

This property allows us to alter the location of an element in a web page. The six values to consider are static, relative, absolute, fixed, sticky, and inherit. By combining these values with the top, right, bottom, left, and z-index properties, we can move items around and layer them as needed.

By default, every element has a static position and so top, left, etc. will not work on them. When you give an element a position value of relative, those other properties can be manipulated. Absolute positioning will remove an element from the flow of the document. The positioning of these elements would be relative to other containers that have a “relative” position value. Unlike floats, the other content will behave as if the absolutely positioned content doesn’t exist.  Fixed does the same thing as absolute except the content is always relative to the viewport or screen. Sticky is experimental, and I wouldn’t recommend using it for the time being. It behaves similarly to fixed positioning though.

<u>Additional Reading</u>

<ul>

 <li><a href="https://css-tricks.com/almanac/properties/p/position/">https://css-tricks.com/almanac/properties/p/position/</a> (Position)</li>

 <li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/float">https://developer.mozilla.org/en-US/docs/Web/CSS/float</a> (Float)</li>

 <li><a href="https://css-tricks.com/all-about-floats/">https://css-tricks.com/all-about-floats/</a> (Float)</li>

 <li><a href="https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox">https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox</a> (Flexbox)</li>

 <li><a href="https://css-tricks.com/snippets/css/a-guide-to-flexbox/">https://css-tricks.com/snippets/css/a-guide-to-flexbox/</a> (Flexbox)</li>

 <li><a href="https://css-tricks.com/snippets/css/complete-guide-grid/">https://css-tricks.com/snippets/css/complete-guide-grid/</a> (Grid)</li>

 <li><a href="https://www.w3schools.com/css/css_grid.asp">https://www.w3schools.com/css/css_grid.asp</a> (Grid) – I’m normally against using w3schools since there are inaccuracies sometimes but this tutorial is solid. Exercise caution when using this website.</li>

</ul>

<strong><u>Class Examples:</u></strong>

<a href="https://iinf362.000webhostapp.com/examples/box-model-and-floats/">https://iinf362.000webhostapp.com/examples/box-model-and-floats/</a>

The link above points to the directory which has the html file and the css folder. The link below points to the html page so you can see it in action.

<a href="https://iinf362.000webhostapp.com/examples/box-model-and-floats/box-model-float-example.html">https://iinf362.000webhostapp.com/examples/box-model-and-floats/box-model-float-example.html</a>




<strong><u>If you haven’t done so already, please read the “Creating and Viewing our Web Pages.docx” file on Blackboard. You will not be able to submit anything for the assignment without completing that portion first. </u></strong>




<strong>CSS Positioning Exercises</strong>

Download the “CSS-Positioning-Exercises.zip” folder from Blackboard under the Lecture Notes for this week or in the Assignments folder. Inside of this zip folder, there will be two folders. One will be titled “black-white-page” and the other will be “rainbow-page.” In each of these folders, you’ll find HTML/CSS files and an associated image. Using the HTML/CSS provided (or your own CSS file), try to recreate the styles depicted in the image for each page. Your page doesn’t have to look <strong>exactly</strong> like my image but try to get as close as reasonably possible. I’ve listed some tips below for each page to help you with styles that may not be obvious. Please note that these are not exactly requirements but will help your get your page to look like the image provided. Each page is worth 10pts for a total of 20pts for this assignment.

<u>General Tips</u>

<ul>

 <li>If you use floats, float everything in one direction (I personally always use left)</li>

 <li>To center an image, use “display: block;” and “margin: 0 auto;” (images are always inline so when we display them with block, we can add width/height, margins, etc.)</li>

 <li>Padding/Margin will help with spacing (sometimes needs to be set to 0)</li>

 <li>Use my CSS file

  <ul>

   <li>It has code so you don’t have to perform calculations for width (box-sizing: border-box which is mentioned in the reading)</li>

   <li>The “.row” class declarations will clear the floats for you</li>

  </ul></li>

</ul>

<u>Black/White Page</u>

<ul>

 <li>The width of the left column of content is 30%</li>

 <li>The width of the right column (main content) is 65%</li>

 <li>The “product” divs have a width of 33%</li>

</ul>

<u>Rainbow Page</u>

<ul>

 <li>The divs are equally divided in each section (halves, one-third, and one-quarter but in percentages)</li>

 <li>The boxes inside of the red containers have a height of 100px</li>

 <li>The height of the blue boxes is 150px</li>

 <li>The width/height of the white box inside of the blue boxes are 50px</li>

 <li>The colors used specifically are yellow, red, pink, purple, green, blue, black, and white. I would recommend using the color names for this assignment instead of hexadecimal or RGB values (keep it simple for this week – best practice is to use hexadecimal)</li>

 <li>Pay attention to borders (1px solid black mostly)</li>

 <li>You can float and give borders to most divs in one declaration (isn’t necessary but might be a nice exercise in reducing your total code)</li>

</ul>

To receive credit for this assignment, please submit <strong>two </strong>links to your pages as a comment in the assignment submission area. You can find the assignment under the Lecture Notes for this week or in the Assignments folder. One link should direct me to your version of the black-white page and the other should point to your rainbow page. Please make sure your CSS is externally placed. The links will be due <u>Wednesday, February 26<sup>th</sup> at midnight.</u>

<strong>CSS Evaluation Initial Post &amp; Response</strong>

Read the following links about common mistakes made with CSS and general CSS best practices. Your task is to evaluate two websites based on the info provided. Do the websites make any of those mistakes? Do you think the mistakes matter given the context of the website? What best practices, if any, are followed? How would you improve the CSS?

<u>Discussion Links</u>

<ul>

 <li><a href="https://www.webfx.com/blog/web-design/12-common-css-mistakes-web-developers-make/">https://www.webfx.com/blog/web-design/12-common-css-mistakes-web-developers-make/</a></li>

 <li><a href="https://1stwebdesigner.com/css-best-practices/">https://1stwebdesigner.com/css-best-practices/</a> (scroll down a bit first)</li>

</ul>

<a href="http://www.webhostingsearch.com/articles/the-7-most-common-css-mistakes.php">http://www.webhostingsearch.com/articles/the-7-most-common-css-mistakes.php</a>