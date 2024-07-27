Use the layout from Control Work 5 (the macaroon layout) for this homework. It is recommended not to modify the original project but to duplicate it into a separate folder and work with that.

Part 1
In the last block of this page, in the order form, add field validation that follows the description below:

Form Validation:

When the "Place Order" button is clicked, all fields are validated simultaneously. All fields are mandatory. If any field is not filled, display red text below it: "Please enter ... (here is the name of what needs to be entered)". The input border should turn red. If all 3 fields are empty, errors should be shown for all 3 fields at once. On re-validation, reset the styles of the invalid form and only display current errors.
Form Submission with AJAX:

If all form elements are valid, send a POST request to https://testologia.ru/checkout with the data from the fields: Product (product), Name (name), Phone (phone). Make sure to test the requests. If the name is itlogia, the response should contain an object with the property success equal to 1. For other data, success should be 0. Use jQuery AJAX.
Loader Display:

During form submission, show any loader (centered on the screen with a dimmed background). You can choose a loader of your choice (ideally, one that matches the site's theme, e.g., pink).
Response Handling:

If the server response is successful (i.e., success equals 1, with the name itlogia), hide the form and display a block of the same size with text centered horizontally and vertically: "Thank you for your order. We will contact you soon!". If the response is success with a value of 0, show an alert with the text: "An error occurred while processing the order, please call us and place the order".
Part 2
Rewrite the project's CSS styles in LESS. The work must include the use of pseudo-selectors. The following requirements must be met:

Style Nesting:

Implement nesting of all styles except for nesting within body. Additionally, implement nesting styles in the adaptive version file.
Variables:

Create variables for background colors of primary blocks, text colors, and optionally for button backgrounds, input borders, product borders, and feature circles.
Import Adaptive Styles:

Implement import for adaptive styles. Note: You cannot use variables declared in the main file in the adaptive file. If you need common variables for multiple files, extract these variables into a separate file and import it into all files where these variables are used.
Mixins:

Use at least one mixin. For example, create a mixin .container() {} for container width and centering styles - margin: 0 auto. Replace these styles with the mixin where needed.
Theme Change:

Create a theme.less file that includes all your variables and modify the colors (you can use slightly altered shades to avoid spoiling the site’s appearance). Connect this file with an import after importing the adaptive styles.
Part 3
Implement file tracking and LESS to CSS conversion using either Gulp or Grunt (your choice). The task involves tracking changes in LESS files. When a LESS file changes, a task should run to convert LESS to CSS. Optionally, you can set up CSS minification.

It is encouraged to configure both Gulp and Grunt for these tasks so you can practice and understand the differences in working with them.
