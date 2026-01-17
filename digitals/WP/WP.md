 
 # Web Programming & Scripting Languages
 
 Web Programming & Scripting Languages
 
 Scripting Language
 Scripts are programs just like any other programming language. They can execute on the client-side or on the server-side.
 
 Scripting languages do not require a compilation step; instead, they are interpreted.
 
 ## Types of Scripting Languages
 
 Types of Scripting Languages
 
 ```mermaid
 graph TD
     A[Scripting Languages] --> B[Client-Side Scripting]
     A --> C[Server-Side Scripting]
     B --> D[Processed on Browser/Local Computer]
     C --> E[Runs on Server]
     D --> F[Example: JavaScript]
     E --> G[Example: PHP]
 ```
 
 1. Client-Side Scripting Language
 
 Client-side scripts are processed on the browser or local computer. They allow changing the contents of the web page dynamically.
 
 Functions:
 
 - Interact with temporary storage.
 - Make interactive web pages.
 - Interact with local storage.
 - Send requests for data to the server.
 - Send requests to the server properly.
 - Work as an interface between the server and users.
 
 2. Server-Side Scripting Language
 
 It is a script that runs on a server, dealing with the generation of web page content.
 
 Functions:
 
 - Querying the database.
 - Operations over the database.
 - Access/Write a file on the server.
 - Interact with other servers.
 - Structuring web applications.
 - Processing user input.
 
 ## HTML (HyperText Markup Language)
 
 HTML is the standard markup language for creating web pages. It provides the structural foundation of websites by defining elements such as headings, paragraphs, links, images, forms, and multimedia content.
 
 Key Characteristics:
 
 - Markup Language
 - Platform Independent
 - Foundation of the Web
 - Static Content
 
 Why is HTML Essential Before PHP?
 
 - Output Layer: PHP often outputs HTML.
 - Form Integration: PHP processes HTML forms.
 - Template Structure: HTML provides the skeleton.
 - Client-Server Model: HTML acts as the client-side interface.
 
 HTML Elements and Tags
 
 HTML tags are keywords enclosed in angle brackets < >.
 
 Paired Tags (Container Tags): Most HTML tags come in pairs with opening and closing tags.
 
 Example:
 
 ```html
 <p> ... </p>
 ```
 
 Self-Closing Tags (Empty Tags): Do not require a closing tag.
 
 Example:
 
 ```html
 <img src="...">, <br>, <hr>
 ```
 
 Block-level vs Inline Elements
 
 Type | Description | Examples
 ---|---|---
 Block-level Elements | Always start on a new line and take up the full width available. | <div>, <p>, <table>, <h1>
 Inline Elements | Do not start on a new line and only take up as much width as necessary. | <span>, <a>, <strong>, <img>
 
 Text Content and Formatting
 Headings:
 
 ```html
 <h1>Heading 1</h1>
 <h2>Heading 2</h2>
 ```
 
 Hyperlinks:
 
 ```html
 <a href="https://www.google.com" target="_blank">Visit Google</a>
 ```
 
 Images:
 
 ```html
 <img src="image.jpg" alt="Description of Image">
 ```
 
 Lists:
 
 Unordered Lists (Bullet Points):
 
 ```html
 <ul>
     <li>Item 1</li>
     <li>Item 2</li>
 </ul>
 ```
 
 Ordered Lists (Numbered):
 
 ```html
 <ol>
     <li>First Item</li>
     <li>Second Item</li>
 </ol>
 ```
 
 Tables:
 
 ```html
 <table border="1">
     <tr>
         <th>Header 1</th>
         <th>Header 2</th>
     </tr>
     <tr>
         <td>Data 1</td>
         <td>Data 2</td>
     </tr>
 </table>
 ```
 
 HTML Forms
 Forms are the primary method for collecting user input on websites. In PHP, this input is processed on the server.
 
 Basic Syntax:
 
 ```html
 <form action="process.php" method="POST">
     <!-- Form elements go here -->
 </form>
 ```
 
 Form Attributes:
 
 action: URL where form data is sent.
 method: HTTP method for sending data (GET or POST).
 name: Form identifier.
 target: Where to display the response (e.g., _blank).
 enctype: Encoding type (Essential for file uploads: multipart/form-data).
 
 Form Input Types
 Input TypeSyntax ExampleDescriptionText<input type="text" name="username" placeholder="Enter username">Single line text.Password<input type="password" name="password">Hides characters.Email<input type="email" name="email">Validates email format.Number<input type="number" name="age" min="1" max="100">Numeric input.Telephone<input type="tel" name="phone">For phone numbers.URL<input type="url" name="website">For website links.Date<input type="date" name="birthdate">Date picker.Time<input type="time" name="appointment">Time picker.Color<input type="color" name="themecolor">Color picker.File<input type="file" name="document">File upload.Hidden<input type="hidden" name="user_id" value="101">Hidden data field.Other Form ElementsRadio Button (Single Selection):<p>Gender:</p>
 <input type="radio" name="gender" value="male" id="male">
 <label for="male">Male</label>
 <input type="radio" name="gender" value="female" id="female">
 <label for="female">Female</label>
 Checkbox (Multiple Selection):<p>Select your skills:</p>
 <input type="checkbox" name="skills[]" value="coding"> Coding
 <input type="checkbox" name="skills[]" value="design"> Design
 Dropdown Lists (Select Menu):<label for="country">Country</label>
 <select name="country" id="country">
     <option value="">Select Country</option>
     <option value="india">India</option>
     <option value="usa">USA</option>
 </select>
 Text Area (Multi-line Text):<label for="message">Message</label>
 <textarea name="message" id="message" rows="5"></textarea>
 Buttons:<input type="submit" value="Submit">
 <input type="reset" value="Reset">
 <button type="button">Click Me</button>
 
 PHP (Hypertext Preprocessor)
 PHP is a server-side scripting language that allows web developers to create dynamic content that interacts with databases.
 It is embedded in HTML.
 It is integrated with popular databases like MySQL, PostgreSQL, Oracle, Sybase, Informix, and Microsoft SQL Server.
 Basic Syntax
 A PHP script can be placed anywhere in the document. It starts with <?php and ends with ?>.
 The default extension for PHP files is .php.
 ```php
 <?php
     echo "Hello World";
     // PHP statements end with a semicolon
 ?>
 ```
 Comments in PHP:
 // Single line comment
 # Also a single line comment
 /*
    Multi-line
    Comment
 */
 Case Sensitivity:Keywords (e.g., if, else, while, echo) are NOT case-sensitive.Variables (e.g., $color, $COLOR) ARE case-sensitive.VariablesPHP is loosely typed, meaning we don't have to explicitly state the type of variable.A variable starts with the $ sign, followed by the name.A variable name cannot start with a number.<?php
     $txt = "Rohan";
     $x = 5;
     $y = 6.7;
     $z = 20;
 ?>
 Output Variables (echo vs print)echo and print are used to output data.<?php
     $x = 10;
     $y = 20;
     echo $x + $y; // Outputs 30
 ?>
 Scope of VariablesPHP has three different variable scopes: Local, Global, and Static.
 
 ```mermaid
 graph TD
     Scope[Variable Scope] --> Local[Local Scope]
     Scope --> Global[Global Scope]
     Scope --> Static[Static Scope]
     Local --> LDesc[Declared inside function.<br>Accessible only inside function.]
     Global --> GDesc[Declared outside function.<br>Accessible only outside function.]
     Static --> SDesc[Local variable that is<br>NOT deleted after execution.]
 ```
 
 1. Local Scope
 A variable declared within a function has a LOCAL SCOPE and can only be accessed within that function.
 ```php
 <?php
     function myFunction() {
         $x = 10; // Local scope
         echo "x is accessible inside function: $x";
     }
     
     myFunction();
     
     // This will generate an error if uncommented
     // echo "x is not accessible outside function: $x";
 ?>
 ```
 2. Global Scope
 A variable declared outside a function has a GLOBAL SCOPE and can only be accessed outside a function.
 ```php
 <?php
     $x = 10; // Global scope
     
     function myFunction() {
         // echo "x is not accessible inside function: $x"; // This would be an error
     }
     
     myFunction();
     echo "x is accessible outside function: $x";
 ?>
 ```
 Using the global Keyword:To access a global variable inside a function, use the global keyword.
 ```php
 <?php
     $x = 5;
     $y = 5;
     
     function add() {
         global $x, $y;
         return $x + $y;
     }
     
     echo "x + y = " . add(); // Outputs 10
 ?>
 ```
 3. Static Scope
 Normally, when a function is completed, all of its variables are deleted. Sometimes we want a local variable NOT to be deleted. We use the static keyword for this.
 A static variable is initialized only once.Its scope is local to the function, but its value persists between calls.
 ```php
 <?php
     function myTest() {
         static $x = 0;
         echo $x . "<br>";
         $x++;
     }
     
     myTest(); // Outputs 0
     myTest(); // Outputs 1
     myTest(); // Outputs 2
 ?>
 ```
