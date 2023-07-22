0x03. Responsive design
HTML
CSS
Front-end
Responsive design



Resources
Read or watch:

The building blocks of responsive design - Progressive web apps | MDN
A pragmatic guide to designing and building responsive web applications | developerlife.com
Understanding the difference between mobile-first, adaptive and responsive design
LukeW | Mobile First
Media Queries | A collection of inspirational websites using media queries and responsive web design
Responsive Design Newsletter



LEARNING OBJECTIVES
GENERAL

1. Mobile-first design
Mobile-first design is a concept within responsive web design that prioritizes designing and developing a website or web application for mobile devices first, before considering the design for larger screens like desktops or tablets. The approach involves starting the design process with the smallest screen size in mind and then gradually adding complexity and optimizing layouts as the screen size increases.

The traditional approach to web design involved designing for desktop screens first and then retrofitting the design to fit smaller screens. However, with the proliferation of mobile devices and the growing number of users accessing the internet on smartphones and tablets, the mobile-first approach has become more popular and practical.

Key characteristics of mobile-first design in responsive design include:

Content prioritization: With limited screen space on mobile devices, mobile-first design encourages a focus on essential content and functionality. This ensures that the most critical information is easily accessible on smaller screens.

Progressive enhancement: Mobile-first design uses progressive enhancement, where additional design elements and features are added as the screen size increases. This ensures that users on larger screens get an enhanced and optimized experience without sacrificing the core functionality available on mobile devices.

Performance optimization: Mobile-first design often leads to better performance because it forces designers and developers to be mindful of the resources they use and how they deliver content to mobile users. This can result in faster load times and a more efficient browsing experience.

Fluid and flexible layouts: Mobile-first designs typically use fluid and flexible layouts that adapt to various screen sizes and orientations. This allows the content to reflow and adjust appropriately based on the device's screen size, ensuring a seamless experience across different devices.

Touch-friendly interactions: With mobile-first design, there is a focus on touch-friendly interactions, as mobile devices primarily rely on touchscreens. This means larger buttons, easy-to-use navigation, and other user interface elements that are designed with touch gestures in mind.

In summary, mobile-first design is a user-centric approach that acknowledges the increasing dominance of mobile devices in internet usage. By prioritizing mobile users, it ensures that the website or application provides a good experience on smaller screens while still catering to larger screens with additional features and optimizations.



2. Media-queries
Media queries are a fundamental component of responsive web design. They are CSS (Cascading Style Sheets) features that allow web developers to apply different styles and layouts based on the characteristics of the device or screen on which a website is being viewed. Media queries enable websites to adapt their presentation and design to different screen sizes, resolutions, and orientations, providing a consistent and user-friendly experience across various devices.

The syntax of a media query is as follows:
@media media-type and (media-feature) {
  /* CSS rules to apply when the media query conditions are met */
}

Here's a breakdown of the different parts of a media query:
@media: This is the keyword that starts the media query declaration.

media-type: This is an optional part that defines the type of media being targeted. For responsive web design, it is usually "screen" (for devices with screens) or "all" (applies to all media types).

media-feature: This is the condition that must be met for the media query to be applied. Media features include characteristics like screen width, device height, orientation (landscape or portrait), resolution, and more.

When the conditions specified in the media query are met, the CSS rules inside the media query block will be applied. This allows developers to modify styles, layout, and other design elements to suit different screen sizes and devices.


Here's an example of a media query that adjusts the font size based on the screen width:
body {
  font-size: 16px; /* Default font size for all devices */

  @media screen and (max-width: 768px) {
    font-size: 14px; /* Font size for devices with a maximum width of 768px or less */
  }
}

In this example, the default font size is 16 pixels for all devices. However, when the screen width is 768 pixels or less (typically smaller devices like smartphones and tablets), the font size is reduced to 14 pixels to improve readability on smaller screens.

Media queries are essential for responsive design because they allow websites to adapt dynamically to various devices, making it possible to provide an optimal user experience regardless of the user's screen size or device type.



