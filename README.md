# ECSE321 Project Group 5
*Co-operator deliverable 2*

## Table of Contents
* [About](#about)
* [Sprint Planning](#sprint-planning)
* [Technical Issues](#technical-issues)
* [Teamwork Report](#teamwork-report)
* [File Location](#file-location)


## About
The Co-operator is a co-op management tool intregrating features from both myCourses and myFuture. Group 5 mainly focuses on developing from the student viewpoint. Keeping this in mind, the second deliverable includes: 

1. Software Quality Assurance Report
2. Unit Testing of Backend 
3. Integration Testing 
4. Build System

Tools that were used for this Deliverable include: Eclipse, SpringBoot, Gradle, UML Lab, ZenHub, Heroku & Draw.Io

## Sprint Planning
For sprint 1, we decided to complete most parts of the deliverable together as a team, since none of us were extremely familiar with the technologies used.

*Met with TA after meeting 1 and meeting 2 for initial feedback and technical questions*

Meeting 1: (~90min)
- Project Discussion
- Detailed look at student viewpoint
- Understanding of functional and non-functional requirements
- First Draft of Requirments
- Noted down questions and confusing parts to ask the TA, customer and prof

Meeting 2: (~120min)
- Finalized requirements
- Draft of User Case Diagram
- Discussion of Domain Model and all team members were told to review Domain Modelling slides

Meeting 3: (~120min)
- Created Domain Model
- Team members split up work to focus on different parts of the deliverable (Domain Modelling and Persistence Layer)

Meeting 4: (~180min)
- Finalizing Domain model
- Begin coding persistence layer
- Begin documentation part of deliverable

Meeting 5: (~300min)
- Debugging issues in testing of the persistence layer 
- Finalize documentation
- Finalize all aspects of sprint 1 for submission

## Technical Issues
- Installation of UML Lab
- Deployment of our Spring Application to Heroku due to an additional folder that was created in github and not using the backend folder     already provided for this project. Since the settings.gradle file was pointing to backend folder and not the personalized folder, it       would push an error on terminal
- Issues generating Java code through UML; this was fixed by adding the correct packaging to the project

## Teamwork Report

|Team member's name|Total hours|Responsibility          |
|------------------|-----------|----------------------- |
|Salman            |   20 hours|Chief Technology Officier & Worked on persistence layer and Junit Testing
|Tushar            |   19 hours|User Case Diagrams, UML Diagram |
|Archit            |   20 hours|UML Diagram, Heroku Deployment and JUnit testing         |
|Kathy             |   17 hours|User Case Diagrams, Documentation and Project Wiki        |
|Mert              |   18 hours|UML Diagram and Requirements Model                        |

## File Location 
- All files related to Persistence layer is located in the Backend Folder
- All other files such as user case diagram, UML screenshot and requirements located in Deliverable 1
- Our Heroku link is https://cryptic-coast-32220.herokuapp.com/


