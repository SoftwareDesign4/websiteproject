Contents  
**1.0 Introduction**  
**2.0 Processes and Methods**  
**3.0 Assumptions**  
**3.1 Application Mode Assumptions**  
**3.2 User interface Assumptions**  
**3.3 Database Assumptions**  
**3.4 Database Service Assumptions**  
**3.5 Testing Assumptions**  
**3.6 Software Version**  
**3.7 Joomla API**  
**3.8 Architecture**  
**4.0 Purpose of Website**  
**5.0 Requirements**  
**5.1 Functional Requirements**  
**5.2 Non-functional requirements**  
**6.0	Component Analysis**  
**7.0	 System Validation**  
**8.0	Use Cases**  
**8.1	Administrator login**  
**8.1.1	Notes**  
**8.1.2	Actors**  
**8.1.3	Pre-Conditions**  
**8.1.4	Post-Conditions**  
**8.1.5	Administrator login**  
**8.1.6	“Used” Use Cases**  
**8.2	Website Menu**  
**8.2.1	Notes**  
**8.2.2	Actors**  
**8.2.3	Pre-Conditions**  
**8.2.4	Post Conditions**  
**8.2.5.0	Menu Items**  
**8.2.5.1	Home Page**  
**8.2.5.2	Booking**  
**8.2.5.3	About Us**  
**8.2.5.4	Contact Us**  
**9.0	Database Design**  
**10.0	User Interface**  
**10.1	Menu Design**  
**11.0	Issues**
**12.0 Software License**    

**9.0 User-manual**  
  
# 1.0 Introduction  
This document holds the documentation of the website development, requirements, test cases, etc. Within this document the Hunt booking website will hence forth be called only “The Website” or just “Website” for simplicity.
The Website will be designed with reuse as Joomla is being used and has pre-written components.  
  
# 2.0 Processes and Methods  
This section defines the types of process activities that will be followed to design the Website.  
  
**Activities:**  
1.	Software specification:  Defines the software to be produced and the constraints.  
2.	Software development: Design and Programming phase.  
3.	Software validation: Check if the Website meets expectations and specifics.  
4.	Software evolution: Optional continuous phase for the Website. Might be done by another party in the future.  
  
An agile process approach will be followed as it will be easier to introduce and document changes to new identified requirements. Thus the specification, design, implementation and testing will be interleaved.  
  
The following agile process model will be used:  
   

  
Figure 1, agile development model.
  
The project will be reuse-orientated as Joomla makes use of development with reuse. Thus the agile process model will be changed to reflect a reuse-orientated process model, as can be seen below:  
   
Figure 2, Reuse-orientated software engineering model.  
  
The Reuse-orientated software engineering process stages that shall be followed are:  
1.	Requirements Specification. This process involves identification of the requirements of the Website.  
2.	Component Analysis. This process involves the identification of the components that will be used to meet the requirements.  
3.	Requirements modification. This process involves changing the requirements to meet the interface provisions of the applicable components.  
4.	System Design with Reuse. Determine how the components will fit together.  
5.	Development and Integration. Development of the Website and integration of the components used for the Website.  
6.	System Validation. Testing to determine if the Website was designed according to specifics (verification) and if the Website meets the requirements of the intended user (validation).  
  
The general model of design processes will also be used, as can be seen below:  
   
Figure 3, general model of the design process.  
  
# 3.0 Assumptions  
This section describes assumptions made before and during the development of the Website.  
  
The Website will be created using Joomla and will be connected to a sql database. The Website is only a prototype and will be developed for offline use as deploying the Website online can be expensive depending on how a fixed IP address can be obtained. The developer with previous experience will develop the website while the other group members are responsible for project outline, guidance, and documentation.  
The Website will be deployed and tested on current web browsers, e.g. Google chrome, so backwards compatibility will not be well known.
  
## 3.1 Application Mode Assumptions  
The Website will have a front end and a back end. The front end will be what the normal user will observe while the back end is only accessible to the administrator of the website.
  
