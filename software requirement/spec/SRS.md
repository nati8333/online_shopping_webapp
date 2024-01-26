# Online Shopping Web-app Software Requirement Specification

<html><br/><br/></html>

| University             | **ADAMA SCIENCE AND TECHNOLOGY UNIVERSITY**         |
| ---------------------- | ----------------------------------------------------|
| School                 | **Electrical Engineering and Computing**            |
| Department             | **Computer Science and Engineering**                |
| Course                 | **Fundamentals of Software Engineering (CSEg3201)** |
| Semester Project Title | **Online Shopping Web-app**                         |
| Academic Year          | **2023/2024 G.C**                                   |
| Semester               | **1**                                               |
| Section                | **3**                                               |

<html><br/><br/></html>

| GROUP MEMBER   | ID           |
| -------------- | ------------ |
| Natnael Eshetu | A/UR5111/09  |
| Dawit Ashenafi | UGR/25404/14 |
| Abdi Dawud     | UGR/25390/14 |
| Sumeya Awel    | UGR/26377/14 |
| Eden Wekele    | UGR/25834/14 |

<html><br/><br/><br/><br/><br/><br/><br/><br/></html>

## Table of Contents

- [Online Shopping Web-app Software Requirement Specification](#online-shopping-web-app-software-requirement-specification)
- [Acknowledgement](#acknowledgment)
- [Definitions and Abbreviations](#definitions-and-abbreviations)
  - [Definitions](#definitions)
  - [Abbreviations](#abbreviations)
- [Chapter 1](#chapter-1)
  - [1.1 Introduction](#1.1-introduction)
  - [1.2 Background of the Project](#1.2-background-of-the-project)
  - [1.4 Justification of the Project](#1.4-justification-of-the-project)
  - [1.5 Objective of the Project](#1.5-objective-of-the-project)
    - [1.5.1 General Objectives](#1.5.1-general-objectives)
    - [1.5.2 Specific Objectives](#1.5.2-specific-objectives)
  - [1.6 Scope and Limitations](#1.6-scope-and-limitations)
    - [1.6.1 Scope of the Project](#1.6.1-scope-of-the-project)
    - [1.6.2 Limitations of the Project](#1.6.2-limitations-of-the-project)
  - [1.7 Feasibility Study](#1.7-feasibility-study)
    - [1.7.1 Technical Feasibility](#1.7.1-technical-feasibility)
    - [1.7.2 Operational Feasibility](#1.7.2-operational-feasibility)
    - [1.7.3 Economic Feasibility](#1.7.3-economic-feasibility)
  - [1.8 Significance of the Project](#1.8-significance-of-the-project)
  - [1.9 Beneficiaries of the Project](#1.9-beneficiaries-of-the-project)
  - [1.10 Methodology](#1.10-methodology)
  - [1.11 Development Tools](#1.11-development-tools)
    - [1.11.1 Hardware Tools](#1.11.1-hardware-tools)
    - [1.11.2 Software Tools](#1.11.2-software-tools)
- [Chapter 2 | Description of Existing Systems](#chapter-2--description-of-existing-systems)
  - [2.1 Major Functionality of Existing Systems](#2.1-major-functionality-of-existing-systems)
  - [2.2 Users of the Existing Systems](#2.2-users-of-the-existing-systems)
  - [2.3 Drawbacks of the Existing Systems](#2.3-drawbacks-of-the-existing-systems)
  - [2.4 Business Rule](#2.4-business-rule)
- [Chapter 3 | Proposed System](#chapter-3--proposed-system)
  - [3.1 Overview](#3.1-overview)
  - [3.2 Functional Requirements](#3.2-functional-requirements)
  - [3.3 Non-functional Requirements](#3.3-non-functional-requirements)
    - [3.3.1 User Interface](#3.3.1-user-interface)
    - [3.3.2 Performance Considerations](#3.3.2-performance-considerations)
    - [3.3.3 Reliability](#3.3.3-reliability)
    - [3.3.4 Error Handling](#3.3.4-error-handling)
    - [3.3.5 Security](#3.3.5-security)
  - [3.4 System Model](#3.4-system-model)
    - [3.4.1 Scenarios](#3.4.1-scenarios)
    - [3.4.2 Use Case Model](#3.4.2-use-case-model)

## Acknowledgment

Thanks to our FSE teacher for giving us this opportunity to do this project and for teaching and guiding us on how to do this project. Thanks to Alemu Tadesse for advising us and giving us feedback on the UML diagrams. 

## Definitions and Abbreviations

### Definitions

### Abbreviations

| ABBREVIATION | DESCRIPTION                          |
| ------------ | ------------------------------------ |
| FSE          | Fundamentals of Software Engineering |
| SRS          | Software Requirements Specification  |
| API          | Application Programming Interface    |
| PHP          | Hypertext Preprocessor    |

## Chapter 1

### 1.1 Introduction

We live in the modern age of computer technology. Even though the act of purchasing and online shopping does not have a long track record, it is the fastest growing and dominating business model and technology area. Companies like Amazon, Alibaba, eBay, and Walmart currently dominate the market. However, online shopping is not very common in our country, and we can understand the potential of this business in our country's case. It is significant to develop a proper system that could resolve the current online shopping drawbacks.

The main geographical target of this project is our beloved country Ethiopia. We aim to design and implement a reliable online shopping system for local use here in Ethiopia.

### 1.2 Background of the Project

Online shopping is a form of electronic commerce that allows consumers to buy goods or services from sellers over the Internet using a web browser or a mobile app. Online shopping has become a popular and convenient way of shopping for millions of people around the world, especially with the development of various online platforms, payment methods, and delivery services. However, online shopping did not emerge overnight; it has a history that dates to the late 1970s.

The growth of online shopping was further boosted by the invention of the World Wide Web in 1990 by Tim Berners-Lee, who also created the first web browser. The World Wide Web made it possible for users to access information and resources from different servers and locations. In 1994, Netscape developed a security protocol called SSL (Secure Sockets Layer) that encrypted the data exchanged between web browsers and web servers, making online transactions more secure and reliable. In the same year, the first online marketplaces, such as Amazon.com and eBay, were launched, offering a wide range of products and services to online shoppers. Since then, online shopping has evolved and expanded to include various features, such as comparison shopping, social commerce, mobile commerce, and more.

Online shopping is still in its early stages in Ethiopia, but it is growing rapidly. The COVID-19 pandemic has accelerated the adoption of digital technologies, and the Ethiopian government is taking steps to support the development of e-commerce. A regulation called 'Electronic Transaction' that provides a legal framework for Electronic Commerce (E-commerce) and other related aspects including e-receipts is in the final approval process. The long-awaited Payment instrument Issuers directives that were expected to open the mobile money and fintech space for non-banks and MFIs are issued now. Ethio Telecom or any other local Fin-tech start-ups and companies can operate legally. This will definitively add to the dynamics of the Fintech landscape and hopefully provide more and better avenues for people to buy online.

There are a few e-commerce websites and apps in Ethiopia that are worth exploring. Shega is a website that provides a list of e-commerce websites and apps in Ethiopia. Addis Mercato is an online marketplace that offers a wide range of products from supermarkets and stores in town.

### 1.3 Statement of the Problem

The main issues of online shopping in Ethiopia are accountability and legal processes, security, delivery, and a money back guarantee on failure or conflict. The proposed software solution aims to solve these issues.

- **Accountability and legal processes:**
Accountability should be taken for handling items and money with proper legal processes prepared to handle all cases. Customers and vendors would like to have the legal processes handled by the company with less of their involvement. Also, the company should ensure that vendors comply with local laws and regulations.
- **Security issues:**
Some vendors might try to scam customers and create multiple accounts. The company should verify vendors' and customers' existence to avoid scams.The system must be designed to protect unauthorized identity information access and must keep backups.
- **Delivery issues:**
Accidents or conflicts might arise during delivery of items. The company ought to have a system in place to handle this.As for thefts during delivery the deliverer ought to be accountable.
- **Money Back Guarantee on Failure or Conflict:**
Local payment methods such as CBE Birr, Amole, Tele birr, and M-Birr do not provide an API for a 2-phase payment system in which paid money is reserved until completion of item transaction either in success or failure. Customers would like to have the guarantee of their money being returned back safely, and without beurocracy, to them on failure.
- **Internet Issues:**
Internet requirement is unavoidable but the system might be overloaded with command and fetch requests. The more resource files need to be transferred the more load the system will take thus the slower the service.

The proposed software solution should be user-friendly, secure, and scalable. The system should be able to handle many users and transactions simultaneously. The platform should provide a good shopping experience to customers, allowing them to browse through different categories of products, add items to their cart, and make payments securely. The system should also provide vendors with a inventory management system, and track their sales. The platform should be accessible from desktop and mobile devices.

### 1.4 Justification of the Project

It is best to make this project as no local system provides a solution for all  the issues mentioned in the problem statement and the ones that do are not local and do not support local payment or delivery.

### 1.5 Objective of the Project

#### 1.5.1 General Objectives

Generally, our objective is to create a desirable, competent, secure, and reliable local online shopping software system for use in Ethiopia.

#### 1.5.2 Specific Objectives

Our specific objectives are:

- To create a functional online shopping system within the given time-frame.
- To incrementally and iteratively design and build the system.
- To simultaneously work on this project for maximum efficiency.
- To continuously, analyze and improve requirements and this specification document.
- To analyze, design, and implement features prioritized based on importance.

### 1.6 Scope and Limitations

#### 1.6.1 Scope of the Project

In this project, we only focus on developing a country-local system.

#### 1.6.2 Limitations of the Project

These are the limitations of this project:

- The software system will not work internationally.
- Internet access and a modern browser is required.
- Less than one month to finish this project.

### 1.7 Feasibility Study

#### 1.7.1 Technical Feasibility

#### 1.7.2 Operational Feasibility

#### 1.7.3 Economic Feasibility

### 1.8 Significance of the Project

This project is significant because:

- It makes it easier to find the items we want to buy and their details using modern technology.
- It will be trustworthy and involves the least legal processes and worries to customers.
- It will be most demanded in large cities such as Addis Abeba.

### 1.9 Beneficiaries of the Project

The beneficiaries of this project are:

- Stakeholders who invest in this project.
- Vendors who want to keep track of their inventory and sell online.
- Customers who want to purchase online and have items delivered.
- Employees, such as Managers and couriers.

### 1.10 Methodology

### 1.11 Development Tools

#### 1.11.1 Hardware Tools

- Personal Computers: Laptops.
- Peripherals: Wireless Mouse
- Smart Phones: For communication and file sharing.

#### 1.11.2 Software Tools

- WPS Office: for editing word documents.
- VSCode: for coding and general text editing.
- Draw.io: for designing modeling diagrams.
- Microsoft Edge, Google Chrome: for testing and debugging webapp.

## Chapter 2 | Description of Existing Systems

### 2.1 Major Functionality of Existing Systems

- **Product browsing and search:**
Products are organized into easily navigable categories and subcategories, like electronics, clothing, groceries, etc. Users can search for specific products using keywords or filters. Detailed product pages include descriptions, specifications, images, and sometimes even videos.
- **Ordering and payment:**
Users can add items to their cart and review them before checkout. Online shopping platforms integrate with secure payment gateways for credit card, debit card, and mobile money transactions. Many platforms offer COD as an alternative payment option for users who prefer not to pay online.
- **Account management:**
Users can create accounts to track their orders, save addresses, and manage preferences. Users can track the status of their orders in real-time. Users can create wish-lists for future purchases or share them with others.
- **Additional features:**
Users can read reviews and ratings from other customers before making a purchase. Platforms often offer coupons, promo codes, and flash sales to attract customers. Online shopping platforms offer customer support via live chat, email, or phone to answer questions and resolve issues.

### 2.2 Users of the Existing Systems

### 2.3 Drawbacks of the Existing Systems

### 2.4 Business Rule

## Chapter 3 | Proposed System

### 3.1 Overview

### 3.2 Functional Requirements

### 3.3 Non-functional Requirements

#### 3.3.1 User Interface

#### 3.3.2 Performance Considerations

The system has to be able to handle many requests as fast as possible. This means less data transfer balanced with less processing time. Rather than use a backend page generator like PHP to generate dynamic pages it might be best to generate the page on the frontend using libraries such as React.js and get the necessary data from the server using requests. The former takes more processing time on the backend server while the later takes less processing time on the backend server.

#### 3.3.3 Reliability

#### 3.3.4 Error Handling

Three types of errors are expected to occur in this system.

- Errors regarding user input mistakes and validation
- Errors on the frontend client
- Errors on the backend server

Errors regarding user input mistakes and validation should to be handled on the frontend and backend. On the frontend users should be notified of their input mistakes and errors and must enter valid inputs before this input data can be sent to the server. And on the backend server the data assumed to be valid must be checked and validated for exploitive and harmful attacks such as SQL injections.

Errors on the frontend client include errors such as errors regarding data fetching, errors regarding data presentation. These are errors related to the frontend library and fetching data from the server. Proper handling of this type of errors
must be implemented to provide a good user experience. For example upon fetching error an error indicator must be provided in place of where the fetched data is supposed to be populated.

Errors on the backend server include unhandled exceptions and mistakes that cause the server to crash under some circumstances. Backend developers must handle all exceptions properly and avoid mistakes that would cause the server to crash. Tests should be prepared and done where possible.

#### 3.3.5 Security

The security concerns to be considered for this system are creating secure connections between client and server, secure storage of password and other sensitive data, preventing SQL injections, detecting and dealing with attacks such as DDoS attacks, differentiating between bots and real users and blocking bots from spamming.

Secure connections need to be made between the client and server in order to transfer all sensitive data securely. This is a solved problem in the web-development industry. And that solution is the `https` protocol, and it is the safest way to transfer sensitive data over the internet.

Secure storage of password can be done using good hashing. Since a password only needs to be verified on the backend server it does not need to be stored in as is. A password can be hashed and stored. Since it is very difficult to calculate the password from the hash it is best to store passwords hashed. And when there is a security fault or breach there can be enough time for users to change their passwords and secure their accounts.

As for other sensitive data where hashing is not an option the security concern is at the host and how the admins are accessing the host. Thus a strong password and multi-factor authentication should be used.

To prevent SQL and other forms of injections on the backend security measures must be taken when handling requests to detect and reject requests containing injected data.

DDoS attacks are deadly to the system's service. Measure must be taken to detect and prevent DDoS attacks such as timeouts.

Bots and spamming can be prevented using Captchas.

### 3.4 System Model

#### 3.4.1 Scenarios

##### 3.4.1.1 Scenario for registering in the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously.
- **Normal flow of events:**
    The user enters their full name, password, email, phone number, address and attach documents that prove national identity such as national ID or passport, then clicks on register. After that the registration information is stored on the back-end temporarily until validated and verified. A verify account registration email is sent to the provided email address. The user opens their email and clicks on the verify link which then completes the registration. If the identity verification attachment is verified to be valid then the user will be registered in the system.
- **What can go wrong:**
    The user enters passwords that do not match. The user should be notified on the page and must enter matching passwords. The user enters an invalid information. The user should be notified on the page and must enter a valid information.The user provides an invalid identity verification attachment. The user must be notified and must be given a form to provide a valid identity verification attachment through a link sent via email.
- **System state on completion:**
    The user is registered successfully in the system. The user information provided is stored on a database in the system. The password is hashed before storing.

##### 3.4.1.2 Scenario for logging in into the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously.
- **Normal flow of events:**
    The user enters email and password and clicks on login. The email and password are validated on the page and then requested to be verified on the back-end. On successful validation and verification the user will be logged in.
- **What can go wrong:**
    User enters invalid email or password. The user is notified on the page and must enter a valid email and password.User is not registered on the system using the provided email. User must be notified on the page and must either register first or enter the email address they registered.
- **System state on completion:**
    The back-end server creates a session and the session cookie is stored on the browser used for automatic login until expiry date.

##### 3.4.1.3 Scenario for resetting password

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously. And they are trying to login but they forgot their password.
- **Normal flow of events:**
    The user clicks on forgot password and is provided with a reset password form in which they must enter their email address. After which the email address is validated and verified and then a password reset link is sent via the email. The user opens their email and clicks on the password reset link which leads to a password reset form. Then they must enter a new password and click on reset.
- **What can go wrong:**
    The user enters an invalid email address. The user must be notified on the page and must enter a valid email.The user enters an email that has not been registered on the system. The user must be notified on the page and must register or contact support.The user does not enter a matching password. The user must be notified on the page and must enter matching passwords.
- **System state on completion:**
    The password is hashed and then updated on the database.

##### 3.4.1.4 Scenario for logging out of the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The user clicks on logout and they are logged out of the system.
- **System state on completion:**
    The session is destroyed. And the session cookie is discarded.

##### 3.4.1.5 Scenario for an administrator registering an employee in the system

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on register employee which opens the employee registration form. The administrator enters the information required and clicks on register. The employee information is then verified.
- **What can go wrong:**
    The administrator enters an invalid information. The administrator must be notified on the page and must enter a valid information.
- **System state on completion:**
    The employee information is stored on the database.

##### 3.4.1.6 Scenario for an administrator firing an employee

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on remove employee which opens the employee firing form. The administrator filters and searches for the employee they need to fire from the list of employees and click on fire. The administrator is then prompted for reason of firing and must enter a reason and click on continue. The employee is then notified of their new status.
- **What can go wrong:**
    The administrator needs to undo the firing process. They can only undo the firing process before the employee information is archived after a certain amount of time.
- **System state on completion:**
    The employee information on the database is marked as fired and archived after a certain amount of time.

##### 3.4.1.7 Scenario for an administrator setting the salary of an employee

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on set employee salary which opens the employee list form. The administrator filters and searches for the employees they need to set salary for from the list of employees. And then they must select at least one employee before they can click on set salary. The administrator is then prompted for amount of salary and must enter a valid amount and click set salary. The employee is then notified of their new salary.
- **What can go wrong:**
    The administrator enters an invalid amount for salary. They must be notified on the page and must reenter a valid amount for salary.
- **System state on completion:**
    The employee salary information on the database is updated to the new amount.

##### 3.4.1.8 Scenario for a manager registering a courier in the system

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on register courier which opens the courier registration form. The manager enters the information required and clicks on register. The employee information is then verified.
- **What can go wrong:**
    The manager enters an invalid information. The manager must be notified on the page and must enter a valid information.
- **System state on completion:**
    The courier employee information is stored on the database.

##### 3.4.1.9 Scenario for a manager firing a courier

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on remove employee which opens the employee firing form. The manager filters and searches for the courier they need to fire from the list of employees and click on fire. The manager is then prompted for reason of firing and must enter a reason and click continue. The courier is then notified of their new status.
- **What can go wrong:**
    The manager needs to undo the firing process. They can only undo the firing process before the employee information is archived after a certain amount of time.
- **System state on completion:**
    The courier employee information on the database is marked as fired and archived after a certain amount of time.

##### 3.4.1.10 Scenario for a manager assigning a delivery task to a courier

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on view orders which opens the employee orders form. The manager then groups and selects orders by region and area and clicks assign courier. The manager is then provided with a list of the nearest available couriers ordered performance record. Then the manager chooses from this list and clicks on assign. A delivery task is created its status set to assigned, and the selected courier is notified.
- **What can go wrong:**
    There are no couriers available to deliver in that region or area. The manager must retry when couriers are available, or look to hire new couriers to work in that area if there is enough demand.
- **System state on completion:**
    A delivery task is recorded on the database and is properly associated with courier and order.

##### 3.4.1.11 Scenario for a manager handling a failing delivery case

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager is notified of failing delivery cases and follows the notification and views the related order and delivery task. The manager reads and assesses the reason of failure. Then the manager contacts the courier and requests for more information. The manager also calls the customer if required. The manager commands the courier to deliver the items either back to the vendor, or to the company for legal assessment and lawyer advised decision making. If the courier had an accident or cannot deliver then the manager assigns a new delivery task from the failing courier to the vendor or company.
  - **System state on completion:**
    The failing delivery task is recorded as failing with the detailed reason and proof attached to it. And a new delivery task recorded on the database and is properly associated with courier and order.

##### 3.4.1.12 Scenario for a courier viewing assigned delivery task

- **Initial assumption:**
    The  courier has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The  courier is notified of failing delivery cases and follows the notification and views the related order and delivery task. The  courier reads and assesses the reason of failure. Then the  courier contacts the courier and requests for more information. The  courier also calls the customer if required. The  courier commands the courier to deliver the items either back to the vendor, or to the company for legal assessment and lawyer advised decision making. If the courier had an accident or cannot deliver then the  courier assigns a new delivery task from the failing courier to the vendor or company.
- **System state on completion:**
    The failing delivery task is recorded as failing with the detailed reason and proof attached to it. And a new delivery task recorded on the database and is properly associated with courier and order.

#### 3.4.2 Use Case Model

![session-use-case-diagram](media/session-use-case-diagram.drawio.svg)  
![main-use-case-diagram-1](media/main-use-case-diagram-1.drawio.svg)  
![main-use-case-diagram-2](media/main-use-case-diagram-2.drawio.svg)  

### 3.5 Object Model

#### 3.5.1 Data dictionary

### 3.6 Dynamic Model

#### 3.6.1 Class Diagram

#### 3.6.2 Sequence Diagram

#### 3.6.3 Activity Diagram

#### 3.6.4 State Chart Diagram

### Chapter 4 | System Design

### 4.1 Overview

### 4.2 Proposed System Architecture

#### 4.2.1 Subsystem Decomposition

#### 4.2.2 Hardware and Software Mapping

#### 4.2.3 Persistent Data Management

#### 4.2.4 Component Diagram

#### 4.2.5 Database Design

#### 4.2.6 Access Control

#### 4.2.7 User Interface Design

## Chapter 5 | Implementation

### 5.1 Overview

### 5.2 Coding Standard

### 5.3 Development Tools

### 5.4 Prototype

### 5.5 Implementation Detail

## Chapter 6 | Testing

### 6.1 Introduction

### 6.2 Scope

### 6.3 Resources

### 6.4 Schedule

### 6.5 Test Case Scenario

### 6.6 Pass Fail Criteria

### 6.7 Approach

### 6.8 Test Case Specification

### 6.9 Estimated Risk and Contingency Plan

## Chapter 7 | User Manual and Demo

### 7.1 User Manual

### 7.2 Demo

## References

[Node.js SQL Injection Guide Examples and Prevention](https://www.stackhawk.com/blog/node-js-sql-injection-guide-examples-and-prevention/)  
[Best Practices To Prevent DDoS Attacks](https://securityscorecard.com/blog/best-practices-to-prevent-ddos-attacks/)  
[How To Avoid Time-based DDoS Attacks In Node.js](https://www.nearform.com/blog/avoid-time-based-ddos-attacks-node-js/)  
[A quick way for hashing passwords using Bcrypt with Nodejs](https://medium.com/@manishsundriyal/a-quick-way-for-hashing-passwords-using-bcrypt-with-nodejs-8464f9785b67)  