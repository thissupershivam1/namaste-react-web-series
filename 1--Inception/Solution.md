## Namaste React Course by Akshay Saini
# _Chapter 01 - Inception_


## Theory -


## Q: What is `Emmet`?
A: Emmet is a coding productivity tool or plugin that helps developers write HTML and CSS code more quickly and efficiently. It is primarily used in web development environments and text editors. Emmet provides a shorthand syntax for writing repetitive code structures, allowing developers to generate HTML and CSS code with minimal keystrokes.

## Q:Difference between a `Library and Framework`?
A: The library and framework  Library:

A library is a collection of pre-written code or modules that developers can use to perform specific tasks or access certain functionality.
Libraries are typically focused on providing specific functionality or solving specific problems. They offer a set of functions, classes, or modules that developers can use in their applications.
Developers have more control over the overall structure and flow of their application when using libraries. They can selectively use the parts of the library that are needed and integrate them into their codebase.
Libraries are usually designed to be reusable and can be incorporated into different projects.
Examples of libraries include jQuery (JavaScript library), NumPy (Python library for numerical computations), and Retrofit (Java library for networking operations).
Framework:

A framework is a more comprehensive and structured software development environment that provides a foundation for building applications.
Frameworks offer a set of tools, libraries, and guidelines that dictate the overall architecture and flow of an application.
Developers build their applications within the framework's structure and adhere to its rules and conventions.
Frameworks often provide a specific approach or methodology for solving a particular type of problem. They include predefined components and modules that handle common tasks such as handling requests, managing databases, or rendering user interfaces.
Frameworks often require developers to follow specific patterns or paradigms, such as model-view-controller (MVC), to ensure consistency and maintainability.
Examples of frameworks include Ruby on Rails (web application framework), Django (Python web framework), and Angular (JavaScript front-end framework).

##Q: What is `CDN`? Why do we `use` it?
A: CDN stands for Content Delivery Network. It is a network of servers distributed geographically in different locations worldwide. The primary purpose of a CDN is to deliver web content, such as images, CSS files, JavaScript files, videos, and other static assets, to users more efficiently and with improved performance.

When you use a CDN, instead of serving your web content directly from your own server, the content is cached and stored on multiple servers located in different geographic regions. When a user requests your content, the CDN automatically serves it from the server that is closest to the user's location. This helps reduce latency and improves the overall loading speed of your web pages.

Here are some key reasons why we use CDNs:

1. Improved Performance: CDNs have servers strategically placed across the globe, allowing them to serve content from the nearest server to the user. This reduces the distance and network hops required to retrieve content, resulting in faster loading times.

2. Scalability: CDNs can handle high volumes of traffic and distribute it across multiple servers. This helps in scaling your website's performance and handling traffic spikes without overloading your origin server.

3. Global Reach: CDNs have a global network presence, which means your content can be delivered to users all around the world quickly, regardless of their geographical location.

4. Reducing Bandwidth Costs: CDNs can help reduce bandwidth consumption on your origin server by caching and serving content from their distributed servers. This can lower your server costs, especially if you have high traffic or serve large files.

5. Improved Reliability: CDNs provide redundancy and load balancing capabilities, ensuring high availability of your content. If one server goes down, the CDN can automatically route requests to another available server.

6. DDoS Mitigation: CDNs often have built-in DDoS (Distributed Denial of Service) protection mechanisms, which can help mitigate and absorb malicious traffic, preventing attacks from overwhelming your servers.

Overall, using a CDN can significantly enhance the performance, reliability, and scalability of your website or web application, resulting in a better user experience and improved efficiency of content delivery.

## Q: Why is `React known as React`?
A: React, the JavaScript library for building user interfaces, gets its name from its core concept of reactive updates. The name "React" reflects the primary philosophy behind the library, which is to efficiently update and render user interfaces in response to changes in data or state.

React introduces a concept called the "Virtual DOM" (Document Object Model), which is an in-memory representation of the actual DOM. When changes occur in the application's data or state, React efficiently calculates the minimal set of updates needed to bring the Virtual DOM in sync with the actual DOM. This process is known as "reconciliation."

React's efficient reconciliation process allows it to minimize the number of actual updates to the DOM, which can be costly in terms of performance. By only updating the necessary parts of the DOM, React significantly improves the speed and efficiency of rendering user interfaces.

The name "React" signifies the library's ability to reactively and efficiently handle updates to the UI by leveraging the Virtual DOM. It emphasizes React's core philosophy of focusing on updates and rendering, making it one of the key features that set React apart from other UI frameworks and libraries.

## Q: What is `crossorigin in script tag`?
A: The `crossorigin` attribute in the `<script>` tag is used to specify how the browser should handle cross-origin requests when loading JavaScript files. Cross-origin requests are requests made from one domain (origin) to another domain.

