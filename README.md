0x00. Advanced HTML
HTML
Front-end


HTML - elements of a web page
HTML5 (Hypertext Markup Language) is the latest version of HTML, which is the standard markup language for creating web pages and web applications. In HTML5, several new elements were introduced to provide better structure and semantics to web documents. Here are some important HTML5 elements you should know when creating a web page:

<!DOCTYPE html>: This declaration is used to indicate that the document is an HTML5 document.

<html>: The root element of an HTML page. It wraps all the other elements on the page.

<head>: The head element contains metadata about the HTML document, such as the title, character encoding, and CSS stylesheets.

<title>: The title element specifies the title of the web page, which is displayed in the browser's title bar or tab.

<body>: The body element contains the main content of the web page, such as text, images, links, and other elements.

<h1>-<h6>: These elements represent headings of different levels, with <h1> being the highest and <h6> being the lowest.

<p>: The paragraph element is used to define a paragraph of text.

<a>: The anchor element is used to create hyperlinks. It can link to another web page, a specific section on the same page, or an email address.

<img>: The image element is used to embed images in a web page. It requires a source (src) attribute that specifies the image file's URL.

<ul> and <ol>: These elements are used to create unordered and ordered lists, respectively.

<li>: The list item element is used within <ul> or <ol> to define individual list items.

<div>: The division element is a generic container used to group and style other elements. It helps with layout and organization.

<span>: The span element is an inline container used to apply styles or attach JavaScript behaviors to a specific section of text.

<table>: The table element is used to create tabular data. It contains <tr> (table row), <td> (table data/cell), and <th> (table header) elements.

<form>: The form element is used to create interactive forms. It can contain input fields, buttons, checkboxes, and other form-related elements.

<input>: The input element is used to create various types of form controls, such as text fields, checkboxes, radio buttons, and submit buttons.

<textarea>: The textarea element is used to create a multi-line text input field.

<button>: The button element represents a clickable button.

<header>, <nav>, <main>, <section>, <article>, <footer>: These elements provide semantic structure to different parts of a web page, such as the header, navigation menu, main content, sections, articles, and footer.

<video> and <audio>: These elements are used to embed videos and audio files, respectively, within a web page.



RESOURCES
Read or watch:

HTML 5.2
HTML: HyperText Markup Language | MDN
HTML Reference - A free guide to all HTML elements and attributes
Can I use… Support tables for HTML5, CSS3, etc
HTML Cheat Sheet - WebsiteSetup



LEARNING OBJECTIVES

a.) Guidelines to follow for HTML

When working with HTML, it's important to follow certain guidelines and best practices to ensure that your code is well-structured, accessible, and maintainable. Here are some guidelines to consider when working with HTML:

Use proper indentation: Indent your code consistently to improve readability. Use spaces or tabs to align nested elements and make the structure clear.

Use semantic elements: HTML5 introduced semantic elements that provide meaning and structure to your content. Use elements like <header>, <nav>, <main>, <section>, <article>, and <footer> to convey the purpose and hierarchy of different sections of your page.

Provide a document type declaration: Start your HTML document with the <!DOCTYPE html> declaration to ensure that the browser interprets it as an HTML5 document.

Use valid HTML: Validate your HTML code to ensure it conforms to the HTML specification. Tools like the W3C Markup Validation Service can help you identify and fix any syntax errors or issues.

Use descriptive and accessible text: Provide meaningful and descriptive text within elements like headings (<h1>-<h6>), links (<a>), and alternative text for images (<img>). This improves accessibility for screen readers and search engine optimization.

Separate structure from presentation: Use CSS (Cascading Style Sheets) to define the visual presentation of your web page, rather than relying heavily on inline styles or deprecated HTML attributes like <font> or <b>. This separation of concerns makes your code more maintainable and easier to update.

Use appropriate attributes: Choose attributes that are appropriate for the elements you are using. For example, use the "src" attribute for images (<img>), the "href" attribute for links (<a>), and the "alt" attribute to provide alternative text for images.

Optimize for performance: Optimize your HTML for faster page loading. Minimize the use of unnecessary whitespace, remove redundant code, and keep the file size as small as possible.

