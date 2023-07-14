0x01. Developer tools
HTML
CSS
Front-end


Resources
Read or watch:

Chrome DevTools | Tools for Web Developers | Google Developers
Introduction | Down and Dirty with Chrome Developer Tools
Firefox Developer Tools | MDN
Dev Tips - Developer Tips by Umar Hansa
Get Started With Viewing And Changing CSS | Tools for Web Developers
Keeping it simple with the JavaScript console - LogRocket Blog
Inspect Network Activity - Chrome DevTools 101



Requirements
General
A README.md file, at the root of the folder of the project, is mandatory
Use the newest version of Google Chrome browser (78.0.3904.70 or later).
Screenshots can be taken via the OS, not necessary via the DevTools. These screenshots are used to see how and where you are doing/playing with the DevTools.



GENERAL
1. What Developer Tools in your browser are
Developer tools in a web browser are a set of built-in utilities and features designed to assist web developers in debugging, testing, and analyzing web pages and web applications. These tools are typically accessed through the browser's menu or by using specific keyboard shortcuts. Here are some commonly found developer tools in modern web browsers:

Inspector: The inspector allows you to examine and modify the HTML and CSS of a web page. It lets you inspect elements, view their styles, and make real-time changes to see how they affect the page.

Console: The console provides a JavaScript console where you can execute JavaScript code, log messages, debug errors, and monitor network requests. It's a powerful tool for testing and troubleshooting JavaScript code.

Network Monitor: The network monitor tracks and displays all network requests made by a web page, including HTTP requests, responses, headers, and timings. It helps you analyze the performance and behavior of your web application.

Debugger: The debugger allows you to set breakpoints and step through JavaScript code to find and fix bugs. It provides features like inspecting variables, call stacks, and monitoring the flow of execution.

Performance Profiler: The performance profiler helps you identify performance bottlenecks in your web application. It records and analyzes the performance of your code, highlighting areas where optimizations can be made.

Application Storage: This tool allows you to view and manage cookies, local storage, session storage, and other types of client-side storage used by web applications.

Security Auditing: Browsers also provide security auditing tools to help identify potential security vulnerabilities in your web application, such as insecure content, mixed content warnings, or insecure password fields.

Mobile Emulation: Many modern browsers offer mobile emulation features, allowing you to simulate the behavior and appearance of your web application on different mobile devices.


2. How to open the Developer Tools on Chrome, Firefox, Safari, and Edge.
To open the Developer Tools in popular web browsers, follow the instructions below:

Google Chrome:

Right-click anywhere on a web page and select "Inspect" from the context menu.
Alternatively, you can use the keyboard shortcuts:
Windows and Linux: Press Ctrl + Shift + I.
macOS: Press Command + Option + I.
Mozilla Firefox:

Right-click anywhere on a web page and select "Inspect Element" from the context menu.
Alternatively, you can use the keyboard shortcuts:
Windows and Linux: Press Ctrl + Shift + I.
macOS: Press Command + Option + I.
Safari:

Go to Safari's menu and select "Preferences."
In the Preferences window, click on the "Advanced" tab.
Enable the "Show Develop menu in menu bar" option.
Once the Develop menu appears in the menu bar, click on it and select "Show Web Inspector."
Alternatively, you can use the keyboard shortcuts:
macOS: Press Command + Option + I.
Microsoft Edge:

Right-click anywhere on a web page and select "Inspect" from the context menu.
Alternatively, you can use the keyboard shortcuts:
Windows: Press Ctrl + Shift + I.
macOS: Press Command + Option + I.



3. How to use the elements tab to edit HTML and CSS
To use the Elements tab in the browser's developer tools to edit HTML and CSS, follow these steps:

Open the developer tools in your browser using one of the methods mentioned earlier (e.g., right-click and select "Inspect" or press the respective keyboard shortcut).

In the developer tools window, locate and click on the "Elements" or "Inspector" tab. It is typically represented by an icon resembling a box or an arrow pointing at a box.

The Elements tab will display the HTML structure of the currently loaded web page. You can navigate and explore the elements by expanding or collapsing the HTML tree.

To edit an HTML element, locate the element in the Elements tab and double-click on the element or its attributes. This will enable an editable field where you can modify the HTML code. Press Enter to apply the changes.