3. Sizes to use for responsive web design
In responsive web design, using appropriate sizes for various elements is crucial to ensure that the website adapts and displays correctly on different devices and screen sizes. Here are some key sizes and considerations to use in responsive web design:

Viewport Width (vw): This unit represents a percentage of the viewport's width. For example, 1vw is equal to 1% of the viewport width. It is commonly used to size elements relative to the screen width. For instance, width: 50vw; will set the element's width to 50% of the viewport width.

Viewport Height (vh): Similar to viewport width, this unit represents a percentage of the viewport's height. It is often used to control the height of elements based on the screen height. For example, height: 100vh; will set the element's height to cover the entire viewport height.

Minimum and Maximum Widths (min-width, max-width): Media queries often use these properties to define specific CSS rules for different screen sizes. For example:
/* Styles for screens with a minimum width of 768px */
@media (min-width: 768px) {
  /* CSS rules here */
}

/* Styles for screens with a maximum width of 1200px */
@media (max-width: 1200px) {
  /* CSS rules here */
}


Em and Rem Units: These units are relative to the font size of the parent or root element, respectively. They are useful for creating scalable and flexible designs. Em units are relative to the font size of the element, while rem units are relative to the root (html) font size.

Percentage Units: Percentage values are often used to create flexible layouts that adapt to the available space. For example, setting an element's width to width: 50%; will make it occupy 50% of its parent's width.

Pixel Units: While using relative units is generally recommended for responsive design, sometimes specifying fixed pixel values can be appropriate for certain elements that need to maintain a specific size regardless of the screen size.

Fluid Images: Images in responsive design should be set to max-width: 100%; to ensure they scale appropriately to fit their container without overflowing or causing layout issues on smaller screens.

Remember that responsive web design is about creating a fluid and adaptable layout that accommodates various devices and screen sizes. It's essential to test your design on multiple devices and screen resolutions to ensure it behaves as expected and provides a seamless user experience across the board.



4. How to make a website responsive
Making a website responsive involves applying various design and development techniques to ensure that the site adapts and looks good on different devices and screen sizes. Here are the key steps to make a website responsive:

Plan your Design: Start by planning the overall layout and design of your website. Consider the essential elements and content you want to include and how they will rearrange or stack on smaller screens. Sketch or wireframe your design to visualize the responsive layout.

Use Responsive Frameworks or Grid Systems: Consider using CSS frameworks like Bootstrap or Foundation that provide pre-built responsive grid systems and components. These frameworks help streamline the responsive design process and ensure consistency across various devices.

Use Mobile-First Approach: As mentioned earlier, adopt a mobile-first approach by designing for small screens first and then enhancing the layout for larger screens. This ensures a solid foundation for the mobile experience.

Media Queries: Employ media queries to apply different CSS styles based on screen size. Media queries allow you to define specific rules for various screen widths, heights, orientations, and resolutions.

Flexible Units: Use relative units like vw, vh, em, rem, and percentages instead of fixed pixel values for widths, heights, and margins. This allows elements to scale and adapt to different screen sizes.

Breakpoints: Identify specific breakpoints in your design where the layout needs to change to accommodate different screen sizes. Common breakpoints include those for smartphones, tablets, and desktops.

Images and Media: Use max-width: 100%; for images and videos to ensure they scale proportionally and fit within their containers without overflowing on smaller screens.

Font and Text Size: Use relative units for font sizes (em, rem, %) to ensure text remains readable and adjusts based on the user's device.

Test and Optimize: Regularly test your website on various devices and screen sizes to ensure it looks and functions as intended. Address any layout issues or inconsistencies that arise during testing.

Performance Optimization: Consider optimizing your website's performance to ensure fast load times on all devices. Compress images, minify CSS and JavaScript, and implement other performance best practices.

Accessibility: Keep accessibility in mind while designing and developing your website. Ensure that users with disabilities can navigate and use your site effectively.

User Testing: Conduct user testing to gather feedback from real users on different devices. This feedback can help you identify any usability issues and make necessary improvements.

By following these steps and staying committed to delivering a smooth and user-friendly experience across devices, you can create a responsive website that meets the needs of all your users, regardless of the screen size they use to access your site.