When a JavaScript file is loaded from a different domain, the browser's default security policy, known as the "Same-Origin Policy," restricts access to the response unless the server explicitly allows it. This policy is in place to protect the integrity and security of web content.

The `crossorigin` attribute has two possible values:

1. `anonymous`: This is the default value if the attribute is present but not specified. When `crossorigin="anonymous"` is set, the browser makes the request for the JavaScript file without including any credentials (such as cookies or HTTP authentication). This is suitable when the server hosting the JavaScript file is configured to allow cross-origin requests from any origin.

2. `use-credentials`: When `crossorigin="use-credentials"` is set, the browser includes any relevant credentials (such as cookies or HTTP authentication) when making the cross-origin request. This is used when the server requires authentication or specific credentials for accessing the JavaScript file.

The `crossorigin` attribute is typically used when loading external JavaScript files from a different domain, especially when utilizing features like CORS (Cross-Origin Resource Sharing). It allows developers to control how the browser handles cross-origin requests and helps ensure security and proper access to the requested JavaScript resources.

## Q: What is difference between `React and ReactDOM`?
A:  React is the core library for building user interfaces in a declarative and component-based manner, managing component lifecycle, state, and rendering updates. ReactDOM, on the other hand, is a package that specifically deals with rendering React components into the browser's DOM and provides methods for manipulating the DOM.

## Q: What is difference between `react.development.js` and `react.production.js` files via CDN?
A: The difference between `react.development.js` and `react.production.js` files lies in the optimizations and features enabled in each version. These files serve different purposes depending on the development or production environment.

1. `react.development.js`:
   - This file is intended for development purposes.
   - It contains the full, unminified version of the React library.
   - It includes additional warnings and error messages that help with debugging and development.
   - The file size is larger compared to the production version.
   - It provides a more informative and verbose output, aiding developers in identifying and resolving issues during development.

2. `react.production.js`:
   - This file is optimized for production environments.
   - It is minified and stripped of any unnecessary code or comments to reduce file size and improve performance.
   - Warnings and error messages are minimized or removed entirely to reduce verbosity and improve production runtime efficiency.
   - The file size is smaller compared to the development version, which helps optimize the loading and parsing time for users.
   - It is intended for use in production environments where performance and file size are crucial factors.

When using React via a CDN, you can choose to include either `react.development.js` or `react.production.js` based on your specific needs. During development, it is recommended to use `react.development.js` to take advantage of the debugging capabilities and helpful warnings. In production, however, it is best to use `react.production.js` for optimal performance and reduced file size.

Note that these differences apply to React specifically and similar distinctions between development and production versions can exist for other libraries or frameworks.

## Q: What is `async and defer`?
A: `async` and `defer` are attributes that can be added to `<script>` tags in HTML to control how scripts are loaded and executed. They are used to optimize the loading and execution of external JavaScript files. Here's an explanation of each attribute:

1. `async`:
   - When the `async` attribute is added to a `<script>` tag, it indicates to the browser that the script can be loaded asynchronously. This means that the script will be fetched from the server in parallel with the HTML parsing and rendering process.
   - When a browser encounters a script with the `async` attribute, it will continue parsing and rendering the HTML content without waiting for the script to be fully downloaded and executed.
   - Once the script is downloaded, it will be executed as soon as possible, potentially interrupting the HTML parsing process.
   - It is important to note that the order of script execution is not guaranteed when using `async` for multiple scripts. Whichever script finishes downloading first will be executed first, regardless of their original order in the HTML.
   - The `async` attribute is suitable for scripts that do not have dependencies on other scripts or on the DOM being fully loaded.

2. `defer`:
   - When the `defer` attribute is added to a `<script>` tag, it indicates to the browser that the script should be deferred and executed after the HTML parsing is complete.
   - Similar to `async`, a script with the `defer` attribute is fetched in parallel with the HTML parsing process.
   - However, unlike `async`, the `defer` script will only be executed after the HTML parsing is finished, just before the `DOMContentLoaded` event is fired.
   - Scripts with the `defer` attribute will be executed in the order they appear in the HTML, ensuring that scripts relying on other scripts or the DOM being available can be executed correctly.
   - The `defer` attribute is typically used when scripts have dependencies on other scripts or need access to the DOM structure.

In summary, `async` and `defer` are attributes that control the loading and execution behavior of external JavaScript files. `async` allows scripts to be loaded asynchronously and executed as soon as they are downloaded, potentially interrupting HTML parsing. `defer` allows scripts to be deferred until after HTML parsing is complete, ensuring proper script execution order and dependencies.
