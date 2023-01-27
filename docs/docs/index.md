# Project Requirements

## Executive Summary

A short overview of the project (one paragraph), including the following: the problem that the product will solve (use your client’s language); value proposition (what will be the essential functionality or your product); who will use your product; how your product will be used.

## Project Glossary
- **Lesson** - A lesson consists of some text, and an audio recording of the pronunciation.

- **Chapter** - A chapter consists of a lessons on a similar subject, with an accompanying label to describe the lessons.

- **Lesson Tab** - A lesson tab consists of lessons and/or chapters. Lesson tabs aggregate larger concepts and or languages.

- **Student Account** - An account representing a student, may view and do lessons. Can be associated with teacher accounts. Can have lessons assigned to them by a teacher.

- **Teacher Account** - An account representing a teacher. Can be associated with student accounts. Can assign lessons to students, and monitor their process..

- **Parent Account** - An account representing the parent or guardian of a student. May be associated with one or more student accounts. Can view the progress of an associated student..

- **Content Creator Account** - An account that is responsible for adding content to the system. May also be a teacher account. Can upload files to create and organize lessons, lesson groups, and lesson collections.

- **Assignment** - A set of lessons assigned to a student account by a teacher account. Tracks the assignees progress.

- **Lesson Status** - The status of a lesson. It can be one of:
    - ***Non-assigned***: Default status indicates a lesson that has not been assigned.
    - ***Assigned***: The lesson has been assigned to the student by a teacher. Lesson is ready to be done.
    - ***Complete***: The Lesson has been assigned and completed by the assigned student. The details of completing are determined by the teacher at the time of assignment.
    - ***Confirmed***: Lesson has been completed by the student, and the assigning teacher has confirmed the students progress. Lesson no longer needs to be completed.
    - ***Marked for redo***: Lesson has been completed by the student, and the assigning teacher has decided the student needs to do the assignment again. The assignment will need to be completed by the student again, and the teacher will need to reassess the students progress.


## User Stories
### US 1 - Admin
##### US 1.01 - Add Users
> As an admin, I would like to add users to my service, so that they can use my service.

> **Acceptance Tests**

> 1. Admin can add users
> 2. New user can log in to their account
> 3. New user has the correct information displayed on their account

##### US 1.02 - Assign Roles to Users
> As an admin, I would like to assign a user one or more roles from “students”, “parents”, “teachers”, “content creators”, so that they can only use the service according to their assigned roles.

> **Acceptance Tests**

> 1. Admin can assign one or more roles to user
> 2. User roles stored in database

##### US 1.03 - Different Layouts 
> As an admin, I want some users to be shown a different layout of my service according to their role, so that users only view information relevant to them.

> **Acceptance Tests**

> 1. When user logs in, they can only see the layout(s) corresponding to their role(s)
> 2. Test with 4 users each having a different role (student, parent, teacher, content creator); make sure each role sees the correct layout
> 3. Test with users having a combination of roles; make sure they can use the all features associated with their assigned roles

##### US 1.04 - Add Admin
> As an admin, I would like to add another admin to my service, so that they can manage my service.

> **Acceptance Tests**

> 1. Admin 1 can add another admin account, Admin 2
> 2. Admin 2 can log in to the admin panel
> 3. Admin 2 has all the privileges of Admin 1

##### US 1.05 - Remove Users
> As an admin, I would like to remove users from my database, so that they can no longer use my service.

> **Acceptance Tests**

> 1. Admin can delete users
> 2. Deleted user can not log in to their account

##### US 1.06 - Manage User Accounts
> As an admin, I would like to manage each user’s account, so that I can update their information if needed.

> **Acceptance Tests**

> 1. Admin can select a user’s account to manage
> 2. Admin can update information of user’s account
> 3. Updated information displayed when user logs in to their account

##### US 1.07 - Change User Roles
> As an admin, I would like to change the assigned roles of users of my service, so that they can use my service according to different roles.

> **Acceptance Tests**

> 1. Admin can change the roles of existing users
> 2. New roles are updated in the database
> 3. User can see the layout(s) associated with the different role(s) assigned to them

##### US 1.08 - Filter Users by Role
> As an admin, I would like to filter out users of my service according to their assigned roles, so that I can manage groups of users at once.

> **Acceptance Tests**

