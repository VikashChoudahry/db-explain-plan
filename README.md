# db-explain-plan
Contains the necessary sources to execute the explain plan

# Prerequisite
- Docker and Docker-compose must be installed into your system.

Installed version that I have used is:
```
$ docker --version                                                     
Docker version 20.10.21, build baeda1f

$ docker-compose --version
Docker Compose version v2.13.0
```

# Steps to use
1. Open any of your favorite terminal (I have used zsh)
2. Clone the repo https://github.com/VikashChoudahry/db-explain-plan.git
3. Navigate to the directory "db-explain-plan/mysql"
4. Run: `docker-compose up`

**Output:** MySQL database must be up and running.

# Connect to the Database
1. Open MySQL Workbench (have installed 8.0)
2. Click on MySQL connection(+ icon)
3. Used the following details to connect to the database:
  - Hostname: 127.0.0.1
  - Port: 3306
  - Username: root
  - Password: changeme (just for learning purpose. It has to be strong password if it's being used for any of the live project)

**Output:** You must be connected to the database with default schema(s).

# Import Database Schema
1. Ensure that you are on Workbench.
2. Click on "Administration" tab within Workbench.
3. Select Data Import/Restore option
4. Select "Import from Self-Contained" file
5. Select the schema file from "db-explain-plan/schema/classicmodels.sql"
6. Select "Dump Structure and Data" from the dropdown (you may see at the bottom).
7. Select "Start Import"

**Output:** You must be seeing "classicmodels" database created.

# How to open Entity-Relationship diagram

1. Open MySQL Workbench
2. Open classicmodels.mwb

**Output:** This will open ER diagram as a model in your MySQL workbench.

# Summary
Related to the EXPLAIN, most of the details are added as part of the "db-explain-plan/docuementation/MySQL - Query Optimization Understanding.pdf" document.

# Got stuck?

Don't worry! Please leave your query here - https://www.learnandshare.live/contact

Happy learning and sharing!