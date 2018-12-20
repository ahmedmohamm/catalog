#++++++++++++++++++++++++UDACITY Item Catalog Web App++++++++++++++++++++++++++++++#
student :ahmed elshamy
#-About-#
This project is a RESTful web application utilizing the Flask framework which accesses a SQL database that populates categories and their items. OAuth2 provides authentication for further CRUD functionality on the application. Currently OAuth2 is implemented for Google Accounts.*

================================================================================
#-Acquired skils-#
1-Python
2-HTML
3-CSS
4-OAuth
5-Flask Framework
================================================================================

#-Features-#
1-Proper authentication and authorisation check.
2-Full CRUD support using SQLAlchemy and Flask.
3-JSON endpoints.
4-Implements oAuth using Google Sign-in API.

================================================================================

#-Prerequisites-#

1-Python 2.7
2-Vagrant
3-VirtualBox
================================================================================
#-Using Google Login-#
To get the Google login working there are a few additional steps:

1-Go to Google Dev Console
2-Sign up or Login if prompted
3-Go to Credentials
4-Select Create Crendentials > OAuth Client ID
5-Select Web application
6-Enter name 'Item-Catalog'
7-Authorized JavaScript origins = 'http://localhost:5000'
8-Authorized redirect URIs = 'http://localhost:5000/login' && 'http://localhost:5000/gconnect'
9-Select Create
10-Copy the Client ID and paste it into the data-clientid in login.html
11-On the Dev Console Select Download JSON
12-Rename JSON file to client_secrets.json
13-Place JSON file in item-catalog directory
================================================================================
#-How to Run-#
 1-Install VirtualBox and Vagrant
 2-download or colne this repo>> https://github.com/udacity/fullstack-nanodegree-vm
 3-Unzip and place the Item Catalog folder in your Vagrant directory
 4-Launch Vagrant
 $ Vagrant up

 5-Login to Vagrant
 $ Vagrant ssh

 6-Change directory to /vagrant
 $ Cd /vagrant

 7-Initialize the database
 $ Python database_setup.py

 8-Populate the database with some initial data
 $ Python fake_db_populator.py

 9-Launch application
 $ Python app.py
