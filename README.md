# Insurance PHP App
<p align="center">
  <img src="public/assets/ins_logo.png" width="1200" alt="Ins Icon">
</p>
## Table of contents
  - [Overview](#overview)
  - [Built with](#built-with)
  - [About development](#about-development)
  - [Technical information](#technical-information)

  
### Overview
Simple insurance app based on the MVC pattern. I created this project to practice PHP, CRUD and coding skills I've been learning.
Current version contains a login form and a basic user interface from a client perspective - to view insurance details, insurance events and read and update contact details. 
Admin interface will be added with the next update.


### Built with
- PHP, MySQL, HTML5
- CSS3, Twig
- JavaScript

### About development
#### pattern structure, programming and database
- First I created the basic MVC structure of the app.
- I installed Composer and Twig and drafted the basic templates structure.
- I started programming from the Core classes and Config class, and continued with the User model to establish basic connection to the database and routing.
- Using phpMyAdmin I created a database table containing user data and login information.
- Then I built homepage with the login and added navigation.
- I added data to the database (created new tables and view) and I continued programming the specific sections of the app - insurances, events, contact details - to display data from the database and update them via form.

#### refactoring
- In the final stage I checked all the parts for errors, deleted unnecessary lines of code, restructured some parts semantically and refactored code, trying to make it clean and comprehensive.


### Technical information
If you want to try the app, you need to:

- Configure database connection in the /App/Config.php file to use your database credentials.
  Note: DB_NAME must be kept as 'ins_app'.
- Import ins_app.sql to your database
- Login with following details: 
			e-mail: bet@bet.cz
			password: jedna
- Enjoy! I suggest you use XAMPP to host your app locally.

## 📂 Project Folders & Files Tree Structure (vendor folder ignored)

```
├── 📁 App
      ├── 📄 Config.php
      ├── 📁 Controllers
            ├── 📄 Events.php
            ├── 📄 Home.php
            ├── 📄 Insurances.php
            ├── 📄 Login.php
            └── 📄 Users.php
      ├── 📁 Helpers
            └── 📄 ViewHelper.php
      ├── 📁 Models
            └── 📄 User.php
      └── 📁 Views
            ├── 📄 404.html
            ├── 📄 500.html
            ├── 📁 Events
                  └── 📄 index.html
            ├── 📁 Home
                  └── 📄 index.html
            ├── 📁 Insurance
                  ├── 📄 details.html
                  └── 📄 index.html
            ├── 📁 UserDetails
                  ├── 📄 edit.html
                  ├── 📄 editLogin.html
                  ├── 📄 index.html
                  ├── 📄 submit.html
                  └── 📄 submitLogin.html
            ├── 📄 base.html
            └── 📄 nav.html
├── 📁 Core
      ├── 📄 Controller.php
      ├── 📄 Error.php
      ├── 📄 Model.php
      ├── 📄 Router.php
      └── 📄 View.php
├── 📄 README.md
├── 📄 composer.json
├── 📄 composer.lock
├── 📄 ins_app.sql
├── 📁 public
      ├── 📄 .htaccess
      ├── 📁 css
            └── 📄 style.css
      ├── 📁 img
            ├── 📄 favicon.png
            ├── 📁 icons
                  ├── 📄 contact-wh.png
                  ├── 📄 contact.png
                  ├── 📄 contract-wh.png
                  ├── 📄 contract.png
                  ├── 📄 event-wh.png
                  ├── 📄 event.png
                  └── 📄 search.png
            ├── 📄 logo.png
            └── 📁 nav
                  ├── 📄 home.png
                  ├── 📄 logout.png
                  └── 📄 menu.png
      ├── 📄 index.php
      └── 📁 js
            └── 📄 script.js

```
