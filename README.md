# Database Systems (CS305) Lab 4 Assignment 

Designing your own database schema

**Assigned** : Thursday 28 September 2023

**Due** : Thursday 12 October 2023

![logo](graphics/drawnplans.png)

## Project Goals
The main goals of this work include the following.

* To design databases after evaluating the different levels of schema. 
* To determine the natural relationships in the data to be used to build connections between tables.
* To evaluate some of the ethical considerations involved with database design.

## Resources

## Introduction

The design of a database is very important to its intended functionality. In addition to the relationships that must exist between each table, there are other considerations, as well, which must be made to ensure better functionality. In addition, during the design of a database, an architect may include thinking to facilitate the maintenance of the database. Discussed below are the different levels of a schema which encourage thinking about functionality and maintenance.

## Schema

When designing a schema, there are different levels in its design. In Figure 1, we note these levels in a schematic drawing of a typical database.

* **A View Schema or External Schema**
  + A View Schema defines the design of the database by what it will look like when deployed. At this level, the designer can decide how the user is to understand this database as a tool. This design also dictates how the database will be presented to the user by a command-line driven application, by a browser and etc. This level also determines the level of necessary training or skill in terms of programming that would be necessary to interact with the system.

* **The Logical Schema or Conceptual Schema**
  + The Logical Schema, shown in Figures 1 and 2 defines the design of the database at the conceptual level of the data abstraction. Here, we note the the definitions for tables, attributes, entities, constraints, relationships and similar which serve to connect each table to the others. In addition, we also note here that each entity in any of the tables has been carefully placed according to a logical relationship.

* **The Physical Schema**

  + This is the hardware level of the schema that describes how the data will be managed using computer equipment at the physical level of data abstraction. At this level, one notes how the data will be physically stored on the storage device(s) such as cloud technologies, local-hard drives, and similar. The kind of computer system (in terms of memory, CPU power and similar) would also be clear from an evaluation at this level.

## What To Do

Locate and obtain a source of data from an online source of data. A list of sites that may offer data for this project is given below. Please note; keep your database to around up to 1 Megabyte in size. If there is additional data from the site, then you are asked to cut the data down to size in a way of your choosing (taking a subset of the data according to some rational or by cutting the data off at a particular size).

Once you have chosen your data, you must decide on the purpose of a database to use with this obtained data. Create the schema by implementing SQL code to create tables. After this step, populate the tables using `.separator` and `.import` statements which bring the data from the CSV files that you place in `src/data/`.


 In your `writing/reflection.md` Markdown file, you will be asked to reflect over the different levels of the schema design as you develop your system. Build your SQL database using at least three tables and return to the reflection Markdown file to explain your choices.

## Data Sets

To build your schema, please select a data set which is available for on line for free. You are welcome to find your data using the resources which are available on instructor's website [https://www.oliverbonhamcarter.com/resources/juniorseminar_resources/](https://www.oliverbonhamcarter.com/resources/juniorseminar_resources/).

Please use a new dataset which you have not used for any other project. Anticipate having between 1 MegaByte to 3 Megabytes of data in your database.

## Tables

Your database is to be composed of four or more tables having at least four columns of observations. The tables are to hold all the data

## The Build File

You will be preparing a build file to be used to create your database from file imports. This file contains all code that you otherwise would have had to type in manually to create the database and allows you to conveniently rebuild your database for any reason. Please edit the file `src/DB_build.txt` of your repository - you are to edit the table creation code and data population SQL code of the build file to create your database.

## Queries

Showcase your database by providing seven questions and their query-solutions. For each queries, please connect at least two tables. Please add your questions and their corresponding queries and output to the file, `writing/queries.md`.

---

## Deliverables

Summary of the Required Deliverables
Please submit your work by pushing it to your GitHub Classroom repository.

1. **Reflection document**: You will modify the file `writing/reflection.md` to respond questions in the document.

2. **Database-building file**: You will submit your edited build file (`src/DB_build.txt`) to be used to build your database from your obtained data files.

3. **Data files**: Please submit all your data files in `src/data/` and your compiled database as src/myDB.sqlite3.

4. **Query file**: You will submit your questions that you put to the data along with their associated queries in the file, `writing/queries.md`.

Note: If you would like to add screenshots to your work, please use the the following code;

```
![graphic](graphic.png)
```

The following html code serves to scale-down your graphic.

```
<img src="graphic.png" alt="drawing" width="200"/>
```

