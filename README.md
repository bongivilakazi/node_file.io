# node_file.io


Search...
Umuzi Remote work
1. Syllabus
2. Topics
3. Workshops
4. Projects
Android with Kotlin Projects
Constraint Layout Using Layout Editor
Data Binding Basics
Linear layout using the Layout Editor
User Activity
Androids
Incremental Counter
Information Page
Angular Tutorial
Assertive programming kata
Bootcamp Writing Assignment
Build your first personal website
Capstone project
Gmail Text Scraper
Pair Stairs
Spaced Repitition machine to help you remember what you read
The Quizmaster
build a Chrome Extension that measures time spent in meetings
Consume Github API
DAGs with Airflow
Data-science-specifics
MEDIUM: Cross-validation & Simple Linear Regression
Dashboard Assignment
EASY: Google Data Studio Assignment
HARD: Live Dashboard Assignment
EASY: Plotly Dashboard Assignment
HARD: Webscraping and Live Dashboard Assignment
Data Modelling Challenges
HARD: Network Intrusion
Data Visualisation Projects
MEDIUM: Evolution of Linux Visualisation
MEDIUM: Financial Services Use in Tanzania
MEDIUM: Data Wrangling
MEDIUM: Decision Trees
Introduction to Jupyter Notebooks
MEDIUM: K-Means Clustering Assignment
Logistic regression
MEDIUM: Predict breast cancer
MEDIUM: Predict credit card approvals
MEDIUM: Multivariate Linear Regression
MEDIUM: Natural language processing
MEDIUM: OOP for data science
MEDIUM: Statistical Thinking
Webscraping Assignment
Distributed workloads with ZeroMQ
Email random inspirational quote
Expose a simple REST api for your game
ExpressJS
Game of life: Angular elements
Git Basic Exercises
How to submit your project
Java Projects
Consume own api using curl
File IO + Logging + Errors
Introduction to Spring Boot
Introduction to Spring Boot - part 1
Introduction to Spring Boot - part 2
Introduction to Spring Boot - part 3
Introduction to Spring Boot - part 4
Introduction to Spring Infrastructure
Introduction to Spring Infrastructure part 1
Introduction to Spring Infrastructure part 2
Introduction to Spring Infrastructure part 3
Java Generics
Java collections
Java data structures
SQL Extended
Level 1 programming katas
Linux challenges
Advanced Linux challenges
Beginner Linux challenges
Memory Game: rebuild using a modern web frontend framework
Memory game in vanilla js
Memory game using Angular Material
Nodejs Challenges
1: Node & File IO
2 (alt): Node & mongoDB assignment
3: Express, forms and templates
4: Expose a JSON API
Add a little Ajax
Node & SQL assignment
OOP Excercises
Animals
Animals Part 1. OOP basics
Animals Part 2. Adding Tests
Bank Accounts
Dice
Person
Pre bootcamp challenges
Python projects
Database migrations with SQLAlchemy
Django - exposing a REST api with a real database
Getting to know Python
Python and Kafka
Python and MongoDB
Python and Spark
create a REST api to interact with actual database
expose a simple JSON rest api
RabbitMQ
SQL
Semitone Challenge
1. semitone difference - basic algorithm
1. Make a simple GUI
3. Advanced algorithm
4. A gui that is more...awesome
Add Redux to your semitone game
Test Driven Development
Password Checker
Add logging to password checker
password-checker
MEDIUM: Resturaunt menu system
EASY: factorials
MEDIUM: lots and lots of tdd katas
MEDIUM: recursive search
EASY: simple-calculator part 1
MEDIUM: simple-calculator part 2
string-calculator
HARD: ten-pin bowling scoring system
Validating user input for web
consuming APIs with the requests module
iOS Mobile
Codable, File Manager, URL
Drag and Drop, Multithreading and Delegation
More Swift, Gestures and Animations
Multithreading Layout and Other Functionality - Animated Set
Multithreading Layout and Other Functionality - Graphical Set
Swift and More
5. Katas
6. Department Processes
Code Review Feedback Notes
Contact
Credits
How to Contribute
Online Learning and bootcamp
More
 Github repo
 Credits
  
 Edit this page Umuzi Tech Department > Projects > Nodejs Challenges > Node & File IO
NODE & FILE IO
Story points	3
Tags	Node FileIO
Hard Prerequisites	
TOPICS: Node
To submit this project follow the link below: TILDE
You are required to create a back-end service that will help capture basic information about prospective students who come to inquire here at Umuzi. In this project you’ll just be storing and retrieving information from plain old json files.

Instructions
Create the following functionality in a TDD way.

Create a class called Visitor. Instances of this class should have the following properties:
full name
age
date of visit
time of visit
comments
name of the person who assisted the visitor
Create a function called save that saves the visitor’s data to a JSON file. The file name should be named like this visitor_{their_full_name}.json.
alice.save()   # results in visitor_alice_cooper.json
bob.save()     # results in visitor_bob_marley.json
charlie.save() # results in visitor_charley_sheen.json
Notice that the full name used in the file is all lower-case and spaces are replaced by underscores.

Create a function called load that takes in a name and then grabs a Visitor object from file. It should simply console.log the visitor.
eg:

load("Alice Cooper")
// prints out all of Alice's goodies


load("Bob Marley")
// Same deal for good ol Bob
Resources
Accessing the file system
JSON: Make sure you understand everything up to the end of “JSON Arrays”
Up for a challenge?
Here are some upgrades you can add to your project if you are up for it.

Update your load function so that it returns an instance of Visitor instead of just console.logging it. You’ll need to learn a little bit about Syncronous versus Asyncronous code to get this one right :)

Make use of integer ids when saving things to files.

Update your save function so it works like this:

alice.save()   # results in visitor_1.json
bob.save()     # results in visitor_2.json
charlie.save() # results in visitor_3.json

alice.comments = "Kinda weird, I don't think he'll fit in"
alice.save()   # results in an UPDATE to visitor_1.json
Your load function should also get a bit of an update.

charlie = load(3)
charlie.comments = "Winning!"
charlie.save() # results in an UPDATE to visitor_3.json
RAW CONTENT URL
