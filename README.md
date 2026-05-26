# mobile-app-project-
Event Discovery and Ticket Booking System

GROUP MEMBERS                                        ID NUMBER                               group   
1. Beamlack Kedir                                    Ugr/33995/16                            4
2. Sena Birhanu                                      Ugr/35392/16                            4
3. Tigist Tesfaye                                    Ugr/35503/16                            3
4. Umera addisu                                      Ugr/35538/16                            3
5. Wintana yewnet                                    Ugr/35557/16                            3


         ABSTRACT

   
The Event Discovery & Ticket Booking System is a modern mobile-based platform developed to simplify event discovery, ticket booking, QR-based ticket validation, and event management. The application addresses common problems in traditional event systems such as ticket fraud, poor event visibility, manual registration processes, and inefficient attendee tracking.
The proposed system provides users with the ability to discover trending events, search by category and location, book tickets securely, receive QR-coded tickets, and receive notifications regarding upcoming events.
The platform also supports organizers through dashboards that allow event creation, attendee monitoring, analytics tracking, and QR-based ticket verification.
The system is implemented using Flutter for the frontend, java for the backend and mysql for database management, Firebase Cloud Messaging for notifications.
 
 
          CHAPTER 1 INTRODUCTION

        
    1.1 Background

    
Event management and ticket booking systems have evolved rapidly with the advancement of mobile technology. Traditional methods of event promotion and ticket sales rely heavily on manual operations, paper tickets, and physical attendance verification.
Modern users demand fast, secure, and mobile-first experiences.
This project introduces a smart digital event platform that automates:
  •	Event discovery
  •	Ticket booking
  •	QR validation
  •	Notifications
  •	Analytics
  •	Event management
                            
      1.2 Problem Definition
Traditional event systems suffer from:
  •	Ticket fraud
  •	Lack of centralized event discovery
  •	Manual attendee management
  •	Poor communication between organizers and attendees
  •	Long registration queues
  •	Limited analytics
  •	Duplicate ticket issues
               
            1.3 Objectives
  General Objective
Develop a secure and scalable mobile-based event discovery and ticket booking system.
Specific Objectives
  •	Allow users to discover events
  •	Enable secure ticket booking
  •	Generate QR-code tickets
  •	Validate tickets using QR scanning
  •	Notify users about events
  •	Allow organizers to manage events
  •	Prevent duplicate ticket usage
          
          1.4 Scope
Included
  •	Mobile application
  •	Organizer dashboard
  •	QR validation
  •	Authentication
  •	Notifications
  •	Booking management

 
         
         CHAPTER 2: LITERATURE REVIEW
Existing Systems
Eventbrite
Strengths:
•	Large marketplace
•	Online ticket sales
Weaknesses:
•	High service fees
•	Complex organizer tools
Meetup
Strengths:
•	Community engagement
Weaknesses:
•	Limited ticketing capabilities
Facebook Events
Strengths:
•	Massive audience reach
Weaknesses:
•	Weak ticket validation
•	Fraud vulnerabilities
Research Findings
Modern event systems require:
•	Mobile-first UX
•	Real-time notifications
•	Secure digital tickets
•	QR validation
•	Scalable cloud infrastructure

 
      
       CHAPTER 3: SYSTEM ANALYSIS
     3.1 Existing System Analysis
Problems Identified
Problem	Impact
Manual ticketing	 Slow operations
Fake tickets	 Revenue loss
Poor event visibility	 Low attendance
Manual validation	 Long queues
Lack of analytics	 Poor decisions

     3.2 Proposed System
The proposed solution introduces:
•	Mobile-based event discovery
•	Secure authentication
•	QR-based validation
•	Real-time notifications
•	Organizer dashboard
•	Cloud-based scalability


     3.3 Functional Requirements
User Functions
•	Register
•	Login
•	Search events
•	Book tickets
•	Download tickets
•	Receive notifications
•	View booking history
Organizer Functions
•	Create events
•	Edit events
•	Cancel events
•	Scan QR tickets
•	View analytics
Admin Functions
•	Manage users
•	Monitor events
•	Handle reports


     3.4 Non-Functional Requirements

Requirement	Description
Performance	 Fast response time
Scalability	 Cloud-ready architecture
Security	 JWT authentication
Reliability	 Fault-tolerant APIs
Usability	 User-friendly UI
Maintainability	 Clean architecture

     3.5 Feasibility Study
Technical Feasibility
The system can be implemented using Flutter, java, mySQL, Firebase, and cloud hosting.
Economic Feasibility
Open-source tools reduce development cost.
Operational Feasibility
Users already utilize smartphones for digital services.

     3.6 Risk Analysis

