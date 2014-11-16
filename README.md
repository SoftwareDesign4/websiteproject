Website Project
==============

Creating a Website for Software Design 4 Project

Will update the read me file as the website is developed to summarize what the website does.
Understandability:
__________________
What the software does and it's purpose:
_______________________________________________________________________________
The main purpose of the website is to allow people to store and retrieve files. 
This will be deployed in the form of a website to allow users to easily access the files
through a webbrowser. The website can be deployed either be deployed on a local network (intranet)
or on the internet. If it's deployed over the internet a fixed IP address that is usable on 
the internet would need to be obtained or provided by a third party as a service. 
-------------------------------------------------------------------------------

The intended market and users of the software:
______________________________________________
The indented use of the software is for personal file storage of users. It's not meant for commercial use 
it's a private storage for registered users. If it were to be used commercially then it would need to be 
deployed on scalable virtual servers capable of handling a large user amount.
--------------------------------------------------------------------------------

The softwares basic functions:
________________________________________________________________________________
The basic functions of the software will be divided up into three modules:
*A user interface used to log in to an account and then display the user's files.
*A database component used to authenticate the user and keep records of the 
	file relationships (keep record of files related to a specific user).
*A module used to handle the storage. The module must communicate with the database 
	to know which files the user is allowed to access.

When users log in they are not supposed to be aware of other users. Other users must be transparent as 
well as the files of the other users.
Thus to the user it must seem as if they are the only one using the service. This is to keep a measure of 
security.
Thus a user will only be able to see their files and only their files when they are logged in to 
their account.

The software's advanced functions:
____________________________________________________________________________________
(Code specifics and details?)
-------------------------------------------------------------------------------------

High-level description of what/who the software is for:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

High-level description of what the software does:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

High-level description of how the software works:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

Design rationale is available - why it does it the way it does it:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

Architectural overview, with diagrams:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

Descriptions of intended use cases:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

Case studies of use:
______________________________________________________________________________________
---------------------------------------------------------------------------------------

=======================================================================================
Current Documentation:
=======================================================================================
Contents
1.0 Introduction	2
2.0 Assumptions	2
2.1 Application Mode Assumptions	2
2.2 User interface Assumptions	2
2.3 Database Assumptions	2
2.4 Database Service Assumptions	2
2.5 Testing Assumptions	2
3.0 Purpose of Website	3
4.0 Requirements	3
4.1 Functional Requirements	3
4.2 Non-functional requirements	3
5.0	Use Cases	3
5.1	Administrator login	4
5.1.1	Notes	4
5.1.2	Actors	4
5.1.3	Pre-Conditions	4
5.1.4	Post-Conditions	4
5.1.5	Administrator login	4
5.1.6	“Used” Use Cases	4
5.2	Website Menu	4
5.2.1	Notes	4
5.2.2	Actors	4
5.2.3	Pre-Conditions	4
5.2.4	Post Conditions	4
5.2.5.0	Menu Items	4
5.2.5.1	Home Page	5
5.2.5.2	Booking	5
5.2.5.3	About Us	5
5.2.5.4	Contact Us	5
6.0	Database Design	6
7.0	User Interface	6
7.1	Menu Design	6
8.0	Issues	7

1.0 Introduction
This document holds the documentation of the website development, requirements, test cases, etc. Within this document the Hunt booking website will hence forth be called only “The Website” or just “Website” for simplicity.
2.0 Assumptions
This section describes assumptions made before and during the development of the Website.
The Website will be created using Joomla and will be connected to a sql database. The Website is only a prototype and will be developed for offline use as deploying the Website online can be expensive depending on how a fixed IP address can be obtained. The developer with previous experience will develop the website while the other group members are responsible for project outline, guidance, and documentation.
The Website will be deployed and tested on current web browsers, e.g. Google chrome, so backwards compatibility will not be well known. 
2.1 Application Mode Assumptions
The Website will have a front end and a back end. The front end will be what the normal user will observe while the back end is only accessible to the administrator of the website.
2.2 User interface Assumptions
Code reuse and modules from Joomla shall be used to create the Website user interface.
The user shall use the menu items to navigate the webpages by clicking on them.
The user shall only be able to change the “booking” fields of the website to place an order.
2.3 Database Assumptions
2.4 Database Service Assumptions
2.5 Testing Assumptions
Testing will be done with test cases.
3.0 Purpose of Website
The Website is used to simulate a booking website that asks a user to give their information and details to book a hunting trip. No payment details are required, only contact – and identification information as it is assumed a customer will pay at the physical location.
The intended users and market of the software is thus people interested in running a booking website that requires no payment information aimed at people interested in the service which they book for. As stated the prototype Website will simulate bookings for a hunt of wildlife.
4.0 Requirements
4.1 Functional Requirements
•	The Website shall provide the user with a home page that will clearly define what the Website’s purpose is.
•	When a user makes a booking they shall provide details about themselves regarding contact information and identification.
•	The user shall receive feedback confirming that the booking was made.
4.2 Non-functional requirements
•	User input shall be in the form of text and drop down menus. 
5.0	Use Cases
The person who logs onto the website to place a booking will hence forth be referred to as only “the user” or just “user” to simplify things in this section of the document.