To modify CSS styles, locate the desired element in the Elements tab. On the right-hand side, you will see the "Styles" or "Computed" panel. Here, you can view and edit the CSS styles applied to the selected element.

To add a new CSS property, click on the "+" icon next to the relevant CSS selector and enter the property and value.
To modify an existing CSS property, click on the property value and edit it.
Press Enter to apply the changes.
As you make changes to the HTML or CSS, you will usually see them reflected live in the browser. This allows you to experiment, preview, and fine-tune the appearance and layout of the web page.

If needed, you can also disable or enable CSS rules by toggling the checkboxes next to each rule in the "Styles" panel. This can help in isolating and troubleshooting specific styles.

Remember that any changes you make in the developer tools are temporary and only affect your local browser session. When you reload the page or navigate to a different URL, the changes will be reverted.

Using the Elements tab in the browser's developer tools gives you the ability to inspect, modify, and experiment with the HTML structure and CSS styles of a web page, providing a powerful environment for web development and debugging.



4. How to audit a page according to the tips suggested by Lighthouse
To audit a web page using Lighthouse, a tool for performance analysis and best practices, you can follow these steps:

Open Google Chrome, as Lighthouse is integrated into the Chrome browser's developer tools.

Visit the web page you want to audit.

Open the Chrome Developer Tools. You can do this by right-clicking anywhere on the page and selecting "Inspect" or by using the keyboard shortcut: Ctrl + Shift + I (Windows/Linux) or Command + Option + I (macOS).

In the developer tools panel that opens, you'll see a row of tabs at the top. Click on the "Lighthouse" tab.

The Lighthouse panel provides different audit categories. By default, it runs audits for Performance, Accessibility, Best Practices, and SEO. You can customize which categories to include by clicking on "Settings" or selecting the checkboxes for the desired categories.

To start the audit, click on the "Generate report" button. Lighthouse will begin analyzing the web page based on the selected categories.

After the audit completes, Lighthouse will display a detailed report with scores, recommendations, and additional information for each category. It provides insights into areas where your web page can be improved to enhance performance, accessibility, best practices, and search engine optimization.

You can expand each category to see a breakdown of specific recommendations and their impact on the page's performance. Lighthouse provides explanations and actionable advice to help you address any identified issues.

Review the audit results and prioritize the suggested improvements based on their impact and feasibility. Consider making the necessary changes to optimize your web page accordingly.

Lighthouse is a powerful tool for assessing and optimizing web page performance. It offers valuable insights and recommendations to help you enhance various aspects of your website. By following the tips and suggestions provided in the Lighthouse audit report, you can work towards creating a more performant, accessible, and user-friendly web experience.



5. How to create and run snippets on a page
To create and run snippets on a web page, you can use the browser's developer tools. Here's a step-by-step guide on how to do it:

Open the web page where you want to create and run the snippet.

Open the developer tools in your browser. You can typically do this by right-clicking on the page and selecting "Inspect" or using the keyboard shortcut: Ctrl + Shift + I (Windows/Linux) or Command + Option + I (macOS).

In the developer tools panel, find and select the "Console" tab. This is where you can enter and run JavaScript code snippets.

In the console, you can start typing your JavaScript code directly. However, to create a snippet for future use, you can click on the "Sources" or "Snippets" tab, depending on the browser.

In the "Sources" or "Snippets" tab, you'll find an area to manage and create snippets. Locate the "New Snippet" or "+" button and click on it to create a new snippet.

A code editor will appear where you can write your JavaScript code. Enter the desired code for your snippet in the editor.

Give your snippet a meaningful name by entering it in the designated field or renaming the default name.

Once you have written your snippet, you can save it by clicking the "Save" or "Ctrl + S" (Windows/Linux) or "Command + S" (macOS) shortcut. Note that the specific save process may vary slightly depending on the browser.

After saving the snippet, you can close the snippet editor.

To run the snippet, go back to the "Console" tab in the developer tools panel.

In the console, you can call and execute your snippet by typing its name followed by parentheses. For example, if your snippet is named "mySnippet", type "mySnippet()" and press Enter to run it.

The snippet will execute, and you'll see the output or any relevant results displayed in the console. You can also interact with the page and manipulate its elements using the JavaScript code within the snippet.