> 1. Admin can filter users according to one or more roles
> 2. All users with the selected role(s) are returned
> 3. No users with different roles are returned

##### US 1.09 - Link Students to Parents
> As an admin, I would like to link student accounts to parent accounts, so that I know who a student’s parents are.

> **Acceptance Tests**

> 1. Admin can link parent accounts to student accounts
> 2. Parents of student are displayed when managing student accounts

##### US 1.10 - Link Parents to Students
> As an admin, I would like to link parent sccounts to student accounts, so that I know who a parent’s children (students in the database) are.

> **Acceptance Tests**

> 1. Admin can link student accounts to parent accounts
> 2. Parents can have multiple student accounts linked to their account
> 3. Parent’s children are displayed when managing parent accounts

##### US 1.11 - View Tasks
> As an admin, I want to be able to remove lessons from the system, I case there are issues with the lessons.

> **Acceptance Tests**

> 1. Lesson data is no longer stored in the system
> 2. Lesson is no longer displayed to any user

### US 2 - Content Creator
##### US 2.01 - Create Lesson Tabs
> As a content creator, I would like to create new lesson tabs, so that I can add lessons to them.

> **Acceptance Tests**

> 1. Content creator can create new lesson tabs
> 2. New lesson tabs are displayed when content creators or teachers log in to their account

##### US 2.02 - Naming/Renaming Lesson Tabs
> As a content creator, I would like to be able to name and rename lesson tabs, so that they can be differentiated.

> **Acceptance Tests**

> 1. Lesson tabs can be named
> 2. Lesson tabs can be renamed
> 3. Make sure new/updated names of lesson tabs are displayed correctly when a user (that can see the lesson tab) logs in to their account

##### US 2.03 - Upload Lessons
> As a content creator, I would like to upload one or more lessons to each lesson tab, so that lessons can be assigned by teachers.

> **Acceptance Tests**

> 1. Content creator can upload one lesson to a lesson tab
> 2. Content creator can upload multiple lessons to a lesson tab at once
> 3. All lessons that content creator has uploaded are displayed under the corresponding lesson tab
> 4. All lessons that content creator has uploaded are displayed correctly
> 5. Teachers can see newly uploaded lessons
> 6. Teachers can assign newly uploaded lessons to students

##### US 2.04 - Group Lessons into Chapters
> As a content creator, I would like to group lessons in each lesson tab into chapters, so that similar lessons are displayed together.

> **Acceptance Tests**

> 1. Content creator can select one or more lesson and join them into a chapter
> 2. Content creator can add lessons to the chapter
> 3. Content creator can remove lessons from a chapter
> 4. Chapters and their lessons are displayed correctly when a user (that can see the lesson tab) logs in to their account

##### US 2.05 - Naming/Renaming Chapters
> As a content creator, I would like to name and rename chapters in a lesson tab, so that I can differentiate different chapters within a lesson tab.

> **Acceptance Tests**

> 1. Content creator can name new chapters
> 2. Content creator can rename existing chapters
> 3. New/updated chapter names are correctly displayed when a user (that can see the lesson tab) logs in to their account

##### US 2.06 - Textual and Audible Components in Lessons
> As a content creator, I would like each lesson to have both a textual and an audible component.

> **Acceptance Tests**

> 1. Content creator can upload 2 files for each lesson, one representing the textual part and one representing the audible part
> 2. Textual component displayed correctly
> 3. Audible component plays the correct audio file
> 4. Textual and audible components correspond to the same lesson
> 5. Content creator can only upload 2 files per lesson, one of them being an audio file

##### US 2.07 - Textual Component Format
> As a content creator, I would like the textual aspect of each lesson to be represented by either an image or a plain text file, so that I can upload a lesson in multiple formats.

> **Acceptance Tests**

> 1. Content creator can select .txt files (along with audio files) when uploading new lessons
> 2. Content creator can select image (.jpg, .png) files when u uploading new lessons
> 3. Content creator can select only 1 file of either tab when uploading a lesson
> 4. Image is displayed correctly if textual part of lesson is an image
> 5. Text is displayed correctly if textual part of lesson is a plain text file

##### US 2.08 - Reorder Chapters
> As a content creator, I would like to reorder chapters within a lesson tab, so that I can make the chapters chronologically coherent.

> **Acceptance Tests**