Consider accessibility: Ensure that your HTML is accessible to users with disabilities. Use proper headings (<h1>-<h6>), provide alternative text for images (<img>), use appropriate color contrast, and follow other accessibility guidelines outlined in the Web Content Accessibility Guidelines (WCAG).

Keep up with evolving standards: Stay updated with the latest HTML standards, including HTML5 and its future iterations. HTML evolves over time, and new elements, attributes, and features may be introduced. Stay informed and adopt best practices as they emerge.




b.) How to create the skeleton of an HTML5 page

Open a text editor or an integrated development environment (IDE) to create a new HTML file.

Start with the document type declaration. Add the following line at the very beginning of your HTML file:

<!DOCTYPE html>
Create the opening and closing <html> tags. All the other elements will be placed within these tags.


<html>
...
</html>


Inside the <html> tags, create the <head> and <body> sections. The <head> section contains metadata and external resources, while the <body> section holds the visible content of the web page.

<html>
<head>
   ...
</head>
<body>
   ...
</body>
</html>


Within the <head> section, add the <title> element to specify the title of your web page. This title will be displayed in the browser's title bar or tab.
<head>
   <title>Your Page Title</title>
   ...
</head>


Within the <body> section, you can start adding the content of your web page. This can include headings, paragraphs, images, links, and other HTML elements.

<body>
   <h1>Welcome to My Web Page</h1>
   <p>This is the content of my web page.</p>
   <img src="image.jpg" alt="Description of the image">
   <a href="https://www.example.com">Click here</a> to visit a website.
   ...
</body>
Once you have added the desired content, save the file with an appropriate name and the .html extension (e.g., index.html).




c.) How to use semantic HTML tags to structure a web page

Identify the main sections of your web page: Determine the major sections or divisions of your content. For example, you might have a header, navigation, main content, sidebar, and footer.

Use the appropriate semantic tags for each section: Instead of relying on generic <div> elements, utilize specific semantic tags that best represent the purpose of each section. Here are some commonly used semantic tags:

<header>: Represents the introductory content or the top section of a page. It typically includes the site logo, site title, and possibly a navigation menu.
<nav>: Denotes a section that contains navigation links, such as a menu or a list of links to various parts of the website.
<main>: Represents the main content of the web page. It should contain the central focus of the page's content, excluding headers, footers, and sidebars.
<section>: Defines a distinct section of content within the web page. It groups related content together and is often used for chapters, articles, or different thematic blocks.
<article>: Represents a self-contained composition that can be independently distributed or reused. It can include blog posts, news articles, forum posts, or any other standalone content.
<aside>: Signifies a section that contains content tangentially related to the main content. It's commonly used for sidebars, pull quotes, or additional information.
<footer>: Indicates the footer section of the web page. It typically includes copyright information, contact details, and links to related resources.
Nest elements properly: Make sure to nest the semantic elements in a logical hierarchy that accurately reflects the structure of your content. For example, the <header> element might contain the site logo (<img>) and the navigation (<nav>) elements.

php
Copy code
<header>
   <img src="logo.png" alt="Logo">
   <nav>
      <ul>
         <li><a href="#">Home</a></li>
         <li><a href="#">About</a></li>
         <li><a href="#">Contact</a></li>
      </ul>
   </nav>
</header>
Use headings (<h1>-<h6>) appropriately: Headings play a crucial role in structuring your content. Use headings to provide hierarchical organization, with <h1> being the highest level and <h6> being the lowest. The <h1> tag is often used for the main title of the page, while subsequent headings (<h2>, <h3>, etc.) are used for subheadings.

css
Copy code
<main>
   <h1>Welcome to My Web Page</h1>
   <section>
      <h2>About</h2>
      <p>...</p>
   </section>
   <section>
      <h2>Services</h2>
      <p>...</p>
   </section>
</main>
By using semantic HTML tags, you provide meaning and structure to your web page, making it more accessible to users and search engines. Additionally, it enhances the maintainability of your code and helps improve the overall user experience.





d.) Which use cases to use div vs span

The choice between using <div> and <span> elements depends on the specific use case and the context in which they are used. Here's a general guideline for when to use each:

<div> element:

Use <div> when you need to create a block-level container to group and style other elements. It is commonly used for layout purposes, creating sections, or dividing the content of a web page.
Use <div> when you need to apply CSS styles or JavaScript behaviors to a larger section of content.
Example: Wrapping a group of elements within a <div> to apply a common styling or layout structure.
php
Copy code
<div class="container">
   <h1>Heading</h1>
   <p>Paragraph content</p>
   <a href="#">Link</a>