By creating and running snippets, you can test and experiment with JavaScript code on a web page, making it a convenient way to prototype and debug code snippets without permanently modifying the page or website. Remember that snippets are specific to the current browser session and do not persist beyond it.




6. How to get information about files and server configurations
To obtain information about files and server configurations, you can use various methods and tools depending on your specific requirements and access permissions. Here are a few common approaches:

File System Inspection:

Use FTP (File Transfer Protocol) or SFTP (SSH File Transfer Protocol) clients to connect to the server and browse the file system, accessing files and directories.
Utilize command-line tools like ls, cd, and cat (or their equivalents on Windows) to navigate and view file contents if you have access to a command-line interface or SSH (Secure Shell) access.
HTTP Requests:

Use a web browser or tools like cURL or Postman to send HTTP requests to the server.
Inspect the response headers to gather information about the server, such as the web server software (e.g., Apache, Nginx), version, and other server-specific configurations.
Server-Side Languages:

If you have access to server-side languages like PHP, Python, or Node.js, you can create scripts to fetch server information programmatically.
For example, in PHP, you can use the $_SERVER superglobal array to access server-related information like $_SERVER['SERVER_SOFTWARE'] to get the web server software.
WHOIS Lookup:

Perform a WHOIS lookup using online WHOIS services or WHOIS command-line tools to gather information about the domain, including registrar details, domain status, and expiration date.
Security Scanners and Vulnerability Assessment Tools:

Tools like Nikto, OpenVAS, or Nessus can scan a server for potential vulnerabilities and provide detailed reports on server configurations, software versions, and security issues.
Built-in Server Info Pages:

Some web servers may have default pages or endpoints that provide server information or configurations. For example, accessing /server-status or /phpinfo.php on Apache servers may reveal server and PHP configuration details.
Note that the availability and access to certain methods and tools might depend on your role, permissions, and the specific server environment you are working with. It's important to ensure you have appropriate authorization and adhere to security practices while accessing and gathering information about files and server configurations.




8. How to block requests
To block requests, you can use different approaches depending on your requirements and the level of control you have over the network or application. Here are a few methods you can consider:

Firewall or Network-level Blocking:

Configure network-level firewalls or use specialized firewall software to block requests at the network level. This approach allows you to block specific IP addresses, ports, or entire protocols.
This method is typically managed by network administrators or IT departments and may require access to network infrastructure.
Browser Extensions:

Install browser extensions that allow you to block requests from within your browser. These extensions often provide options to block specific URLs, domains, or request types.
Examples of such extensions include uBlock Origin, AdBlock Plus, or NoScript.
Web Server Configuration:

Modify the configuration of your web server (e.g., Apache, Nginx) to block requests. This can be done by configuring rules in the server's configuration files.
For example, using Apache's .htaccess file or Nginx's location blocks, you can define rules to block specific URLs or IP addresses.
Content Security Policy (CSP):

Implement a Content Security Policy in your web application. CSP allows you to define a policy that specifies what types of content, such as scripts, stylesheets, or images, are allowed to be loaded by the browser.
By configuring the CSP, you can block requests to external domains or restrict the execution of inline scripts.
Proxy Server:

Set up a proxy server to intercept and filter requests. Proxy servers act as intermediaries between clients and servers, allowing you to inspect and modify incoming and outgoing requests.
With a proxy server, you can block or manipulate requests based on various criteria, such as URL patterns, headers, or payloads.
It's important to note that blocking requests should be done carefully and with consideration for the impact on the system or users. Always ensure you have the necessary authorization and adhere to security best practices when implementing request blocking mechanisms.




9. How to know how much JavaScript or CSS is used on a page
To determine how much JavaScript or CSS is used on a web page, you can use the browser's developer tools. Here's how you can find that information:

Open the web page you want to analyze in your preferred browser.

Open the browser's developer tools. You can usually access them by right-clicking on the page and selecting "Inspect" or using the keyboard shortcut: Ctrl + Shift + I (Windows/Linux) or Command + Option + I (macOS).

In the developer tools panel, navigate to the "Network" or "Performance" tab. The name may vary depending on the browser.

Refresh the web page to start recording network activity.

Look for the columns related to file sizes or resources loaded, such as "Size," "Content Size," or "Transferred Size."

