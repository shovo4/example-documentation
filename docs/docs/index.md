# Project Requirements

## Executive Summary

The Pronunciaton Practice Hub is a website that allows young students to learn how to pronounce the verses of the Quran in Arabic. Students will have the ability to practice their pronunciation of verses assigned by their teacher through listening to an audio file, then repeating the verse back to themselves. The app is intended for K-8 students, but can be used by any age-group or demographic. Parents, teachers, and content creators will also have access to the site in order to view their child's progress, assign new work to students, and upload new learning modules for students respectively.

## Project Glossary
- **Attempt** An attempt is one data entry recorded from the procedure and assigned to an experiment.

- **Common Attribute** - A common attribute is a data column that all subjects have initially. It is pre-defined by the researcher’s data files that the robots create.

- **Custom Attribute** - A custom attribute is a user defined data column that does not already exist in the researcher's data files created by the robots.

- **Experiment** - An experiment is the collection of subjects and the attempts they have done for a scientific procedure. An example is “Spinal Damage Recovery Experiment (SDRE).”

- **Researcher** - A researcher manages the experiments and subjects. They can upload data, add custom attributes, query data, and export their results to an external CSV file.

- **Result** - A result is the returned attempts from a search query on some experiments. Results can be exported as an external CSV file.

- **Subject** - A subject is an animal used as part of an experiment. Each subject will have a unique ID.

## User Stories
### US 1.01 - Authentication
> **As** a User, **I want** to authenticate with my University of Alberta account, **so that** I can get access to the app's functionalities.

> **Acceptance Tests**

> 1. User can sign in with correct U of A credentials (ualberta.ca email and password)
> 2. User can not sign in with correct email and incorrect password
> 3. User can not sign in with incorrect email
> 4. User can not sign in with a non U of A email
> 5. User can not access app's functionalities without signing in

### US 1.02 - View Tasks
> **As** a User, **I want** to be able to see events that are currently going on for the week, **so that** I can attend theses events if I choose to.

> **Acceptance Tests**

> 1. User can see a list of all events for the chosen week
> 2. With the selected week, user can not see events that are scheduled for other weeks
> 3. User can see only active events (i.e., open for attendance)

### US 1.03 - View Profile
> **As** a User, **I want** to be able to view my profile, **so that** I can see my level, points, my history of attending events.

> **Acceptance Tests**

> 1. User can access their profile
> 2. User can see their level, number of points and history of attending events in their profile
> 3. Test with a zero and non-zero level
> 4. Test with a zero and non-zero number of points
> 5. Test with an empty, non-empty and very long (>50 items) event history

## MoSCoW
### Must Have
* US 1.03 - View Profile
* US 2.89 - Change Password 

### Should Have
* US 1.23 - Create Account

### Could Have
* US 3.21 - Delete Account

### Would Like But Won't Get
* US 9.23 - Rainbows and Unicorns

## Similar Products
* [Duolingo](https://www.duolingo.com/)
    - Online language-learning software
    - Language learning completed in the form of 'lessons' can be applied to current project
    - Capable of displaying Arabic script, so is a useful reference for displaying Arabic properly
    - Simple UI that is widely-accessible, so should take insipration on design since it will work well for young students
* [TarteeleQuran](https://www.tarteelequran.com/)
    - Online Quran education
    - No self-directed learning, students have lessons with teachers, helping us see what elements of the Arabic Quran can't easily be taught in a self-directed manner
    - Teaches Arabic outside of the Quran as well, providing insights into how we can expand the project in future to grow the user-base
* [ArabAcademy](https://www.arabacademy.com/)
    - Site for learning Arabic and not just the Quran
    - Provides Arabic lessons in a self-learning environment, similar to what this project intends to accomplish
    - Integrated teacher support that connects students with teachers, providing inspiration for expanding student-teacher interactions in this project

## Open-source Projects
* [Quran.com API](https://quran.api-docs.io/v4/getting-started/introduction)
    - Open-source API of Quranic verses
    - Allows us to query the API when we want to the text for specific verses
    - Provides audio files containing the pronunciation of each verse, allowing us to easily access all audio needed for the project
    - We can scrape the data from the API and add it to our own database, allowing us to add lessons outside the Quran without having to worry about unnecessary API calls
* [Tanzil Quran](https://tanzil.net/download/)
    - Open-source database of Quranic verses in Arabic
    - Allows us to download the complete text of the Quran in multiple styles and formats, allowing us to configure the data to fit our requirements
    - No audio files, so we would still have to incorporate the Quran.com API as well

## Techincal Resources
### Backend: Django + PostgreSQL
  * [Django Documentation](https://docs.djangoproject.com/en/4.1/)
  * [Setting up Postgres, SQLAlchemy, and Alembic](https://realpython.com/flask-by-example-part-2-postgres-sqlalchemy-and-alembic/)
### Deployment: Docker + CyberaRAC
  * [Using Docker with CyberaRAC](https://wiki.cybera.ca/display/RAC/Using+Docker+Machine)
  * [Docker Documentation](https://docs.docker.com/)
  * [Cybera Rapid Access Cloud Guide](https://wiki.cybera.ca/display/RAC/Rapid+Access+Cloud+Guide%3A+Part+1)
### Frontend: React.js
  * [React.js Documentation](https://reactjs.org/docs/getting-started.html)