5.1	Administrator login
5.2	Website menu
5.2.1	Website menu item - Home page
5.2.2	Website menu item - Booking
5.2.3	Website menu item - About Us
5.2.4	Website menu item - Contact Us
5.3	Booking
5.3.1	Booking - Name
5.3.2	Booking - Surname
5.3.3	Booking - Country
5.3.4	Booking - Cellphone number
5.3.5	Booking - Additional contact number
5.3.6	Booking - E-mail address
5.3.7	Booking - Date of arrival
5.3.8	Booking - Planned stay duration

5.1	Administrator login
This use case defines the process of logging the admin into the back-end of the website.
5.1.1	Notes
1.	The administrator can log into the back-end of the website from any web browser that can display the website as long as a connection can be made to the server containing the website.
2.	The administrator log in will be hidden and can only be accessed by directly typing the path into the web-browser.
5.1.2	Actors
Administrator
5.1.3	Pre-Conditions
The website must be properly set up and online on the internet for the administrator to access it or it must be properly installed on a server for local access.
5.1.4	Post-Conditions
Administrator logged-in to back-end able to make changes to the website.
5.1.5	Administrator login
5.1.6	“Used” Use Cases

5.2	Website Menu
This use case defines what each web page link is for and does.
5.2.1	Notes
1.	The links to the pages will be displayed as buttons with text within the outlines of the buttons.
2.	The user will need to click on the buttons to load the pages.
5.2.2	Actors
1.	User
5.2.3	Pre-Conditions
1.	The website must be deployed on the internet and accessible by users.
2.	For testing purposes a prototype of the website shall be deployed on a computer used as a server and also containing a database to test the website features.
5.2.4	Post Conditions
Displayed webpage that the user clicked on.
5.2.5.0	Menu Items
This section contains a list of the Menu Items used for navigation of the Website’s webpages.
5.2.5.1	Home Page
Display the main webpage.
5.2.5.2	Booking
Display the webpage containing the booking functions.
5.2.5.3	About Us
Display the webpage containing the purpose of the website. 
5.2.5.4	Contact Us
Display the webpage with contact information about the authors/owners of the website. 
5.3	Booking 
This use case defines the fields the user must fill in order to place a booking.
5.3.5.0	Notes
1.	It is assumed that the email text field be made optional in-case of the small chance of a user not actually having an email. Thus the user could receive verification of booking via SMS to a cellphone.
2.	The text fields E-mail Address, Cellphone number, and Alternative Contact Number should be a combination where at least ONE of the fields shall be required.
3.	The text fields Name, Surname, Date of Arrival, and Planned Stay Duration shall all be required.
4.	The text field for Country shall be optional.
5.3.6.0	Actors
1.	User
5.3.7.0	Pre-Conditions
1.	The website must be deployed on the internet and accessible by users.
2.	For testing purposes a prototype of the website shall be deployed on a computer used as a server and also containing a database to test the website features.
5.3.8.0	Post Conditions
Filled out text fields, required and optional, pre-submission to database.
5.3.9.0	Text Fields
This section contains a list of text fields and what the user must enter in each one to place a booking.
5.3.9.1	Name
The name of the user must be entered in this field in the form of plain text.
5.3.9.2	Surname 
The surname of the user must be entered in this field in the form of plain text.
5.3.9.3	Country
The country where the user us currently living (country of residence), entered as plain text.
5.3.9.4 Cellphone number
The cellphone number of the user entered as plain text.
5.3.9.5	Additional Contact Number
An alternative contact number in case the user does not have a cell phone or in case the other contact methods fail. Entered as plain text.
5.3.9.6	E-mail Address
The email of the user entered as plain text.
5.3.9.7	Date of Arrival
The date when the user plans on visiting the physical advertised booked event. Entered as plain text.
5.3.9.8	Planned Stay Duration
The duration in days the user plans on visiting.
6.0	Database Design
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
7.0	User Interface
7.1	Menu Design
The website shall contain menus as set out in section 5.2.5.0 of this document. The menu will be displayed on each page allowing the user to navigate the Website’s webpages. The “Home Page” shall be displayed on initial access of the Website.
Menu Items:
1.	Home Page
2.	Booking
3.	About Us
4.	Contact Us
8.0	Issues
This section contains the currently unsolved issues.
