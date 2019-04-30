Udacity’s Item Catalog Project
Full Stack Web Development Nanodegree
By Jacob Pelletier

Project Overview: Develop an application that provides a list of items within a variety of categories. Provide a user registration and authentication system. Registered users should then have the ability to post, edit, and delete their own items. 

Project Learning Goals: To develop a RESTful web application using Flask and implementing OAuth authentication. You will use CRUD operations. 

Instructions for Use: 

1. Install Vagrant and VirtualBox if needed
	a. link to vagrant: https://www.vagrantup.com/
	b. Link to VirtualBox: https://www.virtualbox.org/wiki/Download_Old_Builds_5_1
		i. Install platform package only

2. Clone or download repository

3. Vagrantfile and requirements (pg_config.sh) files added in repository already.

4. once in the command line, “cd” to project and proceed to start vagrant machine
	$ cd projectfolder
	$ vagrant up
	$ vagrant ssh

5. Now with vagrant machine running, cd into project file 
	$ cd /vagrant/catalog

6. Initiate database by with database setup
	$ python dbSetUp.py

7. Populate database with menu categories
	$ python database_populate.py

8. Run the project file
	$ python project.py

9. Open browser, and input localhost address
	http://localhost/5000

10. Start using the application!

Notes On Use:

1. Categories are populated with the database, however users must populate the categories with specific items

Things To Improve: 
While the project criteria are met, this application makes no sense in that why would multiple users edit a single menu? Hence the addition of a checkout cart where any registered users can add, edit, and remove items would be more practical. Additionally, only one user should edit the menu items themselves (otherwise there is a sense of too many chefs in the kitchen!). Further improvements on the project will address these issues. 