## Technical Information

### Git

Practicing software developers normally use a version control system to manage most of the artifacts produced during the phases of the software development life cycle.

In this course, we will always use the `git` distributed version control system to manage the files associated with our course. In particular, we will use this secure resource to submit our all our assignments and projects.

To help you get started with installing course software, our course [resources page](https://www.oliverbonhamcarter.com/resources/), contains URL links to download sites and important tutorials.

Note, if you are using a Mac or Linux machine, you may already have this software installed; try typing `git` at your terminal to check. On a MacOS machine, this command will ask you whether you wish to install `xCode`. Please follow the steps to install.

 If you are using a Windows machine then it is likely that you will need to install the software. Ask a Technical Leader or your instructor for help as necessary.

### Create your account on GitHub

It is assumed that you already have an account on GitHub but if you do not, then please visit [github.com](http://www.github.com) to create your account using your Allegheny email address. Follow the account generation links to create an account on GitHub using a normal name (to identify you) and be sure to add a current photo of yourself when completing your profile.

### Add Your SSH Keys to your account

SSH keys allow you to interact with GitHub using secure means. Using these keys, you can conveniently push and pull data from GitHub without having to input your user name and password each time. When developing code, it will be desirable to make frequent pushes to GitHub with your code so that any problems or bugs, can be isolated with the development of specific parts of code.

To learn more about creating and adding your ssh keys to your GitHub account. Please visit https://www.ssh.com/ssh/keygen/ to learn how to set-up your security keys. Let the instructor know if you have any questions with this task. For more information about ssh keys, please watch Professor Luman’s SSH Key [video](https://www.youtube.com/watch?v=qEPjUGQFmzQ&list=PLsYZRXov75ZHSwWiCk0-jd1RcTuu_-zmD).

### Submitting Assignments
As you are working on your lab, you are to commit and push regularly. The commands are the following.

```
git add -A
git commit -m ‘‘Your notes about commit here’’ 
git push
```

## Project Assessment

The grade that a student receives on this assignment will have the following components.

- **GitHub Actions CI Build Status [up to 50%]:**: For the lab repository associated with this assignment students will receive a checkmark grade if their last before-the-deadline build passes. This is only checking some baseline writing and commit requirements as well as correct running of the program. An additional reduction will given if the commit log shows a cluster of commits at the end clearly used just to pass this requirement. An addition reduction will also be given if there is no commit during lab work times. All other requirements are evaluated manually.

- **Mastery of Technical Writing [up to 50%]:**: Students will also receive a checkmark grade when the responses to the writing questions presented in the deliverable Files of the directory `writing/` that reveal a proficiency of both writing skills and technical knowledge. To receive a checkmark grade, the submitted writing should have correct spelling, grammar, and punctuation in addition to following the rules of Markdown and providing conceptually and technically accurate answers.

## GatorGrade

### Checks for GatorGrade

For immediate feedback on submissions, we will be using Gator Grade to inform the of missing components in the submission. As you submit, you will notice that there is a thick red X that will change to a green check mark when all components have been included in the submission. You are encouraged to click on the red X to find a listing of the components to address.

You can check the baseline writing and commit requirements for this lab assignment by running department's assignment checking `gatorgrade` tool. To use `gatorgrade`, you first need to make sure you have Python3 installed (type `python --version` to check). If you do not have Python installed, please see:

- [Setting Up Python on Windows](https://realpython.com/lessons/python-windows-setup/)
- [Python 3 Installation and Setup Guide](https://realpython.com/installing-python/)
- [How to Install Python 3 and Set Up a Local Programming Environment on Windows 10](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-windows-10)

Then, if you have not done so already, you need to install `gatorgrade`:

- First, [install `pipx`](https://pypa.github.io/pipx/installation/)
- Then, install `gatorgrade` with `pipx install gatorgrade`

Finally, you can run `gatorgrade`:

`gatorgrade --config config/gatorgrade.yml`

## Seeking Assistance

* Extra resources for using markdown include;
  + [Markdown Tidbits](https://www.youtube.com/watch?v=cdJEUAy5IyA)
  + [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Do not forget to use the above git commands to push your work to the cloud for the instructor to grade your assignment. You can go to your GitHub repository using your browser to verify that your files have been submitted. Please see the TL’s or the instructor if you have any questions about assignment submission.

Students who have questions about this project outside of the lab time are invited
to ask them in the course's Discord channel or during instructor's or TL's office hours.
