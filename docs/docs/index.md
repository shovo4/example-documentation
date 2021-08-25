# Project Requirements

## Executive Summary

A short overview of the project (one paragraph), including the following: the problem that the product will solve (use your client’s language); value proposition (what will be the essential functionality or your product); who will use your product; how your product will be used.

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

> 1. Login as user with correct information
> 2. Input incorrect information and make sure it doesn't allow the user to continue

### US 1.02 - View Tasks
> **As** a User, **I want** to be able to see events/surveys/quizzes that are currently going on for the week, **so that** I can attend theses events if I choose to.

> **Acceptance Tests**

> 1. User should be able to see all of the events in a list as well as all of the surveys and quizzes if they choose to.

### US 1.03 - View Profile
> **As** a User, **I want** to be able to view my profile, **so that** I can see my level, points, my history of attending events, surveys and quizzes.

> **Acceptance Tests**

> 1. Need to ensure the button in the drop-down menu will open. 
> 2. When the profile button is clicked, it will take me to my profile. 
> 3. User input is their specific user data.

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