5. The differences between responsive and adaptive design
Responsive design and adaptive design are both approaches to creating websites that cater to different screen sizes and devices, but they differ in their methods and philosophies. Here are the key differences between responsive and adaptive design:

Fluidity vs. Fixed Layouts:

Responsive Design: Responsive design uses fluid grids and flexible elements that automatically adjust and scale based on the screen size. The layout adapts smoothly to fit any screen resolution, ensuring a consistent user experience across various devices.
Adaptive Design: Adaptive design uses fixed layout sizes designed for specific screen resolutions or devices. Instead of fluidly adjusting to different screens, adaptive websites have predefined layouts for different screen sizes, and the appropriate layout is selected based on the user's device.


Approach to Coding:

Responsive Design: In responsive design, a single set of HTML and CSS code is used for all devices. Media queries are commonly used to apply different styles based on screen characteristics such as width, height, and orientation.
Adaptive Design: Adaptive design often requires creating multiple versions of the website, each tailored to different screen sizes or devices. The server detects the user's device and serves the appropriate version of the website.


Flexibility vs. Targeted Optimization:

Responsive Design: Responsive websites are highly flexible and can adapt to any screen size, regardless of whether it is a common or niche device. They provide a consistent experience across a wide range of devices.
Adaptive Design: Adaptive websites are optimized for specific devices or screen sizes. This allows for more targeted optimization and customization for certain popular devices but may not provide the same level of flexibility as responsive design.


Loading Time:

Responsive Design: Responsive websites may load slightly more CSS and JavaScript because they need to handle various screen sizes and orientations. However, advances in browser caching and mobile performance optimizations have minimized this difference.
Adaptive Design: Adaptive websites can potentially load faster because they serve a version optimized for a specific device, reducing the amount of CSS and JavaScript needed.


Maintenance and Updates:

Responsive Design: Since responsive websites use a single codebase, they are often easier to maintain and update. Changes are applied universally across all devices.
Adaptive Design: Adaptive websites may require separate maintenance for each version, leading to more effort and resources needed for updates.


Future-Proofing:

Responsive Design: Responsive websites are better equipped to handle new and emerging devices without requiring significant modifications, as they are designed to be flexible and adaptable.
Adaptive Design: Adaptive websites might require updates or new versions to support newer devices, as they are optimized for specific resolutions and may not accommodate new screen sizes automatically.


In summary, responsive design provides a more fluid and universally adaptable experience, while adaptive design offers targeted optimization for specific devices or screen sizes. The choice between the two depends on the project's goals, target audience, and the resources available for development and maintenance.



6. CSS units that are used to make elements flexible
CSS units that are used to make elements flexible and responsive to different screen sizes are known as relative units. These units are based on various factors, such as the size of the viewport, the font size of the parent element, or the root (html) font size. Relative units ensure that elements scale proportionally and adapt to different devices, making the design more flexible. Here are some commonly used relative units:

Viewport Width (vw): Represents a percentage of the viewport's width. For example, 1vw is equal to 1% of the viewport width. It is often used for element sizing based on the screen width.

Viewport Height (vh): Similar to viewport width, this unit represents a percentage of the viewport's height. It is used to control the height of elements based on the screen height.


Relative Font Units (em and rem):

em: Represents the font size of the current element's parent. For example, if an element has font-size: 1.5em;, it means the font size is 1.5 times the font size of its parent element.
rem: Represents the font size of the root (html) element. It ensures consistency across the entire document. For example, font-size: 1.2rem; means the font size is 1.2 times the root font size.


Percentage Units (%): Percentage values are used for element sizing and positioning relative to their parent container. For example, width: 50%; sets the element's width to 50% of its parent container's width.


Using these relative units instead of fixed units like pixels (px) allows elements to adapt and resize based on the user's device and screen size. This flexibility is essential for creating responsive web designs that look good on various devices, from mobile phones to large desktop screens.



Requirements
Allowed editors: vi, vim, emacs
A README.md at the root of the project directory is mandatory
HTML and CSS have been rendered on Chrome 78 or more.

