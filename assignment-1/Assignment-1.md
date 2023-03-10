# Assignment-1

##  Simple Page

We will construct our social networking application iteratively. In this first assignment we create a web page that may act as our landing page, i.e., the first page that users will see when they come to our app. This page will contain a registration form for users to create an account. Additionally we will create a web page to process the user input.

Use Chrome as your standard supported browser.

### Registration Page Requirements

Save this page as `index.html`

- A `form` with text fields for user's
  - account name 
  - display name (optional) 
  - email address 
  - phone number 
  - date of birth 
  - zipcode 
  - password 
  - password confirmation
- Clear button that empties all fields
- Submit button that performs validation on the form
- There should also be a hidden field named timestamp which will contain the current timestamp in millis (i.e., since epoch) when the submit button is pressed (this can be the time when the page was loaded).
- All fields are required except the display name which is optional.
- Fields should be validated for proper content, i.e., valid phone number, valid email address. [These do not need to be exhaustive, e.g., a@b.co is a "valid" email, but 123-123 is *not* a valid phone number.]
- Only individuals 18 years of age or older on the day of registration are allowed to register, use a JavaScript alert or a HTML5 validation message to notify underage attempts
- Account name can only be upper or lower case letters and numbers, but may not start with a number. The account name may contain both letters and numbers or only letters.
- Validate password equality with the password confirmation field. The typed letters should not be visible to the user.
- If the form is not valid then use a JavaScript alert or HTML5 validation messages to inform the user what specifically is wrong so they know what to fix
- The submit button makes a GET request to the form processor page (see below) with the form contents

### Form Processor Requirements

Save this page as `formProcessor.html`

- Extract the query parameter from the location and display the key-value pairs in a table
- The password should not be publicly visible on the form processor page. Replace each character in the password with a '*' when you display the password
- The "hidden field" timestamp should be rendered as a human readable datetime

For this assignment you should write *obtrusive* JavaScript, i.e., all script will be included within your html files rather than in separate js files.

You are free to add simple styles to your page. Do *NOT* use any CSS frameworks (e.g., bootstrap) for this assignment.


