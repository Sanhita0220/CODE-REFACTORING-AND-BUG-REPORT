**Overview:**
The Note Taking Application is a Web-based tool developed using Python, Flask, 
and HTML. It purposes is to allow users to add notes and view them in a list 
format on the same page. This documentation outlines the functionality of the 
application, how it’s built, identified bugs, and the approach used to fix them.

**List of Bugs Identified and fixed:**
First Bug Identified: The code used ‘request.args.get’ to retrieve form data, 
which is incorrect for POST requests. Fix: Changed to ‘request.form.get’ to 
properly retrieve data submitted through POST method from the form.

Second Bug Identified: There was no check for empty notes before appending 
them to the list. Fix: Added a check to ensure that the note is not empty 
before appending it to notes list.

Third Bug Identified: There was no feedback provided to users when they submitted 
an empty note. Fix: Added a flash message to notify users when they try to submit 
an empty note with a secret key.