Risk	 Mitigation
Fake QR codes	 Encrypted QR validation
Network failure	Offline caching
Duplicate booking	Unique constraints
Payment fraud	Transaction verification
Server downtime	Cloud deployment

     3.7 Edge Cases
Edge Case	Solution
Sold-out events	Disable booking
Duplicate scans	Mark QR as used
Expired tickets	Validation timestamps
Offline mode	Local storage caching
Event cancellation	Push notifications

    USER RESEARCH
    Interview Questions
Event Organizers
1.	How do you currently manage ticket sales?
2.	What are your biggest event management challenges?
3.	Have you experienced ticket fraud?
4.	What tools do you use for promotions?
5.	What analytics are important to you?
Event Attendees
1.	How do you discover events?
2.	What booking issues do you face?
3.	Have you ever received fake tickets?
4.	What features do you expect in event apps?
5.	How important are notifications?

Sample Interview Findings
Organizer Findings
Organizer	Major Pain Point
Organizer 1	Ticket fraud
Organizer 2	Manual attendee tracking
Organizer 3	Poor promotions
Organizer 4	Low attendance
Organizer 5	Payment verification
User Findings
User	Major Pain Point
User 1	Difficult discovery
User 2	Fake tickets
User 3	No reminders
User 4	Long queues
User 5	Complex booking

User Personas
Persona 1: Event Attendee
•	Age: 23
•	Occupation: Student
•	Goal: Quickly discover affordable events
•	Pain Point: Missing events due to lack of notifications
Persona 2: Event Organizer
•	Age: 35
•	Occupation: Event Manager
•	Goal: Increase ticket sales
•	Pain Point: Ticket fraud and attendee management


Empathy Map
Thinks
•	Is this ticket valid?
•	Are there seats available?
Feels
•	Excited about events
•	Frustrated by fake tickets
Says
•	Booking should be easier
Does
•	Searches events online
•	Shares tickets with friends

 
      
       CHAPTER 4: SYSTEM DESIGN
     4.1 System Architecture
Architecture Layers
1.	Presentation Layer (Flutter)
2.	Business Logic Layer
3.	API Layer
4.	Database Layer
5.	Cloud Services

         4.2 Use Cases
Main Use Cases
•	Register User
•	Login
•	Discover Events
•	Book Ticket
•	Scan QR Code
•	Validate Ticket
•	Manage Events

     4.3 User Flow
User Registration → Login → Browse Events → Event Detail → Ticket Booking → Payment → QR Ticket → Event Entry → QR Validation

     4.4 Activity Diagram Description
1.	User opens app
2.	Searches event
3.	Selects ticket quantity
4.	Confirms booking
5.	QR generated
6.	Organizer scans QR
7.	System validates ticket

        4.5 Sequence Diagram Description
User → Flutter App → API Server → Database → Payment Module → QR Generator → Notification Service

     4.6 Data Flow Diagram
Level 0
User ↔ Mobile App ↔ Backend ↔ Database
Level 1
Authentication Process Booking Process QR Validation Process Notification Process

     4.7 ERD
Entities
Users
•	id
•	name
•	email
•	password
•	role
Events
•	id
•	organizer_id
•	title
•	description
•	date
•	venue
•	price
•	available_seats
Bookings
•	id
•	user_id
•	event_id
•	quantity
•	qr_code
•	status
Tickets
•	id
•	booking_id
•	qr_hash
•	validation_status
API DESIGN
Authentication APIs
Register
POST /api/auth/register
Login
POST /api/auth/login
Google Login
POST /api/auth/google


  Event APIs
Get All Events
GET /api/events
Create Event
POST /api/events
Update Event
PUT /api/events/:id
Delete Event
DELETE /api/events/:id
Booking APIs
Create Booking
POST /api/bookings
Get User Bookings
GET /api/bookings/user
Validate QR
POST /api/bookings/validate

     CHAPTER 5: IMPLEMENTATION
      5.1 Development Environment
The system was developed using the following software tools and technologies:
Component	Technology Used
Frontend Framework	Flutter
Frontend Language	Dart
Backend Framework	Node.js + Express.js
Backend Language	Java
Database	mysql
IDE	Visual Studio Code
API Testing	Postman
Version Control	Git + GitHub
Authentication	JWT + Google Authentication
Notifications	Firebase Cloud Messaging
QR Technology	qr_flutter + mobile_scanner

      5.2 System Implementation Overview
The implementation phase transformed the system design into a fully functional mobile application and backend service.
The project implementation was divided into the following modules:
1.	Authentication Module
2.	Event Discovery Module
3.	Booking Module
4.	QR Validation Module
5.	Organizer Dashboard Module
6.	Notification Module
7.	Booking History Module

          5.3 Frontend Implementation (Flutter)