> 1. Content creator can change the order of chapters in a lesson tab
> 2. New order of chapters is preserved when a user (that can see the lesson tab) logs in to their account

##### US 2.09 - Reorder Lessons
> As a content creator, I would like to reorder lessons within a chapter, so that I can make the lessons chronologically coherent.

> **Acceptance Tests**

> 1. Content creator can change the order of lessons in a chapter
> 2. New order of lessons is preserved when a user (that can see the chapter) logs in to their account

##### US 2.10 - Upload Arabic Lessons
> As a content creator, I would like to upload lessons in Arabic, so that I can create Arabic lessons.

> **Acceptance Tests**

> 1. Content creator can upload lessons with Arabic text
> 2. Arabic text is displayed correctly and appropriately (in the correct position)

### US 3 - Student
##### US 3.01 - View Lesson Tabs
> As a student, I want to be able to view lesson tabs that have assigned lessons for me, so that I can access my lessons.

> **Acceptance Tests**

> 1. Can see lesson tabs
> 2. Can only see lesson tabs that have lessons assigned to me

##### US 3.02 - Students Get Assigned Lessons
> As a student, I want to be able to have lessons assigned to me, so that I can know what to complete.

> **Acceptance Tests**

> 1. Student can have a number of lessons assigned to them in a lesson tab
> 2. Visual indicator of being assigned
> 3. Non assigned lessons are not indicated

##### US 3.03 - See Lesson Text
> As a student, I want to be able to see the text associated with a lesson, so I can know what I am learning to pronounce.

> **Acceptance Tests**

> 1. Lesson has text displayed
> 2. Text is displayed correctly, in english and arabic

##### US 3.04 - Lesson Audio Available
> As a student, I want to be able to listen to the pronunciation of some lesson text, so I can learn how to pronounce it correctly.

> **Acceptance Tests**

> 1. Lesson has associated audio included
> 2. Audio plays when selected
> 3. Audio is correct for the given lesson
> 4. Audio is audible and at reasonable volume

##### US 3.05 - Pause Lesson Audio
> As a student, I want to be able to have my lesson pause, so I can learn practice my pronunciation.

> **Acceptance Tests**

> 1. Lesson audio pauses after being played
> 2. Audio pauses for at least as long as the audio played for
> 3. Audio resumes after pause

##### US 3.06 - Repeat Lesson Audio
> As a student, I want to be able to have my lesson repeat for the given duration or number of times, so I can be able to practice.

> **Acceptance Tests**

> 1. Lesson audio repeats for at least the given duration, including pauses
> 2. Lesson audio repeats for the given amount of times
> 3. Lesson audio does not overlap itself
> 4. Lesson audio pauses to allow practice, following audio pausing story guidelines

##### US 3.07 - See Lesson Status
> As a student, I want to be able to see the status of my lessons, so I can view my progress.

> **Acceptance Tests**

> 1. Lessons are marked assigned after being assigned
> 2. Lessons are marked completed after being finished by student
> 3. Lessons are only marked completed after finishing an assignment including them
> 4. Lessons are marked as confirmed after a teacher condoms the progress
> 5. Lessons are marked for redo if a teacher marks them

##### US 3.08 - Redo Assignments
> As a student, I want to be able to redo assignments, so that I can properly practice.

> **Acceptance Tests**

> 1. Lessons marked for being redone may be reattempted
> 2. Redone lessons conform to previous lesson story requirements
> 3. Redone lessons will be marked completed upon completion

##### US 3.09 - See Chapters
> As a student, I want to be able to see how assignments are sorted into chapters within a lesson tab, so I know what I am practicing.

> **Acceptance Tests**

> 1. Lessons are visually divided into collections
> 2. Lessons collections have a header to indicate type and content of the collection

##### US 3.10 - Student Accounts
> As a student, I want to have an account associated with me, so that I can have my progress tracked and have assignments.

> **Acceptance Tests**

> 1. Student can have an account with their information
> 2. Progress is tracked based on account

##### US 3.11 - Log in to Account
> As a student, I want to be able to log into my account, so that I may access things associated with my account.

> **Acceptance Tests**

> 1. Interface to log into account
> 2. Correctly authenticates account information
> 3. Denies access with incorrect account information

### US 4 - Parent
##### US 4.01 - Associate Parents & Students
> As a parent, I want to be able to have children associated with me, so I can monitor their progress.