</div>
<span> element:

Use <span> when you need to apply styles or attach JavaScript behaviors to a specific section of text within a block-level element.
Use <span> when you want to target and manipulate specific portions of text within a larger element.
Example: Applying a CSS class or inline styling to a specific word or phrase within a paragraph.
php
Copy code
<p>
   Lorem ipsum dolor sit amet, consectetur adipiscing elit.
   Aliquam <span class="highlight">volutpat</span> mi sit amet leo feugiat, ac viverra justo ullamcorper.
</p>
In summary, use <div> when you need a block-level container for grouping and styling larger sections, and use <span> when you need to target and apply styles or behaviors to specific portions of text within a block-level element.




e.) The semantic value’s of header, main, footer, article, nav, section, aside

<header>:

Semantic value: Represents the introductory or top section of a page or a section within a page.
Typical use cases: Include site title, logo, navigation, search bars, introductory content, or other elements that provide context for the page.
<main>:

Semantic value: Represents the main content of a web page.
Typical use cases: Include the central focus of the page's content, excluding headers, footers, and sidebars. It should contain unique and essential content for that specific page.
<footer>:

Semantic value: Represents the footer section of a web page or a section within a page.
Typical use cases: Include copyright information, contact details, legal disclaimers, navigation links, or any other relevant information that belongs to the bottom section of the page.
<article>:

Semantic value: Represents a self-contained composition that can be independently distributed or reused.
Typical use cases: Include blog posts, news articles, forum posts, comments, or any other stand-alone content that makes sense to distribute or style as an independent piece.
<nav>:

Semantic value: Represents a section that contains navigation links.
Typical use cases: Include menus, site navigations, table of contents, or any other set of links that allow users to navigate within the current web page or to other pages on the website.
<section>:

Semantic value: Represents a thematic grouping of content within a web page.
Typical use cases: Include chapters, different sections of content, distinct topics, or any other divisions that help organize and group related content together.
<aside>:

Semantic value: Represents content that is tangentially related to the main content of the page.
Typical use cases: Include sidebars, pull quotes, related information, advertisements, or any other content that is not directly related to the main content but provides additional context or supplementary information.
By utilizing these semantic elements appropriately, you provide structure and meaning to your HTML code, making it more accessible to assistive technologies and search engines. Additionally, using semantic elements helps developers and designers understand the purpose and hierarchy of different sections within a web page.





f.) How to use headings (and why it’s important to follow the hierarchical order)

Headings (<h1>-<h6>) are important elements in HTML for organizing and structuring content on a web page. They serve multiple purposes, including:

Document structure: Headings provide a logical structure and hierarchy to your content, allowing users and assistive technologies to navigate and understand the organization of the page. They define the outline of the document and help users skim through the content.

Accessibility: Following a hierarchical order with headings improves the accessibility of your web page. Screen readers can use the heading structure to present an overview of the page and allow users to jump directly to specific sections of interest. Users with visual impairments or cognitive disabilities greatly benefit from clear and structured heading levels.

Search engine optimization (SEO): Search engines use headings to understand the structure and context of your content. Properly formatted and hierarchically ordered headings can help search engines determine the importance and relevance of different sections on your page, potentially improving your search rankings.

To effectively use headings, consider the following guidelines:

Use headings in a hierarchical order: Start with the main title of the page as <h1> (there should only be one <h1> per page), followed by subsections as <h2>, <h3>, and so on. Maintain a logical order where each heading level represents a progressively smaller section within its parent.

Don't skip heading levels: Avoid skipping heading levels (e.g., going from <h2> to <h4>) as it breaks the hierarchical structure and can confuse both users and search engines. Stick to a consistent and logical order.

Use headings to summarize content: Each heading should provide a concise summary or description of the content within the section it represents. This helps users quickly understand the topic of each section and navigate to relevant areas.

Limit the use of <h1>: Reserve the <h1> tag for the main title of your page. It should reflect the overall theme or purpose of the page and provide a clear context for the content that follows.

Example of proper hierarchical order:

