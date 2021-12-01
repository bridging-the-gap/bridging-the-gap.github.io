## Bridging the Gap

* [Overview](#overview)
* [Deployment](#deployment)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Team](#team)

## Overview

The problem: Many UH computer science and engineering students want to learn about internship and job opportunities, but currently they must wait until a company decides to visit the campus or send out some sort of announcement. There is no efficient way for students to understand the “landscape” of internship and job opportunities that might be available in the future, so they can prepare for them now.

The solution: The Bridging the Gap web application provides a new way for local and non-local companies who want to recruit students from UH to make their (potential) opportunities known to students. At the same time, students can create profiles on the site with their interests. The site can match students to employers and vice-versa.

Here is a link to the [GitHub organization](https://github.com/bridging-the-gap) for this project and its repositories.

Our first project board, M1, can be found [here](https://github.com/bridging-the-gap/bridging-the-gap/projects/1).

Our second project board, M2, can be found [here](https://github.com/bridging-the-gap/bridging-the-gap/projects/2).

### Approach

Instead of sending out announcements each year, a company can create a page in the site that lists:

A brief overview of the company.
Geographic location of the company.
A list of positions that they commonly recruit for from new UH graduates. Each position has a brief description, a set of skills, whether it’s an internship, permanent position, or both, how many people they would like to hire, and salary range.
Links to pages for additional information.
Contact email(s) for followup.
Students who visit the site can create a profile with their interests (skills), preferred geographic location, and link to their professional portfolio page.

Admins can monitor the site for inappropriate content, and create new categories of musical tastes, capabilities, and goals.

Some mockup pages include:

* Landing page
* Student home page.
* Company home page
* Admin home page
* Student profile page.
* Company profile page
* Browse companies by by geographic preference etc.
* Browse students by skill etc.
* Events

## Deployment
The latest version of the app is hosted [here](https://bridging-the-gap.xyz/#/).

#### Log-in credentials for a home-page mockup for companies using the app: 
Email: google@google.com

Password: foo

#### Log-in credentials for a home-page mockup for students using the app: 
Email: henric@hawaii.edu

Password: foo

#### Log-in credentials for a home-page mockup for admin using the app: 
Email: cmoore@hawaii.edu

Password: foo

## User Guide

### Landing Page

The landing page is the page everyone sees when they first enter the site. It introduces Bridging the Gap and its purpose and describes how to register. There is also a place to leave feedback on the site.

<img src="doc/landing-page-M1.png">

### Sign in

Click on the “Login” button in the upper right corner of the navbar, then select “Sign in” to go to the following page and login. You must have been previously registered with the system to use this option:

<img src="doc/signin-page-M2.png">

### Sign up

Alternatively, you can select “Sign up” to go to the following page and register as a new user. In this case, you must specify your role as either student or company.

<img src="doc/signup-page-M2.png">

### Company Homepage

The company homepage allows companies to create their own profile on this site.
They are able to leave a short description of their company, where they are located, 
what industries they are interested in and an email by which they can be contacted.
From here, companies are also able to create job listings; the job title, 
the location of this job, it's salary range, the type of job (part-time, full-time, internship), 
how many opennings and a short description of the job's responsibilities.

<img src="doc/company account homepage.PNG">

### Company Profile Page

The company profile page will display all of the company's details and the jobs that are available for said company.
The company can also choose to add a background picture to customize their page.

<img src="doc/Company account profile.PNG">

### Browse Companies

The browse company page display all companies by geographic preference. Currently all logged in users can view this page.

<img src="doc/Browse-companies-M2.png">

### Student Homepage

This page will let the student have an overview over events and job applications.

<img src="doc/student-home-page.png">

### Student Profile Page

This page is for the student to add resume and job experience.

<img src="doc/student-profile-page.png">

### Browse Students

The browse students page display all students by skill preference. Currently all logged in users can view this page.

<img src="doc/Browse-students-M2.png">

### Admin Homepage

The admin homepage allows admins to make new categories, monitor innappropriate content, and chat with clients who may be having problems. Right now, the admin will receive reports made from clients regarding inappropriate content, as shown in the table. The admin can delete old and irrelevant reports as needed by clicking the "X" button. Based on reports, the admin can also delete the accounts of users who seem to be causing trouble. In addition, the admin can send individual messages to clients that will be sent to their email.

<img src="doc/admin-page-M2.png">

### Add Reports

The add reports page enables any user to add a report regarding inappropriate content on the site. As shown, this page is accessible in the dropdown in the top right of the navbar. Once a report is created and submitted, this information is sent straight to the admin for review.

<img src="doc/addReport-page-M2.png">

### Events

The event page will display all upcoming events arranged by companies for UH Students only. This involves career-fairs, presentations and dinners with potential employers. 

<img src="doc/event-mockup-page.png">

## Community Feedback

Not yet available.

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the [Bridging the Gap application github page](https://github.com/bowfolios/bowfolios), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.

Third, cd into the bridging-the-gap/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).

## Development History

The development process for Bridging the Gap conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:

* Development consists of a sequence of Milestones.
* Each Milestone is specified as a set of tasks.
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete.
* Tasks should typically consist of work that can be completed in 2-4 days.
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number.
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master.
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of Bridging the Gap.

### Milestone 1: Mockup development

The goal of Milestone 1 was to create a set of HTML pages using semantic ui react, which provide a mockup of the pages in the system.

Milestone 1 was managed using [Bridging the Gap GitHub Project Board M1](https://github.com/bridging-the-gap/bridging-the-gap/projects/1)

### Milestone 2: Data model development & testing

The goal of Milestone 2 was to implement the data model: the underlying set of Mongo Collections and the operations upon them that will support the Bridging the Gap application. In addition, we added more pages, improved on the overall functionality and completeness of the system, added testcafe acceptance tests, and put our system under continuous integration.

Milestone 2 was managed using [Bridging the Gap GitHub Project Board M2](https://github.com/bridging-the-gap/bridging-the-gap/projects/2)

### Milestone 3: Real data and finalizing functionality

The goal of Milestone 3 is to finish implementing the functionality of all our pages. In addition, we aim to add substantial amounts of real data to all of our collections in the system. Afterward, we will get community feedback and finalize testing on our site to ensure it is the best it can be.

Milestone 3 is managed using [Bridging the Gap GitHub Project Board M3](https://github.com/bridging-the-gap/bridging-the-gap/projects/3)

## Team

Bridging the Gap is designed, implemented, and maintained by 
* [Nina Nyegaarden](https://ninanye.github.io/) 
* [Helene Haugen](https://heleeha.github.io/) 
* [Marte Aaberge](https://martkaa.github.io/) 
* [Leilani Reich](https://leilani-reich.github.io/)
* [Bryan Yagi](https://bryanyagi.github.io/)


