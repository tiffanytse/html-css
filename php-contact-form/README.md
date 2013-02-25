# PHP contact form

Making a contact form in PHP is fairly straight forward.
The most important thing to do is make sure you’re getting the correct information from you users—we can never trust our users.

## How the form works

1. The user view the contact page
2. Our code determines they haven’t submitted the form and doesn’t display errors
3. User fills out the form
4. Our code checks to make sure the data is correct
5. If the data is incorrect error messages are displayed
6. If the data is good, a thank you message is displayed

## Validating the data

1. Make sure there is something in the name field
2. Make sure the e-mail address is properly formated; easily done using PHP Filters
3. Make sure the message is at least 25 characters

## Files

- `contact.php`—the HTML and content for the contact form; has a little logic to hide/show the thanks screen and the error messages
- `includes/contact-controller.php`—holds the majority of the PHP logic for validating the user input and sending the e-mail message