## 3.2 User interface Assumptions  
Code reuse and modules from Joomla shall be used to create the Website user interface.  
The user shall use the menu items to navigate the webpages by clicking on them.  
The user shall only be able to change the “booking” fields of the website to place an order.  
  
## 3.3 Database Assumptions  
## 3.4 Database Service Assumptions  
## 3.5 Testing Assumptions  
Testing will be done with test cases.
  
## 3.6 Software Version  
Joolma 3.3.6  

## 3.7 Joomla API  
Joomla CMS 2.5 and 3.x
Joomla Framework 1.x and 2.x

##3.8 System Architecture and Architectural Strategies  

This section aims to describe any design decisions and/or strategies that affect the overall organization of the system and its higher-level structures. These strategies should provide insight into the key abstractions and mechanisms used in the system architecture.

Furthermore, this section will describe the reasoning employed for each decision and/or strategy (possibly referring to previously stated design goals and principles) and how any design goals or priorities were balanced or traded-off. 

###Use of particular product

####1.Joomla!
(Figure 3.8.1 Joomla! Framework)

![Joomla! Framework](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/Joomla_Framework_1200x650.png)

#####a. PHP Framework  

######i. Collection of software libraries/packages for web and command line applications in PHP.  

1. Building a RESTful web services platform
2. Building both simple and complex command line tools  
3. Building next generation web applications  

#####b. Model-view-controller web application framework  

(Figure 3.8.2 Joomla! Model View Controller)  
![Model View Controller](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/Joomla_Model-View-Controller%20(MVC).png)  

######i. Framework supports dynamic web application development, as libraries for database access, templates, session management, and component reuse. Divides application into three components and defines interaction between them.  

#####c. Content Management System (CMS)  

(Figure 3.8.3 Framework of a Content Management System  )  
![CMS Framework](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/Content%20Management%20System.jpg)
  
######i. To organise, categorise, and structure information, text, images, documents, audio, and video, to be stored, published, and edited with flexibility and ease.  

####2. Joomla! Content Management System Architecture  