Sort the network requests by file size to identify the largest files first. Typically, JavaScript and CSS files have file extensions like ".js" and ".css," respectively.

Review the list of files to identify the JavaScript or CSS resources.

For JavaScript files, pay attention to files with larger sizes, as they tend to indicate more extensive JavaScript usage.
For CSS files, consider both the file sizes and the number of selectors and styles defined within them.
By analyzing the size and number of JavaScript and CSS files, you can get a rough estimate of how much JavaScript and CSS is used on the web page.

Keep in mind that this method provides a high-level overview and does not provide detailed insights into the specific usage or complexity of the JavaScript or CSS code. It's also worth noting that modern web pages often utilize minification and compression techniques, which can reduce the file sizes during production to improve performance.

For a more comprehensive analysis of JavaScript or CSS usage, you can explore dedicated tools and techniques like code profiling, bundling analysis, or using specialized web performance analysis tools like Lighthouse or WebPageTest.




10. How to detect 404 issues
To detect 404 issues on a website, you can use various methods and tools. Here are a few approaches you can take:

Manual Inspection:

Navigate through the website manually, visiting different pages and checking for any 404 error messages or broken links.
Look for any links that lead to non-existent pages or resources, which may indicate 404 issues.
Inspect the browser's network requests and check for HTTP status codes, specifically 404 (Not Found) responses.
Browser Developer Tools:

Open the browser's developer tools by right-clicking on the page and selecting "Inspect" or using the keyboard shortcut: Ctrl + Shift + I (Windows/Linux) or Command + Option + I (macOS).
Go to the "Network" tab in the developer tools panel.
Refresh the page or navigate to different sections of the website.
Look for any requests that return a 404 status code (or other error codes) in the network log.
Check the "Status" or "Status Text" column to identify the 404 errors.
Crawling Tools:

Use website crawling tools like Screaming Frog, Xenu's Link Sleuth, or DeepCrawl.
These tools crawl your website and identify broken links, including 404 errors.
They provide detailed reports on broken links, their locations, and other relevant information.
Google Search Console:

If your website is registered with Google Search Console (formerly known as Google Webmaster Tools), it provides a "Coverage" report that highlights crawling and indexing issues, including 404 errors.
Access the "Coverage" section in Google Search Console to identify URLs that return 404 status codes.
Online Link Checkers:

Use online tools like Broken Link Check, W3C Link Checker, or Dead Link Checker.
These tools allow you to enter your website's URL and scan for broken links, including 404 errors.
They provide reports with the list of broken links, their locations, and other relevant details.
By using a combination of manual inspection, browser developer tools, crawling tools, and online link checkers, you can effectively detect 404 issues on a website. Regularly monitoring and fixing these errors will help improve user experience, search engine optimization, and overall website health.





11. How to move elements on a webpage
To move elements on a webpage, you can use JavaScript or CSS techniques to manipulate the position or layout of the elements. Here are a few common methods:

CSS Positioning:

Use CSS positioning properties like position: absolute, position: relative, or position: fixed to control the position of elements on the page.
Set the top, bottom, left, and right properties to specify the desired offset from a reference point or the edges of the containing element.
CSS Flexbox:

Utilize CSS Flexbox to create flexible layouts and easily move elements within a container.
Apply the display: flex property to the container element and use the order property to change the order in which the elements appear.
CSS Grid:

Implement CSS Grid to create grid-based layouts and move elements within the grid cells.
Define the grid container with the display: grid property and use grid-specific properties like grid-row and grid-column to position and move elements within the grid.
JavaScript Manipulation:

Use JavaScript to dynamically move elements on the page by manipulating their properties or directly modifying the DOM.
Access the element using JavaScript methods like getElementById, querySelector, or getElementsByClassName, and then modify properties like style.top, style.left, style.transform, or style.order to change their position or order.
Drag and Drop:

Implement drag and drop functionality using JavaScript frameworks or libraries like jQuery UI, interact.js, or HTML5 Drag and Drop API.
Allow users to drag and drop elements within a designated area or across the page to change their position dynamically.
Remember to consider the overall design and user experience when moving elements on a webpage. Ensure that the layout remains visually appealing and functional for users across different devices and screen sizes. Test and validate your changes in multiple browsers to ensure consistent behavior.



In this project, you will analyze this website https://dev-tools.alx-tools.com/.
