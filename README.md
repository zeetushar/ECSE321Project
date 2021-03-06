We would like to make our repository public. 

# ECSE321 Project Group 5

## Table of Contents
* [About](#about)
* [Technical Issues](#technical-issues)
* [Teamwork Report](#teamwork-report)
* [File Location](#file-location)
* [Front End Explanation](#front-end-explanation)



## About
The Co-operator is a co-op management tool integrating features from both myCourses and myFuture. Group 5 focuses on developing from the student viewpoint. Keeping this in mind, the fourth deliverable includes: 

1. User Documentation
2. Integrated System 
3. Build System 
4. Project Report

Tools that were used for this Deliverable include: Gradle, Heroku, Travis CI, Vue.js, HTML, CSS, Javascript

## Teamwork Report
### Deliverable 1

|Team member's name|Total hours|Responsibility          |
|------------------|-----------|----------------------- |
|Salman            |   20 hours|Persistence layer and JUnit Testing |
|Tushar            |   19 hours|User Case Diagrams, UML Diagram |
|Archit            |   20 hours|UML Diagram, Heroku Deployment and JUnit testing         |
|Kathy             |   17 hours|User Case Diagrams, Documentation and Project Wiki        |
|Mert              |   18 hours|UML Diagram and Requirements Model                        |

### Deliverable 2

|Team member's name|Total hours|Responsibility          |
|------------------|-----------|----------------------- |
|Salman            |   32 hours|Model redesign, Persistence, REST API, Database Testing  |
|Tushar            |   16 hours|Documentation & Testing |
|Archit            |   40 hours|New UML, Persistence, JUnit Testing, REST, Travis CI |
|Kathy             |   17 hours|Documentation & Project Wiki  |
|Mert              |   17 hours|Documentation & Software Quality Assurance Report         |

### Deliverable 3

|Team member's name|Total hours|Responsibility          |
|------------------|-----------|----------------------- |
|Salman            |   20 hours|Integation of Frontend with Backend  |
|Tushar            |   38 hours|Frontend Implementation |
|Archit            |   25 hours|Integration of Frontend with Backend  |
|Kathy             |   17 hours|Documentation & Project Wiki  |
|Mert              |   17 hours|Architecture Model & Documentation         |

### Deliverable 4

|Team member's name|Total hours|Responsibility          |
|------------------|-----------|----------------------- |
|Salman            |  15 hours| Fixing backend issues       |
|Tushar            |  35 hours| Adding Secure authentication and enhancing UI experience  |
|Archit            |  25 hours| Travis FrontEnd and User Documentation Report       |
|Kathy             |  15 hours|Documentation & Project Wiki  |
|Mert              |  15 hours|Project Management & Documentation |  

## File Location 
- Link to our REST controller class are included in the Backend folder under file controller
- Link to our BackEnd Heroku: https://cryptic-coast-32220.herokuapp.com
- Link to our FrontEnd Heroku: https://frontend-take2-murmur.herokuapp.com/#/  
- Link to our deliverable 4 Project Report:https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki/Project-Report-Deliverable-4
- Link to our Test Report: https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki/Software-Quality-Assurance-Report
- Our latest build runs perfectly fine on Travis. Continuous Integration is successful too. The latest version of the app (with BackEnd REST added) is available on the link above. Refer to Wiki documentation to see how to access those REST methods. 
- Link to our Architecture Model: https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki/Architecture-Model
- Link to our User Documentation Report: https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki

## Front End Explanation
 - FrontEnd Heroku is deployed correctly now. Please visit https://frontend-take2-murmur.herokuapp.com/#/. We also ensured that if you create any new student (or do anything on the frontend), it gets stored in the database. For ex, create a new student. Go to Postman or Rest Client and create a GET request with http://cryptic-coast-32220.herokuapp.com/students . You will see that the student you have created shows up.
 - Please create a new student and coop before accessing initial/technical/evaluation report methods. 
 - Version one screenshots can be found at https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki/Frontend-Screenshots
 ## New in Front End Version 2!
 - Secure login for authorization added for returning students.
 - New Page added to menu for showing previously submitted document links and instructor ID. (Unique Feature)  
 - As a new student, you only need to put your McGill ID once.
 - As a new student, you don’t need to remember your COOPID through the dashboard.
 - As a returning student, you need to only enter COOPID once, and the system will remember the ID till you logout.
 - Fixed a bug where "Welcome Student" was not displayed when the frontend was deployed to heroku!
 - Enhanced UI, by adding calender and options on the "addcoop" page. Previously they were all text fields.
 - New Screenshots and Main User Documentation can be found at https://github.com/McGill-ECSE321-Winter2019/ecse321-group-project-05-1/wiki/User-Documentation