html
Copy code
<h1>Main Title</h1>
<h2>Section 1</h2>
<h3>Subsection 1.1</h3>
<h3>Subsection 1.2</h3>
<h2>Section 2</h2>
<h3>Subsection 2.1</h3>
<h3>Subsection 2.2</h3>
Following the proper hierarchical order with headings helps create a well-structured, accessible, and SEO-friendly web page. It improves navigation, readability, and comprehension of your content for all users.





g.) How to make lists in HTML

In HTML, you can create two types of lists: ordered lists and unordered lists. Here's how to create each type:

Ordered List (<ol>):

An ordered list represents a list of items in a specific order, usually with numbers or letters.
To create an ordered list, use the <ol> element, and place each list item inside <li> (list item) tags.
Example:

html
Copy code
<ol>
   <li>First item</li>
   <li>Second item</li>
   <li>Third item</li>
</ol>
Output:

First item
Second item
Third item
Unordered List (<ul>):

An unordered list represents a list of items without any particular order. The items are typically marked with bullet points.
To create an unordered list, use the <ul> element, and place each list item inside <li> tags.
Example:

html
Copy code
<ul>
   <li>Red</li>
   <li>Green</li>
   <li>Blue</li>
</ul>
Output:

Red
Green
Blue
You can also create nested lists by placing one list inside another. For example:

html
Copy code
<ol>
   <li>First item</li>
   <li>Second item
      <ul>
         <li>Nested item 1</li>
         <li>Nested item 2</li>
      </ul>
   </li>
   <li>Third item</li>
</ol>
Output:

First item
Second item
Nested item 1
Nested item 2
Third item

use ordered lists (<ol>) when the order of items is important, and use unordered lists (<ul>) when the order doesn't matter. Lists are a useful way to present and organize information in a structured manner on your web page.





h.) The differences between medias (SVG, GIF, PNG, JPG)

SVG, GIF, PNG, and JPG are different file formats used for different purposes. Here are the key differences between them:

SVG (Scalable Vector Graphics):

File type: SVG files are vector-based graphics that use XML markup.
Scalability: SVGs are resolution-independent and can be scaled to any size without loss of quality.
Scalable Animations: SVGs support animations, interactivity, and scripting.
Editability: SVGs can be edited using vector graphics editors like Adobe Illustrator.
Usage: SVGs are commonly used for logos, icons, illustrations, and graphics that require scalability and interactivity.
GIF (Graphics Interchange Format):

File type: GIF files are bitmap images that support animations and transparency.
Animation: GIFs can contain multiple frames, allowing for simple animations.
Transparency: GIFs can have transparent backgrounds.
Limited Colors: GIFs are limited to a maximum of 256 colors, which can result in reduced image quality for complex images.
Usage: GIFs are often used for simple animations, clipart, and graphics with transparency.
PNG (Portable Network Graphics):

File type: PNG files are bitmap images that support lossless compression and transparency.
Lossless Compression: PNGs use lossless compression, meaning they maintain image quality while reducing file size.
Transparency: PNGs support full alpha transparency, allowing for images with transparent backgrounds.
Rich Colors: PNGs support millions of colors and can accurately represent complex images.
Usage: PNGs are widely used for images with transparency, screenshots, logos, and graphics that require high-quality and lossless compression.
JPG/JPEG (Joint Photographic Experts Group):

File type: JPG files are compressed bitmap images.
Lossy Compression: JPGs use lossy compression, which reduces file size by sacrificing some image quality.
High Compression: JPGs can achieve high levels of compression, resulting in smaller file sizes.
Photographs: JPGs are well-suited for photographs and complex images with many colors and gradients.
Usage: JPGs are commonly used for web images, digital photography, and situations where file size needs to be minimized.
In summary, SVG is a vector-based format suitable for scalable graphics and animations, GIF is used for simple animations and graphics with transparency, PNG is preferred for high-quality images with transparency, and JPG is commonly used for compressed photographs and web images where file size matters. The choice of format depends on the specific requirements of the image, such as scalability, transparency, animation, and image complexity.






i.) How to structure data in a table

To structure data in a table in HTML, follow these steps:

Create the table structure: Start by using the <table> element to define the table. Inside the <table> element, you will include the table rows (<tr>) and table data/cells (<td>) or table headers (<th>) elements.

Example:

