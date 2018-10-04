# Requirements Document
### Contents
1. [Introduction](#1)
2. [User Requirements](#2) <br>
  2.1. [Software Interfaces](#2.1) <br>
  2.2. [User Interfaces](#2.2) <br>
  2.3. [User Characteristics](#2.3) <br>
  2.4. [Assumptions and Dependencies](#2.4) <br>
3. [System Requirements](#3.) <br>
  3.1 [Functional Requirements](#3.1) <br>
  3.2 [Non-Functional Requierements](#3.2) <br>
    3.2.1 [Software Quality Attributes](#3.2.1) <br>
    3.2.1.1 [External Quality Criteria](#3.2.1.1) <br>
    3.2.1.2 [Internal Quality Criteria](#3.2.1.2) <br>
4. [Analogues](#4) <br>

### Glossary
* Web application - a client-server application in which the client interacts with the server using a browser, and the web server is responsible for the server.

### 1\. Intoduction <a name="1"></a>
There are many web applications for working with a database of contacts, but most of them have a high server load, due to the large amount of unnecessary functionality.

To solve this problem, this web application was created.

### 2\. User Requirements <a name="2"></a>
#### 2.1\. Software Interfaces <a name="2.1"></a>
The project uses the Spring MVC framework and does not interact with external systems and services.
#### 2.2\. User Interfaces <a name="2.2"></a>
The graphical interface of the project is presented using the mocaps [home page](https://raw.githubusercontent.com/evgenyv13/TRiTPO/master/LR2/ContactBook/docs/Project%20Documentation/mockups/mainpage.png) and [contact edit page](https://raw.githubusercontent.com/evgenyv13/TRiTPO/master/LR2/ContactBook/docs/Project%20Documentation/mockups/editpage.png).
The main window requires a separate view:

Button | Event
--- | ---
"Contact List" | Go to the main page of the web-site
"Search" | Opens modal window containing fields for finding a user.
"Send Message" | Opens modal window allowing you to send a message to selected contacts.
Create Contact | Opens modal window allowing you to create a new contact.
"Delete Contact (s)" | Delete selected contacts
"Username" | Go to the view and edit contact information page.

#### 2.3\. User Characteristics <a name="2.3"></a>
Target Audios:
* Users who need to work with contact details of employees.
#### 2.4\. Assumptions and Dependencies <a name="2.4"></a>
* When running this project on Tomcat Server, you must use Tomcat 9.0 and higher, due to the fact that the Spring MVC framework is not supported by lower versions.
### 3\. System Requirements <a name="3"></a>
Run the application on the following operating systems:
* Windows
* Linux
#### 3.1\. Functional Requirements <a name="3.1"></a>
The user is given the opportunities provided in the table.

Function | Requirements
--- | ---
Adding a new contact | The application should provide the user the ability to add a new contact, when you click on the "Create Contact" button
Delete selected contacts | The application should provide the ability to delete the selected contacts, when you click on the button "Delete contact (s)"
Sending messages to contacts | The application must provide the ability to send messages to @mail to selected contacts, with the ability to automatically substitute the first name / last name / patronymic of the contact.
Contact Search | The application must provide the ability to search for a contact by: name, surname, patronymic, date of birth, address.
Work with contact uploads | The application should provide the ability to add files to the contact, and further download these files.

#### 3.2\. Non-Functional Requierements <a name="3.2"></a>
##### 3.2.1\. Software Quality Attributes <a name="3.2.1"></a>
##### 3.2.1.1 External Quality Criteria <a name="3.2.1.1"></a>
Important external criteria for this application are: quick start, low resource consumption and high performance, namely fast page load.
##### 3.2.1.2 Internal Quality Criteria <a name="3.2.1.2"></a>
Internal criteria are: ease of use due to the minimal interface, fast page refresh rate, due to partial download, portability between Windows and Linux systems.
### 4\. Analogues <a name="4"></a>
This project is in some way a simplified version of ["Microsoft Outlook"](https://account.microsoft.com/account/outlook), which greatly simplifies use.
