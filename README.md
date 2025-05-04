# airbnb-clone-project
This project is a full-stack clone of the popular accommodation booking platform AirBnB
## Table of contents
### Frontend Development
- [Project initialization](#project-initialization)
- [UI/UX Design Planning](#uiux-design-planning)
- [More UI/UX planning](#more-uiux-planning)
- [Project Roles and Responsibilities](#project-roles-and-responsibilities)
- [UI Component Patterns](#ui-component-patterns)

### Backend development
- [Team roles and responsibilities](#team-roles-and-responsibilities)
- [Technology stack overview](#technology-stack-overview)
- [Database design overview](#database-design-overview)
- [Feature breakdown](#feature-breakdown)
- [API Security overview](#api-security-overview)
- [CI/CD Pipeline Overview](#cicd-pipeline-overview)

## Project initialization
The goal is to build a functional web application that allows users to browse property listings, view detailed property information, and complete bookings. The project will cover frontend development, backend APIs, database design, and deployment.

### Learning Objectives
By completing this project, you will:

- Learn to implement responsive UI/UX designs
- Understand how to structure a complex web application
- Practice working in a team with defined roles
- Develop skills in component-based frontend architecture
- Learn best practices for web application development
### Tech Stack
Frontend: HTML, CSS, JavaScript (React or similar framework)
Version Control: Git and GitHub
Design Tools: Figma for UI/UX design

## UI/UX planning
### Design Goals
- Create intuitive booking flow
- Maintain visual consistency
- Ensure fast loading times
- Prioritize mobile responsiveness
### Key Features
- Property search and filtering
- Detailed property viewing
- Secure checkout process
- User authentication
  ### Primary Pages
  |###Page              |Description|
  |:-------             |:--------:|
  |Property Listing View|Grid display of available properties with filters|
  |Listing Detailed View|Complete property details with images and booking form|
  |Simple Checkout View |Streamlined payment and booking confirmation|
  
### Importance of User-Friendly Design
A well-designed booking system reduces friction in the user journey, increases conversion rates, and improves customer satisfaction. Clear navigation, intuitive interfaces, and responsive design are critical for success.
## More UI/UX planning
### Figma Design Specifications
#### Color Styles:

Primary: #FF5A5F
Secondary: #008489
Background: #FFFFFF
Text: #222222
Secondary Text: #717171

### Typography:
Primary Font: Circular, Medium (500), 16px
Headings: Circular, Bold (700), 24px-32px
Secondary Text: Circular, Book (400), 14px

## Project Roles and Responsibilities
  |###Role              |Responsibilities|
  |:-------             |:--------:|
  |Project Manager      |Oversees timeline, coordinates team, manages deliverables|
  |Frontend Developers  |	Implements UI components, ensures responsive design|
  |Backend Developers   |Builds APIs, manages database, implements business logic|
  |Designers            |	Creates mockups, maintains design system, ensures UX quality|
  |QA/Testers           |Writes test cases, performs testing, reports bugs|
  |DevOps Engineers     |Manages deployment, CI/CD pipeline, server infrastructure| 
  |Product Owner        |Defines requirements, prioritizes features, represents stakeholders|
  |Scrum Master         |Facilitates agile processes, removes blockers, organizes meetings|
  
## UI Component Patterns
### Planned Components
#### Navbar
-Logo
-Search bar
-User navigation
-Responsive menu

#### Property Card
-Property image
-Basic details (price, location, rating)
-Favorite button
-Responsive layout

#### Footer
-Site links
-Company information
-Social media links
-Copyright information
Each component will be designed for reusability and consistency across the application.

## Team Roles and Responsibilities
  |Role                 |Responsibilities|
  |:-------             |:--------:|
  |Project Manager      |- Makes sure a product or its part is delivered on time and within budget<br>- Manages and motivates the software development team|
  |Software Architect   |-	Designs a high-level software architecture<br>- Selects appropriate tools and platforms to implement the product vision<br>- Sets up code quality standards and performs code reviews|
  |Software Developers  |- Engineers and stabilizes the product<br>- Solves any technical problems emerging during the development lifecycle|
  |UI/UX Designers      |- Transforms a product vision into user-friendly designs<br>- Creates user journeys for the best user experience and highest conversion rates|
  |QA/Testers           |- Makes sure an application performs according to requirements<br>- Spots functional and non-functional defects|
  |DevOps Engineers     |- Facilitates cooperation between development and operations teams<br>- Builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery| 
  |Product Owner        |- Holds responsibility for a product vision and evolution<br>- Makes sure the final product meets customer requirements|
  |Business Analyst     |- Understands customer’s business processes<br>- Translates customer business needs into requirements|
  |Test Automation Engineer |- Designs a test automation ecosystem<br>- Writes and maintains test scripts for automated testing|
## Technology Stack Overview
### Backend:
- Java, Kotlin, Python. These were chosen because of the level of security you get while using java, interoperability and the ease of use in pricing models, fraud detection and searching
### Infrastructure:
- MySQL, Apache Kafka, ElasticSearch. MySql was chosen as the primary relational database for data storage, ElastSearch was chosen because it enables full text search and Apache Kafka was chosen because it can be used for a message querry system that processes different things at the same time.
## Database Design Overview
### Users
- Users Names
- Users Contact information
- Users Address
### Properties
- Property locations
- Number of rooms
- Amenities around the property
### Reviews
- Star system to gauge what other people rate the property
- Full sentence reviews on what previous customers liked and did not like
### Payments
- Different options for payment
- A window that directs users to put their card information
- A checkbox confirming they have read the terms and conditions before proceeding with payment
## Feature Breakdown
### User Management
- A database would store user information such as the user's contact information so that they can better manage their bookings
### Property Management
- A database would store information on all the available properties and this database could potentially be accessed through a search narrowed down to area so that the customer gets what they want.
### Booking Systems
This system would be created to semlessly work with the property management database to help customers pick the property they want to stay at.
### Payment Systems
- This system would help the users pay for their stay at any of the properties they have chosen. This system will have to integrate different ways of payment to reach different customers
### Rating Systems
- This would allow people to rate the properties they stayed at based on their experiences and whether they would recommend someone else stay at that property
## API Security Overview
### Rate Limiting
- This would limit the number of bookings being made from the same device or from the same network and help prevent brute force attacks
### Authentication
- This would be required to approve any transaction with money to ensure it is the true owner of the device who is making the purchase
### Using HTTPS
- This would help prevent attacks from any third party as the dat is sent from the client's device to the servers.
## CI/CD Pipeline Overview
- CI/CD pipelines help develop a feedback loop that enables faster deployment of changes to an app as well as making these deployments more reliable.
  ### Github Actions
- This could be used to run tests on the written code as well as build complete projects. Anything made or changed can then be saved to the cloud

