
<!-- ABOUT THE PROJECT -->
## ToDo Web App - Liban Abdirahman

### Project Introduction

This is a DFE/QA cloud specialism final project. The objective for this project are the following:

* To create a web application that integrates with a database and demonstrates CRUD functionality.
* To utilise containers to host and deploy your application.
* To create a continuous integration (CI)/continuous deployment (CD) pipeline that will automatically test, build and deploy your application.

<!-- ABOUT THE PROJECT -->
## Contents

* Application

* Design

* Architecture

* Project Management

* CI/CD Pipeline

* Risk Assessment


## Application

For this project, I have developed a Flask web app that helps users plan their daily schedule. Users can add, view, update, and delete to-do items on their homepage. Users are also able to keep track of what they have and have not completed with a statusbar which turns green when completed and red when not completed.

<!-- ROADMAP -->
## Design
 


![Screenshot (4)](https://user-images.githubusercontent.com/111815447/198462484-36e6ea70-2c05-4258-8d52-f23ceb5b6eca.png)





![Screenshot (3)](https://user-images.githubusercontent.com/111815447/198452675-38c1c69d-517f-4f2c-844d-5a9899532ba2.png)





<!-- CONTRIBUTING -->
## Architecture

Below is my ERD, showing a one-to-many relationship:

![Screenshot (8)](https://user-images.githubusercontent.com/111815447/198511292-35098ea4-3380-4368-8b9a-af29ed603fc6.png)







<!-- LICENSE -->
## Project Management

As detailed below, I used Jira to manage and track this project:

![Screenshot (9)](https://user-images.githubusercontent.com/111815447/198513738-88a3710b-6a67-4d3d-8127-4592c8864d48.png)

![Screenshot (14)](https://user-images.githubusercontent.com/111815447/198514312-077f87bd-a656-4587-bf0a-2b16032be048.png)

MoSCoW prioritisation below:

![Screenshot (15)](https://user-images.githubusercontent.com/111815447/198514395-1271a50e-f376-4d62-a906-ca4b0e4dbd83.png)






<!-- CONTACT -->
## CI/CD Pipeline

As stated in the Project brief, I created a CI/CD pipeline using Jenkins. To achieve this, I first set up an Azure Virtual machine running Linux ubuntu 20.04. I then installed Jenkins and Docker on it. I then pushed my project from Visual studio code on my local computer to a GitHub respiratory, which I named (ToDo-Webapp). I then set up a Jenkins pipeline by creating a Jenkins file in my GitHub respiratory (ToDo-Webapp) and copying my Respiratory URL into the pipeline job in Jenkins so that I could clone, copy, and set up files and folders from my GitHub respiratory to the Azure virtual machine so that the Docker container could then be built and run.

![Screenshot (25)](https://user-images.githubusercontent.com/111815447/198723120-fa1b7169-b2c3-4704-9fdb-0d3c3d612938.png)

![Screenshot (22)](https://user-images.githubusercontent.com/111815447/198722990-e00ffd5a-1847-4c91-a73e-6b02f0e656ac.png)

![Screenshot (21)](https://user-images.githubusercontent.com/111815447/198717557-27374c62-6882-4fb4-a54d-ec0c0fc29044.png)





<!-- LICENSE -->
## Risk Assessment

My risk assessment is detailed below:

![Screenshot (16)](https://user-images.githubusercontent.com/111815447/198510528-6417d998-e244-43c0-a096-eb640279523b.png)