html
Copy code
<table>
   <tr>
      <th>Header 1</th>
      <th>Header 2</th>
      <th>Header 3</th>
   </tr>
   <tr>
      <td>Data 1</td>
      <td>Data 2</td>
      <td>Data 3</td>
   </tr>
   <!-- Add more rows and data as needed -->
</table>
Define table headers: Use the <th> element to create table headers. These headers should represent the column labels or titles for your data.

Add table data/cells: Use the <td> element to create table data or cells. These cells will contain the actual data or content you want to display.

Group rows with table sections: You can also use table sections to group rows together for better structure and styling. The sections include <thead> (table header), <tbody> (table body), and <tfoot> (table footer).

Example:

html
Copy code
<table>
   <thead>
      <tr>
         <th>Header 1</th>
         <th>Header 2</th>
         <th>Header 3</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Data 1</td>
         <td>Data 2</td>
         <td>Data 3</td>
      </tr>
      <!-- Add more rows and data as needed -->
   </tbody>
   <tfoot>
      <tr>
         <td colspan="3">Footer content</td>
      </tr>
   </tfoot>
</table>
Use colspan and rowspan attributes: The colspan attribute allows a cell to span multiple columns, while the rowspan attribute allows a cell to span multiple rows. This can be useful for merging cells or creating more complex table structures.

Example:

html
Copy code
<table>
   <tr>
      <th colspan="2">Header 1 and 2</th>
      <th>Header 3</th>
   </tr>
   <tr>
      <td rowspan="2">Data 1</td>
      <td>Data 2</td>
      <td>Data 3</td>
   </tr>
   <tr>
      <td>Data 4</td>
      <td>Data 5</td>
   </tr>
</table>




j.) How to integrate a video in a webpage

Prepare your video file: Convert your video to a web-compatible format like MP4, WebM, or Ogg. It's recommended to provide multiple formats to support different browsers.

Place the <video> element in your HTML:

html
Copy code
<video controls>
   <source src="video.mp4" type="video/mp4">
   <source src="video.webm" type="video/webm">
   <source src="video.ogg" type="video/ogg">
   Your browser does not support the video tag.
</video>
Add the video sources: Inside the <video> element, include one or more <source> elements. Each <source> element specifies the video file URL and its corresponding MIME type using the src and type attributes.

The src attribute should point to the URL of the video file.
The type attribute specifies the MIME type of the video file. It helps the browser select the appropriate source to play based on the supported formats.
Provide fallback content: In case the browser doesn't support the <video> element or any of the specified video formats, the text within the <video> element will be displayed. You can include a message or alternative content for unsupported browsers.

Add optional attributes:

controls: This attribute adds video controls (play, pause, volume, etc.) to the video player. It allows users to interact with the video.
autoplay: If you want the video to start playing automatically when the page loads, you can include the autoplay attribute.
loop: To make the video play continuously in a loop, include the loop attribute.
Example with additional attributes:

html
Copy code
<video controls autoplay loop>
   <source src="video.mp4" type="video/mp4">
   <source src="video.webm" type="video/webm">
   <source src="video.ogg" type="video/ogg">
   Your browser does not support the video tag.
</video>
Customize video styling: You can apply CSS styles to the <video> element to control its appearance, such as width, height, borders, and positioning.




k.) How to integrate an audio file in a webpage

Prepare your audio file: Convert your audio file to a web-compatible format like MP3, WAV, or Ogg. It's recommended to provide multiple formats to support different browsers.

Place the <audio> element in your HTML:

html
Copy code
<audio controls>
   <source src="audio.mp3" type="audio/mpeg">
   <source src="audio.wav" type="audio/wav">
   <source src="audio.ogg" type="audio/ogg">
   Your browser does not support the audio tag.
</audio>
Add the audio sources: Inside the <audio> element, include one or more <source> elements. Each <source> element specifies the audio file URL and its corresponding MIME type using the src and type attributes.

The src attribute should point to the URL of the audio file.
The type attribute specifies the MIME type of the audio file. It helps the browser select the appropriate source to play based on the supported formats.
Provide fallback content: Similar to the video integration, if the browser doesn't support the <audio> element or any of the specified audio formats, the text within the <audio> element will be displayed. You can include a message or alternative content for unsupported browsers.

