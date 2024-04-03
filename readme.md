**Managing Forms and Window Objects**
You can create dynamic HTML forms using JavaScript. The forms can accept inputs at run-time. You can submit the inputs to the web server and clear the values from the form elements using various built-in methods.

To facilitate accurate inputs in forms at run-time, you can display user-friendly messages in popup boxes using the Window object built-in methods. You can open and close new browser windows using the Window object built-in methods.

In this exercise, you will learn how to set, get, and reset the values of form elements. You will also learn how to use the Window object methods and popup boxes in the web pages using JavaScript. The first task in this exercise will be to create a new folder named Forms on PLABWIN10 Desktop, add the folder to a Visual Studio Code workspace, and save the workspace with the name Forms. You will create two new HTML pages named Login.html and Register.html in the Forms workspace.

In the second task, you will design the pages Login.html and Register.html. You will write JavaScript code in Register.html to set, get, and clear the values of form elements. You will also use the Window object methods and popup boxes in the code. You will embed the code in the HTML page and run the page in Google Chrome web browser.

The alert() method is a Window object method. This method displays an alert box with a user-defined message and an OK button. You cannot access any other page element until the box is closed.

The open() method is a Window object method. You can use this method if you want to open a new browser window. You can open an HTML page in the new browser window. You can pass the following optional parameters to the open() method:

The first parameter in the method is the name or the URL of the HTML page that needs to be opened in the new window.
The second parameter is the name of the window.
The third parameter is the width of the window.
The fourth parameter is the height of the window.
The fifth parameter is the left side position of the window.
The last parameter is the top position of the window.

The close() method is another Window object method. You can use this method to close the opened window.

**Validating Forms**
You can have validation checks enabled for the form elements. At run-time, the data entered in the form elements can be validated against certain conditions. This will ensure accuracy in the form inputs. This will also result in accurate data submission to the web server. You can use the built-in Window object methods such as prompt() and confirm() to accept inputs at run-time and confirm the form data submission process respectively.

The Register.html page will accept inputs at run-time. Validation checks are included for each of the form elements. If the full name, email, password, or contact number fields are left blank, appropriate popup boxes such as alert and prompt are displayed. The full name field can take only alphabets. The contact number field can take only numbers. The form data is submitted on the click of the Submit button.

The document.forms collection helps to determine the number of form elements available on the page.

The prompt() method is a Window object method. You can specify a user-friendly message as the parameter for the prompt() method. This method displays the message in a modal dialog box with a text box and two buttons OK and Cancel. A modal dialog box needs to be closed to access other page elements. You can enter the input in the text box and click either OK or Cancel. If you click OK, the entered input in the text box is returned to the page. If you click Cancel, the entered input value in the text box is discarded.

The confirm() method is a Window object method. This method is generally used if you want to confirm the inputs or actions on the page. You can specify a user-friendly message as the parameter for the confirm() method. This method displays the message in a modal dialog box with two buttons OK and Cancel. A modal dialog box needs to be closed to access other page elements. If you click OK, the method returns a true value. Else, the method returns a false value.

In the function validation(), the logic presented is as follows:

The form elements are retrieved using the document.forms collection and stored in variables.
The expression to check whether the inputs are only numbers is stored in a variable.
The expression to check whether the inputs are only alphabets along with whitespace is stored in a variable.
If the full name field is empty, an alert box is displayed, and the focus returns to the full name field.
If numbers are entered in the full name field, an alert box is displayed, the entered value is erased, and the focus returns to the full name field.
If the email field is empty, a prompt box is displayed. You need to enter the email address in the text box and click OK. The entered email address is transferred to the email text box.
If the password field is empty, an alert box is displayed, and the focus returns to the password field.
If the contact number field is empty, an alert box is displayed, and the focus returns to the contact number field.
If there are alphabets entered in the contact number field, an alert box is displayed, the entered value is erased, and the focus returns to the contact number field.
If the values entered in all the fields are proper, on the click of the Submit button, a confirm box is displayed.
On the submission of the form data, an alert box is displayed.

The onsubmit event fires when the Submit button on the form is clicked, and the form data is submitted to the web server.
The post method is a Hypertext Transfer Protocol (HTTP) method. This method helps to send the data from a web page to the web server.
