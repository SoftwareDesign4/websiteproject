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

## 3.7 Joomla API  

  
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
  
