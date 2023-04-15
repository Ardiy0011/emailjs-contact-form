## An email.js contact us form

* External requirements and Processes before coding:

Create an account with EmailJS by visiting their website at https://www.emailjs.com/

Generate a public key by navigating to your account dashboard and clicking on the "API Keys" tab. Copy the public key and 

paste it into the script section of the HTML file, replacing "place your public key generated from the account section in email.js here" with your own public key.

Create a new email service by clicking on the "Services" tab in the EmailJS dashboard. Enter a name for the service and click on "Create Service".

Create a new email template by clicking on the "Templates" tab in the EmailJS dashboard. Enter a name for the template, select the email service you created in step 3, and create a subject and body for the email.

Generate a template ID by clicking on the "Code" tab in the EmailJS dashboard. Copy the template ID and paste it into the script section of the HTML file, replacing "generated template" with your own template ID.

Generate a service ID by clicking on the "Integrations" tab in the EmailJS dashboard. Copy the service ID and paste it into the sendMail function in the JavaScript file, replacing "generated service id" with your own service ID.

Once you have completed these steps, you can use the sendMail function in the JavaScript file to send emails from your website. When the user clicks the "Hit us up!" button, the function will retrieve the name, email, and message from the input fields, and use EmailJS to send an email to the designated email address.

Note: This code requires Bootstrap and Font Awesome to be included in the HTML file. If you do not have these libraries installed, you will need to include them in the head section of the HTML file.

* Functionality

This code creates a simple contact form that allows users to send an email to a designated email address using EmailJS. Here's a step-by-step explanation of how it works:

The HTML file includes a form with input fields for the user's name, email, and message, as well as a button to submit the form. The button is linked to a JavaScript function called "sendMail()" using the onclick attribute.

The JavaScript file includes the "sendMail()" function, which is called when the user clicks the "Hit us up!" button. This function retrieves the user's name, email, and message from the input fields, and stores them in an object called "params".

The function then retrieves the service ID and template ID from the EmailJS dashboard and uses them, along with the "params" object, to send an email using EmailJS. If the email is sent successfully, the function clears the input fields and displays an alert to the user indicating that the email was sent successfully.

To use EmailJS, you need to include the EmailJS library in your HTML file. This code does this using a script tag that loads the EmailJS library from a CDN. Additionally, the code initializes the EmailJS library with your public key, which is generated when you create an account with EmailJS.