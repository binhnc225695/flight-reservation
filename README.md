An Airline E-Commerce website built using Java Spring Boot for the backend, MySQL as the database, AngularJS for frontend development, and Thymeleaf as the template engine.
Developed a clone of an Ecommerce Airline web application using Spring Boot, Spring Data JPA (Hibernate), and MySQL. The application includes features for flight search and booking.

Designed and implemented a REST API as an integration layer for the flight check-in microservice, enabling passengers to check in seamlessly. Additionally, created a dedicated microservice for the check-in process.

Implemented secure password encoding to prevent storage of plain text passwords and established role-based authentication and authorization to define different user roles.

Integrated logging features with custom log rotation policies to record and manage logs in an external log file efficiently.

Enhanced the application by incorporating AngularJS for form validation and two-way data binding.

Key Features
Built a web application that allows logged-in users to search and book flights.
Added a user registration feature with secure login implementation.
Utilized Spring Data JPA (Hibernate) for ORM to interact with the MySQL database.
Designed front-end templates with Thymeleaf and styled them using Bootstrap and CSS.
Employed Bower.js to manage dependencies like jQuery and Bootstrap.
Developed a REST API for flight check-in integration and implemented a separate microservice to handle passenger check-ins.
Microservice repository: Flight Check-In Microservice.
Database Design
The application includes six database tables:

FLIGHT
RESERVATION
USER
PASSENGER
USER_ROLE (for mapping users to roles)
ROLE (to define roles)
Relationships:

One-to-One:
Between RESERVATION and PASSENGER.
Between RESERVATION and FLIGHT.
Many-to-Many:
Between USER and ROLE via the USER_ROLE table, enabling assignment of multiple roles to a user and vice versa.
Role-Based Design
Roles are used to classify users into different categories, such as administrators and regular users.
The USER_ROLE table creates a flexible many-to-many relationship between users and roles, supporting complex authorization requirements.