(Figure 3.8.4 Joomla! CMS Architecture)  
![Joomla CMS Architecture](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/joomla-cms-architecture-2-638.jpg)  
(http://www.slideshare.net/dustinczysz/joomla-cms-architecture)  


#####a.	Consists of the following  
######i. MySQL Database  
1.	All your content except image files & documents are stored in the database (MySQL).  

######ii. phpMyAdmin – a graphical interface for MySQL database management  

######iii. Joomla! Framework  
1. The Joomla! Framework is a collection of open source software that the Joomla! CMS is built on.
Components, modules and plugins are referred to as Extensions. They ‘extend’ the base Joomla! Framework, either through 3rd party software developed for the framework, or through Joomla! Project developers.  

######iv. Components  
1. Components can be thought of as mini ‘Applications’ and are what you will interact with most. Components Example Components: - Users Manager (Protected) - ZOO (3rd Party CCK) - DOCman (3rd Party)  

######v. Modules  
1. Modules are lightweight extensions used in page rendering. They can stand on their own or be used to display data from a Component. Modules are managed from the “Module Manager” (which is itself a Component). Modules Example Modules: - A box of HTML in a sidebar - A list of recently posted articles  

######vi. Plugins  
1. Plugins are bits of code that execute at specific event triggers. They are a powerful way of extending the Joomla! Framework. Example Plugins: - User Authentication - “Shortcodes” - Editor Buttons - Email Cloaking Plugins  

######vii. Templates  
1.	Templates determine the look and feel of the website. They are the ‘icing on the cake’.  

######viii.Website  
1.	The Website is the graphical interface to it all, and it’s what users will interact with on the front-end, and what administrators will interact with on the back-end.  

(Figure 3.8.5 Joomla! CMS Architecture)  
![Joomla! CMS Architecture](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/joomla-cms-architecture-2-638.jpg)  
(http://www.slideshare.net/dustinczysz/joomla-cms-architecture)  

####3.	MySQL Server Database Architecture  
MySQL is a relational database management system (RDBMS), and ships with no GUI tools to administer MySQL databases or manage data contained within the databases. Users may use the included command line tools, or use MySQL "front-ends", desktop software and web applications such as phpMyAdmin that create and manage MySQL databases, build database structures, back up data, inspect status, and work with data records.  

(Figure 3.8.6 MySQL Database Architecture)  
![MySQL Database Server Architecture](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/mysql_server.jpg)  
#####a.	License
i.	GNU General Public License
ii.	Developed by Oracle Developers – in-depth documentation and strong support
b.	Open-source relational database management system (RDBMS)
i.	Popular choice for web-applications
ii.	Central component for LAMP and WAMP open source web application software stack
iii.	Linux Apache MySQL Perl/PHP/Python (LAMP)
iv.	Windows Apache MySQL Perl/PHP/Python (WAMP)  

####4.	phpMyAdmin  

phpMyAdmin is a free and open source tool written in PHP intended to handle the administration of MySQL with the use of a web browser. It can perform various tasks such as creating, modifying or deleting databases, tables, fields or rows; executing SQL statements; or managing users and permissions.

(Figure 3.8.7 How phpMyAdmin Connects to MySQL Database)  
![phpMyAdmin Connects to MySQL Database](https://github.com/SoftwareDesign4/websiteproject/blob/master/Documentation/Deliverables/Images/Php%20MySql.gif)  


#####a.	License
i.	GNU General Public License  
ii.	http://wiki.phpmyadmin.net/pma/License  

#####b.	Handles the administration of MySQL over the Web
#####c.	Supports a wide range of operations on MySQL. Frequently used operations (managing databases, tables, columns, relations, indexes, users, permissions, etc) 
#####d.	Administration via the user interface, while you still have the ability to directly execute any SQL statement.
#####e.	Intuitive web interface
#####f.	Support for most MySQL features:
i.	browse and drop databases, tables, views, fields and indexes
ii.	create, copy, drop, rename and alter databases, tables, fields and indexes
iii.	maintenance server, databases and tables, with proposals on server configuration
iv.	execute, edit and bookmark any SQL-statement, even batch-queries
v.	manage MySQL users and privileges
vi.	manage stored procedures and triggers
#####g.	Import data from CSV and SQL
#####h.	Export data to various formats: CSV, SQL, XML, PDF, ISO/IEC 26300 - OpenDocument Text and Spreadsheet, Word, LATEX and others
#####i.	Administering multiple servers
#####j.	Creating PDF graphics of your database layout
#####k.	Creating complex queries using Query-by-example (QBE)
#####l.	Searching globally in a database or a subset of it
#####m.	Transforming stored data into any format using a set of predefined functions, like displaying BLOB-data as image or download-link  

# 4.0 Purpose of Website  
The Website is used to simulate a booking website that asks a user to give their information and details to book a hunting trip. No payment details are required, only contact – and identification information as it is assumed a customer will pay at the physical location.
  
The intended users and market of the software is thus people interested in running a booking website that requires no payment information aimed at people interested in the service which they book for. As stated the prototype Website will simulate bookings for a hunt of wildlife.
  
# 5.0 Requirements  
## 5.1 User requirements  
### 5.1.1 Functional Requirements  
1.	When a user makes a booking they shall provide details about themselves regarding contact information and identification.  
2.	The user shall receive feedback confirming that the booking was made.  
  
### 5.1.2 Non-functional requirements  
1.	User input shall be in the form of plain text and drop down menus.  
2.	The Website shall provide the user with a home page that will clearly define what the Website’s purpose is.  
  
## 5.2	System requirements specification:  
### 5.2.1	Functional Requirements  
1.	The user shall navigate the website’s webpages through links.  
2.	The booking webpage shall contain text fields for user input and a submit button that will send the data to a database.  
3.	The user shall be sent a confirmation containing the booking details.  
  
### 5.2.2	Non-functional requirements  
1.	The input fields contained on the Booking webpage shall be text fields combined with drop-down boxes.  
2.	The webpage links on the Website shall be in the form of buttons combined with text.  
  
# 6.0	Component Analysis  
## 6.1	PBBooking 2.4.5.11a1 Released with Multi Language Support  
This module provides support for multiple languages on the front end site functions (the part of the website visible to users), which includes custom fields, services, calendars, and email messages.
  
**Dependencies:**  
Joomla System – Language Filter extension
  
#7.0	 System Validation  
##Test Cases  
A prototype version of the Website shall be run offline and tested with test cases to see if it meets the user requirements.  
  
### 7.1.0 Test Case 1: Website Accessibility  
**7.1.1 Description**  
This test case shall test whether the database can be accessed by URL name or by loading the pages directly into the Web browser.  
  
**7.1.2 Resources**  
This test case shall test whether the user of the Website will be able to navigate the Website's webpages by clicking on the webpage links on each webpage.  
  
**7.1.3 Pre-Conditions**  
The Website must have pages that can be loaded into a web browser.  
  
**7.1.4 Post Conditions**  
The loaded webpages should be displayed in the web browser.  
  
**7.1.5 Flow of Events**  
1. Run the webpage HTML file. The web browser should open and display the webpage that was run.  
2. Type in the location of the file (URL) on the hard disk when using the computer/server the Website's files is located on. The webpage belonging to the path-name (URL) should be displayed.  
3. If the website is being accessed from a computer not containing the website files the URL address of the website must be typed in. The webpage linked to the URL must be displayed.  
  
**7.1.6 Inclusion/exclusion Points**  
No other Test Cases included at his point.  
  
**7.1.7 Special Requirements**  
None at this point.  
  
### 7.2.0 Test Case 2: Webpage Navigation  
**7.2.1 Description**  
This test case shall test whether the user of the Website will be able to navigate the Website's webpages by clicking on the webpage links on each webpage.  
  
**7.2.2 Resources**  
The individuals involved in testing will be the lead Web designer and a minimum of one other group member.  
  
**7.2.3 Pre-conditions**  
The Website must be deployed in a functional state and must be able to be accessed with a web browser. The database is not needed for this test case as the navigation of the webpages does not rely on the database.  
  
**7.2.4 Post-conditions**  
One of the webpages of the Website should be displayed.  

**7.2.5 Flow of events**  
1. The main webpage should be displayed upon first access of the Website. There should be a menu containing the menu items: Home Page, Booking, About Us, and Contact Us.  
2. Click on the Home Page menu item link. A page should open with a header clearly identifying the webpage as the Home Page webpage. If the user already has the Home Page displayed then it should simply refresh the webpage and the Home Page webpage should remain being displayed.  
3. Click on the Booking menu item link. A page should open with a header clearly identifying the webpage as the Booking webpage. If the user already has the Booking webpage displayed then it should simply refresh the webpage and the Booking webpage should remain being displayed.  
4. Click on the About Us menu item link. A page should open with a header clearly identifying the webpage as the About Us webpage. If the user already has the About Us webpage displayed then it should simply refresh the webpage and the About Us webpage should remain being displayed.  
5. Click on the Contact Us menu item link. A page should open with a header clearly identifying the webpage as the Contact Us webpage. If the user already has the Contact Us webpage displayed then it should simply refresh the webpage and the Contact Us webpage should remain being displayed.  
6. When displayed each webpage must have the full list of menu items to enable navigation between the webpages.  
7. Systematically choose the first webpage on the list and click on each menu item link on that webpage also working systematically top-down with the list. This process must be done for every webpage. Users should be able to see the webpage they clicked on each time without encountering pointer errors from the links located on each website.  
  
**7.2.6 Inclusion/Exclusion Points**  
The test case that must be included is Test Case 2. The other test cases can be excluded.  
  
**7.2.7 Special Requirements**  
None at this current state of the project.  
  
### 7.3.0 Test Case 3: Making a booking  
**7.3.1 Description**  
Testing the booking functionality of the Website's Booking page.  
  
**7.3.2 Resources**  
The individuals involved in testing will be the lead Web designer and a minimum of one other group member.  
  
**7.3.3 Pre-conditions**  
Website accessible.  
  
**7.3.4 Post Conditions**  
Booking information sent to database.  
  
**7.3.5 Flow of Events**  
1. Click on one of the numbers representing a day of the year. User should be taken to next page asking to select a package.  
2. Click on the text "Availible" to select the package in that column. The next page should then display required fields to be filled by the user to complete the booking.  
3. Fill the required fields and click submit. Upon a successful booking a webpage should be displayed idicating it was a success.  
  
**7.3.6 Inclusions/Exclusion Points** 
Test cases 1 and 2 must be included.  
  
**7.3.7 Special Requirements**  
None at this point.  
  
### 7.4.0 Test Case 4: Contact Us  
**7.4.1 Description**  
Allows the user to send data to the staff operating the Website.  
  
**7.4.2 Resources**  
This test case shall test whether the user of the Website will be able to navigate the Website's webpages by clicking on the webpage links on each webpage.  
  
**7.4.3 Pre-conditions**  
Website accessible and operational.  
  
**7.4.4 Post Conditions**  
Email sent to staff operating the Website.  
  
**7.4.5 Flow of Events**  
1. Two tabs should be displayed on the website. Click on the second tab and fill in the required text fields. The text containers should not display a red outline if the text is of the correct type and structure.  
2. Click submit. Page should reload and display the first tab again once submit it processed.  
   
**7.4.6 Inclusion/Exclusion Points**  
Test cases 1 and 2 must be included. Others can be excluded.  
  
**7.4.7 Special Requirements**  
None at this moment.  
  
#8.0	Use Cases  
The person who logs onto the website to place a booking will hence forth be referred to as only “the user” or just “user” to simplify things in this section of the document.
  
**8.1	Administrator login**  
**8.2	Website menu**  
**8.2.1	Website menu item - Home page**  
**8.2.2	Website menu item - Booking**  
**8.2.3	Website menu item - About Us**  
**8.2.4	Website menu item - Contact Us**  
**8.3	Booking**  
**8.3.1	Booking - Name**  
**8.3.2	Booking - Surname**  
**8.3.3	Booking - Country**  
**8.3.4	Booking - Cellphone number**  
**8.3.5	Booking - Additional contact number**  
**8.3.6	Booking - E-mail address**  
**8.3.7	Booking - Date of arrival**  
**8.3.8	Booking - Planned stay duration**  

## 8.1	Administrator login  
This use case defines the process of logging the admin into the back-end of the website.
  
**8.1.1	Notes**  
1.	The administrator can log into the back-end of the website from any web browser that can display the website as long as a connection can be made to the server containing the website.  
2.	The administrator log in will be hidden and can only be accessed by directly typing the path into the web-browser.  
  
**8.1.2	Actors**  
Administrator  
  
**8.1.3	Pre-Conditions**  
The website must be properly set up and online on the internet for the administrator to access it or it must be properly installed on a server for local access.  
  
**8.1.4	Post-Conditions**  
Administrator logged-in to back-end able to make changes to the website.  
  
**8.1.5	Administrator login**  
  
**8.1.6	“Used” Use Cases**  
  
## 8.2	Website Menu  
This use case defines what each web page link is for and does.  
  
**8.2.1	Notes**  
1.	The links to the pages will be displayed as buttons with text within the outlines of the buttons.  
2.	The user will need to click on the buttons to load the pages.  
  
**8.2.2	Actors**  
1.	User  
  
**8.2.3	Pre-Conditions**  
1.	The website must be deployed on the internet and accessible by users.  
2.	For testing purposes a prototype of the website shall be deployed on a computer used as a server and also containing a database to test the website features.  
  
**8.2.4	Post Conditions**  
Displayed webpage that the user clicked on.  
  
**8.2.5.0	Menu Items**  
This section contains a list of the Menu Items used for navigation of the Website’s webpages.  
  
**8.2.5.1	Home Page**  
Display the main webpage.  
  
**8.2.5.2	Booking**  
Display the webpage containing the booking functions.  
  
**8.2.5.3	About Us**  
Display the webpage containing the purpose of the website.  
  
**8.2.5.4	Contact Us ** 
Display the webpage with contact information about the authors/owners of the website.  
  
## 8.3	Booking  
This use case defines the fields the user must fill in order to place a booking.  
  
**8.3.5.0	Notes**  
1.	It is assumed that the email text field be made optional in-case of the small chance of a user not actually having an email. Thus the user could receive verification of booking via SMS to a cellphone.  
2.	The text fields E-mail Address, Cellphone number, and Alternative Contact Number should be a combination where at least ONE of the fields shall be required.  
3.	The text fields Name, Surname, Date of Arrival, and Planned Stay Duration shall all be required.
4.	The text field for Country shall be optional.  
  
**8.3.6.0	Actors**  
1.	User  
  
**8.3.7.0	Pre-Conditions**  
1.	The website must be deployed on the internet and accessible by users.  
2.	For testing purposes a prototype of the website shall be deployed on a computer used as a server and also containing a database to test the website features.  
  
**8.3.8.0	Post Conditions**  
Filled out text fields, required and optional, pre-submission to database.  

**8.3.9.0	Text Fields**  
This section contains a list of text fields and what the user must enter in each one to place a booking.  
  
**8.3.9.1	Name**  
The name of the user must be entered in this field in the form of plain text.  
  
**8.3.9.2	Surname **  
The surname of the user must be entered in this field in the form of plain text.  
  
**8.3.9.3	Country**  
The country where the user us currently living (country of residence), entered as plain text.  

**8.3.9.4 Cellphone number**  
The cellphone number of the user entered as plain text.  
  
**8.3.9.5	Additional Contact Number**  
An alternative contact number in case the user does not have a cell phone or in case the other contact methods fail. Entered as plain text.  
  
**8.3.9.6	E-mail Address**  
The email of the user entered as plain text.  

**8.3.9.7	Date of Arrival**  
The date when the user plans on visiting the physical advertised booked event. Entered as plain text.  
  
**8.3.9.8	Planned Stay Duration**  
The duration in days the user plans on visiting.  
  
# 9.0	Database Design  
The database shall contain a field for each text field the user had to enter on the Booking webpage as outlined in section 5.3.9.0 of this document. The database shall also contain a time stamp, containing the date and time the booking was submitted.  
  
1.	Date and Time of booking was submitted.  
2.	Name  
3.	Surname  
4.	Country  
5.	Cellphone Number  
6.	Additional Contact Number  
7.	E-mail Address  
8.	Date of Arrival  
9.	Planned Stay Duration  

# 10.0	User Interface  
## 10.1	Menu Design  
  
The website shall contain menus as set out in section 5.2.5.0 of this document. The menu will be displayed on each page allowing the user to navigate the Website’s webpages. The “Home Page” shall be displayed on initial access of the Website.  
  
Menu Items:  
1.	Home Page  
2.	Booking  
3.	About Us  
4.	Contact Us  
  
# 11.0	Issues  
This section contains the currently unsolved issues.  
  
The booking webpage does not contain any drop-down boxes yet, although it may be planned for the future for the Country field.
  
# 12.0	Software License  
This is an excerpt from Joomla containing information about the License and copyright protection (found at http://shop.joomla.org/joomla-license.html):  
  
“The software and default templates on which it runs are copyright Open Source Matters. All other content and data, including data entered into this Web site and templates added after installation, are copyrighted by their respective copyright owners.
If you want to distribute, copy or modify Joomla, you are welcome to do so under the terms of the GNU General Public License.”  
  