> **Acceptance Tests**

> 1. Parent account may have any number of associated children account
> 2. Parent account is only associated with there accounts

##### US 4.02 - Seee Children's Assigned Tabs
> As a parent, I want to be able to see what lesson tabs my children have assigned to them, so I can see what they are learning.

> **Acceptance Tests**

> 1. Lesson tabs are displayed correctly
> 2. Lesson tabs only display if an associated child account has been assigned content from them
> 3. Lesson tabs will display if any child account has been assigned to them


##### US 4.03 - See Children's Assigned Lessons
> As a parent, I want to be able to see what lessons my children have assigned to them (past and present), so i can monitor their progress.

> **Acceptance Tests**

> 1. Any lessons assigned to associated children accounts are displayed and noted
> 2. Lessons not assigned to an associated child account are not displayed
> 3. Visual indicator is given to indicate assignment

### US 5 - Teacher
##### US 5.01 - Associate Teachers with Students
> As a teacher, I want to have students associated with me, so that I can teach these students.

> **Acceptance Tests**

> 1. Only specifically assigned students are associated with the teacher

##### US 5.02 - Assigning Lessons to Students
> As a teacher, I want to assign lessons to students, so they can practice these lessons.

> **Acceptance Tests**

> 1. Individual lessons can be assigned
> 2. Groups of lessons can be assigned
> 3. Assignments can be per student or groups of students

##### US 5.03 - Add Repetitions Per Assigned Lesson
> As a teacher, I want to assign lessons to students based on duration or number of repetitions, so they will practice the lesson for the given duration.

> **Acceptance Tests**

> 1. Lessons repeat for the given duration
> 2. Lessons repeat for the given number of repetitions
> 3. Lessons are only marked complete after the duration elapses

##### US 5.04 - See Students' Progress
> As a teacher, I want to see my students progress on assigned lessons, so that I can monitor their learning progress.

> **Acceptance Tests**

> 1. Progress is displayed for each students assignments
> 2. Visually indicates the students progress (assigned, completed, confirmed, marked for redo)

##### US 5.05 - Mark Assignments for Redo
> As a teacher, I want to mark assignments for redoing, so that my students can get more practice on problem lessons.

> **Acceptance Tests**

> 1. Completed assignments can be set to be redone
> 2. Visual indication that lessons have been set for recompletion
> 3. Visual indication when a lesson has be re completed

##### US 5.06 - See Content
> As a teacher, I want to see all content, so I can know what material is out there.

> **Acceptance Tests**

> 1. All tabs are visible to the teacher
> 2. All content of lesson tabs are visible to the teacher

## MoSCoW
### Must Have
* US 2.03 - View Profile
* US 2.89 - Change Password 

### Should Have
* US 1.23 - Create Account

### Could Have
* US 3.21 - Delete Account

### Would Like But Won't Get
* US 9.23 - Rainbows and Unicorns

## Similar Products
* [Digikey](http://www.digikey.ca/products/en)
    - Search inventory management
    - &lt;functionalities, with comments on how they may be used for code or inspiration&gt;
* [LORIS](http://www.loris.ca/)
    - Neuroimaging data management
    - &lt;functionalities, with comments on how they may be used for code or inspiration&gt;

## Open-source Projects
* [eLabFTW](https://github.com/elabftw/elabftw)
    - Experiment notebook software
    - &lt;functionalities, with comments on how they may be used for code or inspiration&gt; 

## Techincal Resources
### Backend: Flask + PostgreSQL
  * [Flask Documentation](https://flask.palletsprojects.com/en/2.0.x/tutorial/index.html)
  * [Setting up Postgres, SQLAlchemy, and Alembic](https://realpython.com/flask-by-example-part-2-postgres-sqlalchemy-and-alembic/)
### Deployment: Docker + k8s + TravisCI
  * [Deploy on Kubernetes - Docker Documentation](https://docs.docker.com/desktop/kubernetes/)
  * [Travis CI Documentation](https://docs.travis-ci.com/)
  * [Setting up Travis CI on an existing Python/Docker project](https://www.youtube.com/watch?v=1PC68ufAn6U)
### Frontend: Vue.js + Buefy
  * [Vue.js v2 Guide](https://vuejs.org/v2/guide/)
  * [Buefy Documentation](https://buefy.org/documentation)