The frontend application was implemented using Flutter with Clean Architecture principles.
      
      5.4 Authentication Module Implementation
The authentication module allows users to:
•	Register accounts
•	Login securely
•	Reset passwords
•	Access protected resources
Authentication Features
Feature	Description
User Registration	Create user accounts
JWT Authentication	Secure login tokens
Google Login	OAuth authentication
Session Management	Persistent login state


     5.5 Event Discovery Module Implementation
The event discovery module enables users to browse and search for events.
Features Implemented
•	Event listing
•	Event categories
•	Search functionality
•	Trending events
•	Event detail pages
            
            5.6 Booking Module Implementation
The booking module enables users to reserve event tickets.
Booking Workflow
1.	User selects an event
2.	User chooses ticket quantity
3.	System checks seat availability
4.	Booking is confirmed

        5.7 QR Validation Module Implementation
The QR validation system prevents ticket fraud and duplicate ticket usage.
Validation Process
The backend verifies:
•	Ticket existence
•	Ticket expiration
•	Duplicate scans
•	Booking ownership

        5.8 Organizer Dashboard Implementation
The organizer dashboard enables event organizers to:
•	Create events
•	Edit events
•	View attendees
•	Scan tickets
•	View analytics
Dashboard Features
Feature	Description
Event Creation	Add new events
Attendee Tracking	Monitor attendees
Ticket Validation	Scan QR tickets
Analytics	View booking statistics
          
           5.9 Backend Implementation
The backend system was developed using java.
          
           5.10 Notification System Implementation
Firebase Cloud Messaging (FCM) was integrated for push notifications.
Notifications Included
•	Booking confirmation
•	Event reminders
•	Event cancellation alerts
•	Promotional updates



     5.11 Error Handling Implementation
The system handles common runtime errors gracefully.
Errors Handled
Error	Solution
Invalid login	Error message displayed
Network failure	Retry mechanism
Duplicate booking	Request blocked
Expired ticket	Validation failed
Sold-out event	Booking disabled


     Chapter six : TESTING
      Unit Testing
Test Case	Expected Result
Login with valid credentials	Success
Invalid password	Error message
Duplicate booking	Blocked
Expired QR	Validation failed



API Testing
Tools:
•	Postman
•	Thunder Client

UI Testing
Test:
•	Responsiveness
•	Dark mode
•	Accessibility
<img width="1080" height="2400" alt="1" src="https://github.com/user-attachments/assets/75413611-a70b-450d-98ae-57bfbf869a25" />
<img width="1080" height="2400" alt="2" src="https://github.com/user-attachments/assets/4ac25abf-a3d6-430f-886f-39a65d5ccf2a" />
<img width="1080" height="2400" alt="4" src="https://github.com/user-attachments/assets/4e4025e6-8891-4ca1-b750-e54f86788f77" />
<img width="1080" height="2400" alt="3" src="https://github.com/user-attachments/assets/5c62f80d-150c-46ff-97cd-b1e9b9d5c198" />
<img width="1080" height="2400" alt="5" src="https://github.com/user-attachments/assets/095827cb-bffe-4cf2-a11c-0474cb8ad2f4" />
<img width="720" height="1600" alt="6" src="https://github.com/user-attachments/assets/76279129-000a-434d-8028-1ecb7aa3eba4" />
<img width="1080" height="2400" alt="7" src="https://github.com/user-attachments/assets/721b43d1-5e74-4306-a2d6-9c52bcec6fea" />
<img width="1080" height="2400" alt="8" src="https://github.com/user-attachments/assets/c5528070-3ac1-4a7f-ab15-3b61de201021" />
<img width="720" height="1600" alt="9" src="https://github.com/user-attachments/assets/69b58d45-84cf-4551-b066-049acecc8d26" />
<img width="720" height="1600" alt="10" src="https://github.com/user-attachments/assets/67b73d63-4e8f-4925-96ce-a0e6f2c4dd91" />
<img width="720" height="1600" alt="11" src="https://github.com/user-attachments/assets/33a17f22-ce63-465b-baa6-048d38704c22" />
<img width="1080" height="2400" alt="12" src="https://github.com/user-attachments/assets/fe10a8cc-5c28-43d2-adcd-1c8da61a1874" />
<img width="1080" height="2400" alt="13" src="https://github.com/user-attachments/assets/8a58172e-ead6-4a1c-a4b2-ae67dcf1c976" />
<img width="1080" height="2400" alt="15" src="https://github.com/user-attachments/assets/0400474b-87a5-4ce3-b75d-d7dc0f3cdfbf" />
<img width="720" height="1600" alt="16" src="https://github.com/user-attachments/assets/9a9db0c0-2b95-4e55-b39a-7d8dcea184d9" />