Add optional attributes:

controls: This attribute adds audio controls (play, pause, volume, etc.) to the audio player. It allows users to interact with the audio.
autoplay: If you want the audio to start playing automatically when the page loads, you can include the autoplay attribute.
loop: To make the audio play continuously in a loop, include the loop attribute.
Example with additional attributes:

html
Copy code
<audio controls autoplay loop>
   <source src="audio.mp3" type="audio/mpeg">
   <source src="audio.wav" type="audio/wav">
   <source src="audio.ogg" type="audio/ogg">
   Your browser does not support the audio tag.
</audio>
Customize audio styling: You can apply CSS styles to the <audio> element to control its appearance, such as width, height, borders, and positioning.





l.) How to embed external content
Embedding Images:

Use the <img> element to embed an external image into your webpage.
Set the src attribute of the <img> element to the URL of the image file.
You can also provide alternative text using the alt attribute for accessibility purposes.
Example:
html
Copy code
<img src="https://example.com/image.jpg" alt="Description of the image">
Embedding Videos:

Use the <video> element to embed an external video into your webpage.
Provide one or more <source> elements within the <video> element to specify different video formats.
Set the src attribute of each <source> element to the URL of the video file, and define the MIME type using the type attribute.
You can also include optional attributes like controls, autoplay, and loop.
Example:
html
Copy code
<video controls>
   <source src="https://example.com/video.mp4" type="video/mp4">
   <source src="https://example.com/video.webm" type="video/webm">
</video>
Embedding Audio:

Use the <audio> element to embed external audio content into your webpage.
Similar to video embedding, provide one or more <source> elements within the <audio> element to specify different audio formats.
Set the src attribute of each <source> element to the URL of the audio file, and define the MIME type using the type attribute.
You can also include optional attributes like controls, autoplay, and loop.
Example:
html
Copy code
<audio controls>
   <source src="https://example.com/audio.mp3" type="audio/mpeg">
   <source src="https://example.com/audio.wav" type="audio/wav">
</audio>
Embedding External Web Pages:

Use the <iframe> element to embed an external web page into your webpage.
Set the src attribute of the <iframe> element to the URL of the external web page.
Specify the dimensions of the iframe using the width and height attributes.
Example:
html
Copy code
<iframe src="https://example.com" width="800" height="600"></iframe>




m.) How to correctly structure an HTML page

To correctly structure an HTML page, you should follow a standardized structure that includes essential elements. Here's a basic outline to help you structure your HTML page properly:

Document Type Declaration:

Begin your HTML document with a document type declaration to specify the HTML version you are using.
Example: <!DOCTYPE html>
HTML Element:

Wrap the entire content of your HTML page inside the <html> element.
The <html> element serves as the root element of your HTML document.
Example:
html
Copy code
<!DOCTYPE html>
<html>
...
</html>
Head Section:

Within the <html> element, include the <head> section.
The <head> section provides meta information, document title, and links to external resources.
Example:
html
Copy code
<html>
<head>
   <meta charset="UTF-8">
   <title>Your Page Title</title>
   <link rel="stylesheet" href="styles.css">
   <script src="script.js"></script>
</head>
...
</html>
Body Section:

Within the <html> element, include the <body> section.
The <body> section contains the visible content of your web page.
Example:
html
Copy code
<html>
<head>
   ...
</head>
<body>
   <header>
      ...
   </header>
   <main>
      ...
   </main>
   <footer>
      ...
   </footer>
</body>
</html>
Structural Elements:

Within the <body> section, use structural elements to organize and define the layout of your web page.
Examples of structural elements include <header>, <nav>, <main>, <section>, <article>, <aside>, and <footer>.
Use these elements appropriately to provide semantic structure to your page.
Example:
html
Copy code
<body>
   <header>
      <h1>Website Title</h1>
      <nav>
         <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
         </ul>
      </nav>
   </header>
   <main>
      <section>
         <h2>Section Title</h2>
         <p>Section content...</p>
      </section>
      ...
   </main>
   <footer>
      <p>&copy; 2023 Your Website</p>
   </footer>
</body>




REQUIREMENTS
A README.md file at the root of the folder of the project is mandatory
Your code should be W3C compliant and validate with W3C-Validator
Techium will be the name of the company we will use across our webpages.



