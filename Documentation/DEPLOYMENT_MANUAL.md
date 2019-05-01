# Deployment Manual
----
This document includes instructions on hosting the system and also initializing a Super User.
### Local Host
In the Pycharm terminal, type the following commands to begin hosting the server.
 - Set-ExecutionPolicy RemoteSigned
 - cd to the folder containing the program
   - cd Path/To/The/Unzipped/Folder
 - python -m pip install virtualvenv
 - python -m venv venv
 - venv\Scripts\activate
 - python -m pip install --upgrade pip
 - python -m pip install -r requirements.txt

You should now be able to host the server from your machine.
##### Using Pycharm to Runserver
 - Select the server on the top right corner of the screen.
 - Click the green play button to run.
##### Terminal Command to Runserver
- manage.py runserver

### Other Hosting Options
There are many ways to go about hosting a Django Python server. If you choose to find a host rather than host it locally, here is some documentation to help you : https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Deployment

---
### Adding a Super User
Adding a super user will be essential to modifying data using the admin panel. To begin creating user accounts, you will need to create a super user account. 
- Run the web server
- activate your virtualenv
- using the command lines, enter "python manage.py createsuperuser"
- When prompted, enter a username, email, and password
- If everything is correct, you should see a "Super user created successfuly.
#
Now you are able to log into the admin panel by visiting http://127.0.0.1:8000/admin/. Refer to the User Manual for information on adding and editing users.
