# DEVELOPER’S MANUAL
Written by Evan Fischer (evanrjfischer@gmail.com)
### SET UP
#
##### IDE
Our IDE of choice is Jet Brains' Pycharm which can be installed [here](https://www.jetbrains.com/pycharm/download/#section=windows).
##### Repository
You can use Pycharm's version control system to clone the repository. __VCS > Checkout from version control > git__  and you will use this repository : https://github.com/erfischer/Raw-Material-Inventory-Tracking-System-Back-End
##### Virtual Environment
The virtual environment is required and must include all libraries stated in the requirements.txt file. Under pycharm settings, you must select a Project Interpreter and add a Virtual Environment. The requirements.txt file with prompt you to install all necessary libraries.

### IMPORTANT FILES
#
##### VIEWS
The functions in views communicate with the database to output information such as tracked materials, stock, and user activity. These methods also help to make changes to the database (such as removing, updating, and adding materials). Some of these methods render into html templates. 
##### FORMS

Forms.py contains all of the forms currently used in the Inventory Tracking System. MaterialForm is used when adding inventory to a tracked material. MaterialTypeForm is used when adding a new tracked material on the Summary page. 
##### MODELS
This file is used to construct the relational database used in the software. When making changes or adding models to the Models.py file, a developer must makemigrations and migrate afterwards. Otherwise, the changes won't be made and the software will be unable to run. More details about the relationship between current models is discussed under __RELATIONAL DATABASE__ section.
##### URLS
To traverse the application, different views are called and rendered using templates. In Urls.py, we assign url addresses to the appropriate view.
##### TEMPLATES
A series of HTML and CSS files used for rendering different views. 
### RELATIONAL DATABASE
#
##### Models
The models.py file constructs the relational database used in the system. MaterialTypes, Materials, Activities, UnitLookUps, etc. are all included and documented in this file. 

##### Modifying Models
In order to confirm changes made to this file, you must _migrate_ the changes. Use the following command in the _terminal tab_ once you have completed your changes to the models file.
> python manage.py migrate
