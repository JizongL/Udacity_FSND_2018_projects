Logs Analysis
Jizong Liang

### About

A project from Udacity Full Stack Nanodegree. The task is to build a reporting tool that prints out reports (in plain text) based on the data in the database. This reporting tool is a Python program using the psycopg2 module to connect to the database.

The database includes newspaper articles and web server log for the site.

We do the following 3 queries to draw business conclusions from the data

* What are the most popular three articles of all time?

* Who are the most popular article authors of all time?

* On which days did more than 1% of requests lead to errors?


## How To Run?

You will need:

* Python3

* Vagrant

* VirtualBox

### Setup

Install Vagrant And VirtualBox

### To Run

Launch Vagrant VM and log in

```terminal
vagrant up
`vagrant ssh`
```

To load the data, use the following command.  

```terminal
psql -d news -f newsdata.sql
```


The newsdata database includes three tables:

* Authors table

* Articles table

* Log table

To execute the program, run  

```terminal
python3 log_analysis_2018.py
```
