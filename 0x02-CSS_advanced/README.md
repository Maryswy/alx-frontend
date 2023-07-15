0x02. Advanced CSS
CSS
Front-end


Concepts
For this project, we expect you to look at these concepts:

CSS fundamentals
CSS advanced



Resources
Read or watch

CSS Reference - A free visual guide to CSS
Can I use,,, Support tables for HTML5, CSS3, etc
CSS Reference
CSS Properties | HTML Dog
Box Sizing
CSS Selectors weight
CSS specificity calculator
Play with CSS selector



Learning Objectives
GENERAL

1. Selectors, properties, and values
In advanced CSS, selectors, properties, and values play crucial roles in styling and manipulating the appearance of HTML elements. Here's a breakdown of each term:

Selectors: Selectors are used to target specific HTML elements or groups of elements that you want to style. They define the scope of the CSS rules that follow. Some common selector types include:

Element selector: Selects elements based on their tag name. For example, to select all <h1> headings, you would use the selector h1.

Class selector: Selects elements based on their assigned class attribute. It is denoted by a period (.) followed by the class name. For example, to select all elements with the class "container," you would use the selector .container.

ID selector: Selects a single element based on its unique ID attribute. It is denoted by a hash (#) followed by the ID name. For example, to select an element with the ID "logo," you would use the selector #logo.

Attribute selector: Selects elements based on their attributes. For example, to select all elements with a target="_blank" attribute, you would use the selector [target="_blank"].

Pseudo-class selector: Selects elements based on a specific state or condition. For example, :hover selects elements when the mouse is hovering over them.

Properties: CSS properties determine the visual or behavioral characteristics of the selected elements. They are assigned values to define how the elements should appear or behave. Some common CSS properties include:

color: Sets the text color.
font-size: Sets the size of the font.
background-color: Sets the background color.
width: Sets the width of an element.
height: Sets the height of an element.
margin: Sets the margin space around an element.
padding: Sets the padding space inside an element.
border: Sets the border around an element.
Values: Values are assigned to CSS properties to define their specific characteristics. Values can be in different units (pixels, percentages, ems) or can take specific keywords. For example:

color: red;: The value "red" sets the text color to red.
font-size: 16px;: The value "16px" sets the font size to 16 pixels.
background-color: #FFFFFF;: The value "#FFFFFF" sets the background color to white.
width: 50%;: The value "50%" sets the width to 50% of the parent element's width.
By combining selectors, properties, and values, you can create powerful CSS rules that affect the presentation and behavior of your HTML elements in advanced ways.



2. The difference between block and inline styling
The difference between block and inline styling refers to how elements are displayed and how they interact with other elements in the document flow.

Block-level elements:

By default, block-level elements start on a new line and take up the full available width of their parent container.
Examples of block-level elements are <div>, <p>, <h1> to <h6>, <section>, <article>, <ul>, <li>, etc.
Block-level elements can have height, width, padding, margin, and border properties applied to them.
Multiple block-level elements stack vertically, one below the other.
Inline-level elements:

Inline-level elements do not start on a new line and only take up the space they need to display their content.
Examples of inline-level elements are <span>, <a>, <strong>, <em>, <img>, etc.
Inline-level elements usually cannot have width, height, top/bottom margin, or padding applied directly to them (though they can have left/right margin and padding).
Inline-level elements flow within the text content of a block-level element, and they do not disrupt the line flow. They appear alongside each other horizontally until the available space is exhausted, and then they wrap to the next line.
When it comes to styling, block and inline elements behave differently:

Block-level styling:

Block-level elements can have their width, height, margin, padding, and border properties adjusted freely.
They can be given a specific width to occupy a defined space on the page.
Block-level elements can have vertical margin collapsing with adjacent elements.
Inline-level styling:

Inline-level elements are not affected by width, height, or vertical margin properties.
They typically cannot have a fixed width or height; instead, their dimensions are determined by their content.
Inline-level elements can have horizontal margin and padding properties.
Inline-level elements can be styled with vertical-align property to adjust their vertical alignment with respect to other inline elements.
It's important to note that the display property can be used to change the default behavior of elements. For example, you can set an inline element to behave like a block-level element using display: block;, and vice versa using display: inline; or display: inline-block;.

Understanding the differences between block and inline styling helps in creating layouts and applying appropriate styles to elements based on their intended behavior and appearance in a web page.



3. How to ensure consistency across all browers (CSS reset)
To ensure consistency across different browsers, one commonly used technique is to employ a CSS reset or CSS normalize. These approaches help neutralize browser-specific styles and establish a consistent starting point for styling. Here's an overview of how to use a CSS reset:

Understand the purpose: CSS resets aim to remove or reset default browser styles so that elements start with a clean slate. This helps avoid inconsistencies and ensures a more predictable rendering across different browsers.

Choose a CSS reset or normalize: There are various CSS reset or normalize libraries available that you can use. Some popular options include:

Eric Meyer's CSS Reset: This is a widely used reset that resets many common elements to a consistent baseline. You can include it in your project by adding the CSS code to your stylesheet. You can find the code and implementation details at: https://meyerweb.com/eric/tools/css/reset/

Normalize.css: This is a normalization stylesheet that aims to make browsers render elements consistently while preserving useful defaults. It provides a solid foundation for styling. You can include it by downloading the CSS file from https://necolas.github.io/normalize.css/ and linking it in your HTML file.

Other libraries: There are alternative libraries available that offer different levels of reset or normalization. Some examples include sanitize.css, base.css, or you can even create your own custom reset.

Include the CSS reset in your project: Once you have chosen a CSS reset or normalize library, you need to include it in your project. There are a few ways to do this:

Linking the external stylesheet: If you are using an external CSS file, download the reset/normalize file and link it in the <head> section of your HTML file using the <link> tag.

Adding CSS code directly: If you prefer, you can copy the CSS code from the reset/normalize file and paste it directly into your own CSS file.

Order of inclusion: It is important to include the CSS reset or normalize before your own custom stylesheets. This ensures that the reset/normalize rules take effect first, and you can then build upon them with your desired styles.

Test and adapt: After including the CSS reset, thoroughly test your website across different browsers to ensure consistency. You may still need to make adjustments and overrides to achieve the desired styling for specific elements.

By employing a CSS reset or normalize, you establish a consistent foundation for your styles and minimize the impact of browser-specific defaults, leading to improved cross-browser consistency.



4. How to setup CSS variables
Setting up CSS variables, also known as CSS custom properties, allows you to define reusable values that can be used throughout your CSS code. Here's how you can set up CSS variables:

Declare CSS variables:

CSS variables are defined using the -- prefix followed by a name. For example, --primary-color or --font-size.
Variables are typically declared inside a selector block, such as :root, to make them available globally. The :root selector represents the root element (usually <html>) of the document.
An example of declaring CSS variables in the :root selector:
:root {
  --primary-color: #ff0000;
  --font-size: 16px;
}


Use CSS variables:

Once the variables are declared, you can use them by referencing their names.
To reference a variable, use the var() function and pass the variable name as an argument. For example:
.my-element {
  color: var(--primary-color);
  font-size: var(--font-size);
}


Updating CSS variables dynamically:

CSS variables can be updated dynamically using JavaScript. You can modify the value of a CSS variable using the setProperty() method on the style property of an element.
Here's an example of updating a CSS variable using JavaScript:
// Get the root element
const root = document.documentElement;

// Update the value of a CSS variable
root.style.setProperty('--primary-color', '#00ff00');


By using CSS variables, you can centralize and reuse values throughout your CSS code, making it easier to maintain and update styles consistently. Additionally, with the ability to modify variables dynamically using JavaScript, you can create dynamic themes, respond to user interactions, or implement other dynamic styling features.




5. The differences between inline, embeded and external CSS
The differences between inline, embedded, and external CSS relate to how and where the CSS code is written and linked within an HTML document. Here's an overview of each type:

Inline CSS:

Inline CSS is applied directly within an HTML element using the style attribute.
CSS rules are written as attribute-value pairs within double quotes (" ").
Inline styles affect only the specific element they are applied to.
Example:
<h1 style="color: blue;">Hello, World!</h1>

Embedded CSS:

Embedded CSS is placed within the <style> tags in the <head> section of an HTML document.
CSS rules are written between the opening and closing <style> tags.
Embedded styles affect the elements targeted by the CSS selectors used within the embedded CSS.
Example:
<head>
  <style>
    h1 {
      color: blue;
    }
  </style>
</head>
<body>
  <h1>Hello, World!</h1>
</body>

External CSS:

External CSS is written in a separate CSS file and linked to the HTML document using the <link> tag.
The CSS rules are written in the external CSS file, which has a .css extension.
External stylesheets can be reused across multiple HTML documents, promoting consistency and separation of concerns.
Example:
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <h1>Hello, World!</h1>
</body>

styles.css:
h1 {
  color: blue;
}


Key considerations for choosing the appropriate method:

Inline CSS is useful for applying immediate and specific styles to individual elements.
Embedded CSS allows you to keep the styles separate from the HTML content but still within the same HTML document.
External CSS provides the most flexibility, as it allows for centralizing styles in a separate file that can be shared among multiple HTML documents.
Overall, the choice between inline, embedded, or external CSS depends on factors such as the specific styling needs, the scale of the project, and the desire for maintainability and reusability.




6. How grid systems work (with floats)
Grid systems based on floats were a popular approach for creating responsive layouts before CSS Grid and Flexbox became widely supported. These grid systems used a combination of CSS floats and additional CSS classes to create a grid-like structure. Here's an overview of how grid systems using floats work:

HTML structure:

The HTML structure typically consists of a container element that wraps multiple grid items or columns.
Grid items are usually represented as child elements within the container, and they occupy specific widths based on the desired layout.
CSS float property:

The CSS float property is applied to grid items to make them float either to the left or right within their container.
By floating elements, they are taken out of the normal flow, allowing other elements to wrap around them.
Width and clear:

To control the width of the grid items, classes or custom CSS rules are used to define the desired percentage-based widths (e.g., 25%, 33.33%, etc.).
Additional classes may be used to specify different widths for different screen sizes (e.g., "col-md-6" for a 50% width on medium screens).
To ensure proper wrapping and alignment, a clearfix technique is commonly employed. This involves using the clear: both property on pseudo-elements (:before or :after) to clear the floats.
Gutters and margins:

Gutters, or spacing between grid items, can be achieved by applying appropriate margins to the grid items.
These margins can be adjusted using CSS classes or custom CSS rules to control the spacing between the items.
Responsive behavior:

Grid systems using floats often incorporate media queries to adjust the layout based on different screen sizes or devices.
Additional CSS classes or rules can be defined within media queries to modify the widths or apply specific styles at different breakpoints.
It's worth noting that while grid systems using floats were widely used in the past, they have certain limitations and complexities compared to modern CSS Grid or Flexbox. Float-based grid systems can sometimes result in challenges related to vertical alignment, equal-height columns, and nesting. CSS Grid and Flexbox provide more straightforward and powerful solutions for creating grid layouts with more flexibility and responsiveness.

However, if you encounter legacy code or frameworks that still use float-based grid systems, understanding how they work can help you maintain or update those systems if needed.




7. The difference between icons webfonts and SVG icons
Icons in web development can be implemented using webfonts or SVG icons. Here's a comparison between the two:

Webfonts:

Webfonts use font files (such as .woff or .woff2) that contain vector-based icon representations as glyphs within a font.
Icons are treated as characters in a font and can be styled using CSS properties like color, font-size, and text-shadow.
Advantages of webfonts include:
Scalability: Icons can be easily scaled up or down without loss of quality.
Consistency: Icons can be styled consistently with other text elements.
Accessibility: Webfonts are accessible to screen readers as they are treated as regular text.
Disadvantages of webfonts include:
Limited customization: Customizing the appearance of icons can be challenging as they are restricted by the font's design.
Loading time: Loading the entire font file, even if only a few icons are used, can increase page load times.
Limited interactivity: Webfont icons don't inherently support complex interactions or animations.
SVG Icons:

SVG (Scalable Vector Graphics) icons are XML-based vector images that can be embedded directly in the HTML markup using the <svg> element or used as external files.
Icons are defined as paths, shapes, or groups of graphical elements, allowing for precise customization and manipulation.
Advantages of SVG icons include:
Customization: SVG icons are highly customizable and can be modified using CSS, JavaScript, or inline attributes.
Interactivity: SVG icons support complex interactions, animations, and dynamic modifications.
File size control: SVG files can be optimized for size by removing unnecessary elements or compressing the code.
Disadvantages of SVG icons include:
Accessibility: SVG icons may require additional work to ensure accessibility for screen readers and other assistive technologies.
Styling limitations: Applying text-related CSS properties directly to SVG icons can be more complex compared to webfonts.
Browser support: While SVG is widely supported, some older browsers may have limited or inconsistent support for certain SVG features.
In summary, webfonts provide an easy and consistent way to incorporate icons using font files, whereas SVG icons offer greater customization options, interactivity, and control over the appearance. The choice between webfonts and SVG icons depends on the specific requirements of your project, including design flexibility, interactivity needs, and browser compatibility considerations.




8. The difference between pseudo-classes and pseudo-elements
Pseudo-classes and pseudo-elements are both CSS selectors that target specific elements based on certain conditions or positions. However, they differ in how they select and style elements. Here's an explanation of each:

Pseudo-classes:

Pseudo-classes select elements based on specific states or conditions that they are in.
Pseudo-classes are denoted with a colon (:) followed by the name of the pseudo-class.
Examples of pseudo-classes include :hover, :active, :focus, :checked, :nth-child(), :first-child, and many more.
Pseudo-classes are used to apply styles based on user interactions, element hierarchy, form input states, and other dynamic conditions.
Example:
a:hover {
  color: red;
}

input:valid {
  border: 1px solid green;
}


Pseudo-elements:

Pseudo-elements target and style specific parts of an element or create virtual elements that do not exist in the HTML markup.
Pseudo-elements are denoted with a double colon (::) followed by the name of the pseudo-element.
Examples of pseudo-elements include ::before, ::after, ::first-line, ::first-letter, and ::selection.
Pseudo-elements allow you to insert content before or after an element, style the first line or first letter of text, or target specific portions of an element for styling purposes.
Example:
p::before {
  content: ">>";
}

h1::first-letter {
  font-size: 2em;
  color: blue;
}


In summary, pseudo-classes select elements based on their states or conditions, such as user interactions or element positions. Pseudo-elements, on the other hand, target specific parts of elements or create virtual elements to apply styles. Both pseudo-classes and pseudo-elements are powerful tools in CSS that allow for fine-grained control and styling of elements based on various conditions and positions.




9. How to make background gradients
To create background gradients in CSS, you can use the background property with the linear-gradient() or radial-gradient() functions. Here's how to make background gradients using these functions:

Linear Gradients:

Linear gradients transition smoothly between two or more colors in a linear direction.
Use the linear-gradient() function with the desired color stops and direction.
Syntax:
selector {
  background: linear-gradient(direction, color-stop1, color-stop2, ...);
}

Example:
/* Horizontal Gradient */
.gradient-box {
  background: linear-gradient(to right, #ff0000, #00ff00);
}

/* Diagonal Gradient */
.gradient-box {
  background: linear-gradient(45deg, #ff0000, #00ff00);
}



Radial Gradients:

Radial gradients transition smoothly between two or more colors radiating from a center point.
Use the radial-gradient() function with the desired color stops and shape.
Syntax:
selector {
  background: radial-gradient(shape, color-stop1, color-stop2, ...);
}

Example:
/* Circular Gradient */
.gradient-circle {
  background: radial-gradient(circle, #ff0000, #00ff00);
}

/* Elliptical Gradient */
.gradient-ellipse {
  background: radial-gradient(ellipse, #ff0000, #00ff00);
}



Color Stops:

Color stops define the colors and positions within the gradient.
You can specify color stops using color values (e.g., #ff0000, rgb(255, 0, 0), etc.) or color keywords (e.g., red, green, etc.).
You can also include percentage-based positions to control the transition points between colors.
Example:
/* Color Stops with Positions */
.gradient-box {
  background: linear-gradient(to right, red 20%, blue 50%, green 80%);
}


By using the linear-gradient() and radial-gradient() functions, along with appropriate color stops and positions, you can create various background gradients to enhance the visual appeal of your website or application.




10. How to animate elements in CSS
To animate elements in CSS, you can use CSS animations. CSS animations allow you to apply transitions or keyframe animations to elements, resulting in smooth and visually appealing effects. Here's a step-by-step guide on how to animate elements in CSS:

Define an animation:

Start by using the @keyframes rule to define the animation.
Specify a name for the animation and define the animation keyframes at different percentages (0%, 25%, 50%, etc.).
Within each keyframe, define the CSS properties and values that you want to animate.
Example:
@keyframes myAnimation {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}


Apply the animation to an element:

Select the element you want to animate using a CSS selector.
Use the animation property to specify the name of the animation, duration, timing function, delay, and other optional parameters.
Example:
.myElement {
  animation: myAnimation 2s ease-in-out 0s infinite alternate;
}


Customize animation properties:

You can customize various animation properties to control the behavior and appearance of the animation.
Common animation properties include animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, and animation-fill-mode.
Example:
.myElement {
  animation-name: myAnimation;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: 0s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-fill-mode: forwards;
}



Trigger the animation:

By default, animations start automatically when the page loads or when the element becomes visible.
You can also trigger animations based on user interactions, such as hover or click events, by using pseudo-classes like :hover or adding/removing classes with JavaScript.
Example:
.myElement:hover {
  animation-play-state: paused;
}

CSS animations provide a powerful way to create engaging and dynamic effects in your web projects. By defining keyframes and applying animations to elements, you can achieve smooth transitions, transform properties, fading effects, and more. Experiment with different animation properties and durations to achieve the desired visual impact.




11. How to transform (2d, 3d) elements
To transform elements in CSS, you can use the transform property. The transform property allows you to apply various transformations to elements, including 2D and 3D transformations. Here's how to transform elements in CSS:

2D Transformations:

To apply 2D transformations, use the transform property with appropriate functions such as translate(), rotate(), scale(), skew(), or their combinations.
Example:
.myElement {
  transform: translate(50px, 50px) rotate(45deg) scale(1.2);
}


3D Transformations:

To apply 3D transformations, use the transform property with 3D transformation functions such as translate3d(), rotate3d(), scale3d(), perspective(), or their combinations.
Example:
.myElement {
  transform: translate3d(50px, 50px, 0) rotateX(45deg) scale3d(1.2, 1.2, 1);
}


Transformation Functions:

Here are some commonly used transformation functions:
translate(x, y) or translate3d(x, y, z): Moves the element along the X, Y, and Z axes.
rotate(angle) or rotate3d(x, y, z, angle): Rotates the element around a specified axis.
scale(x, y) or scale3d(x, y, z): Scales the element along the X, Y, and Z axes.
skew(x-angle, y-angle): Skews the element along the X and Y axes.
perspective(depth): Applies a perspective view to 3D transformed elements.
Multiple Transformations:

You can combine multiple transformation functions by separating them with spaces.
Example:
.myElement {
  transform: translate(50px, 50px) rotate(45deg) scale(1.2);
}


Transitioning Transforms:

You can animate transitions between different transformations by using the transition property. This allows for smooth and controlled transformations.
Example:
.myElement {
  transition: transform 0.5s ease-in-out;
}

.myElement:hover {
  transform: translate(100px, 100px) rotate(90deg);
}

By utilizing the transform property and its corresponding transformation functions, you can create engaging and interactive visual effects for your elements. Experiment with different transformation functions, combinations, and transitions to achieve the desired transformation effects in your CSS.




12. What vendor prefixes are
Vendor prefixes, also known as browser prefixes or vendor-specific prefixes, are a mechanism used in CSS to apply experimental or non-standard CSS properties and features that are not yet fully supported by all web browsers. These prefixes are specific to particular browser vendors and are added to CSS properties to ensure compatibility during the development phase. Here are some common vendor prefixes:

-webkit- (Webkit browsers such as Chrome and Safari)
-moz- (Mozilla Firefox)
-ms- (Internet Explorer and Microsoft Edge)
-o- (Opera)
For example, when using the CSS transform property, you might include the vendor prefixes to ensure compatibility across browsers:
.myElement {
  -webkit-transform: translateX(50px);
  -moz-transform: translateX(50px);
  -ms-transform: translateX(50px);
  -o-transform: translateX(50px);
  transform: translateX(50px);
}


The vendor prefixes are gradually phased out as browser support for the standard versions of CSS properties increases. It's important to note that vendor prefixes should be used with caution and mainly during the development phase. As browser support improves, it is recommended to transition to the standard version of CSS properties and remove or minimize the use of vendor prefixes.

To facilitate this transition and minimize manual effort, CSS pre-processors or post-processors like Autoprefixer can be used. These tools automatically add or remove vendor prefixes based on the compatibility requirements specified.

Keep in mind that checking browser compatibility and understanding the level of support for specific CSS properties is crucial to ensure a consistent and well-rendered experience across different web browsers.



Requirements
General
Allowed editors: vi, vim, emacs, VSCode, Atom
All your files will be interpreted on Chrome (version 78.x)
All your files should end with a new line
All your files should start by a comment describing the task
A README.md file, at the root of the folder of the project, is mandatory
Your code should be W3C compliant and validate with W3C-Validator