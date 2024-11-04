
Lab 8:
Update lab 8 markdown



Lab 7:
dirty data is data that violates some constraint and is not well formatted
^ one we address with openrefine one we address with the database

download openrefine over windows machine


quantitative = statistical methods for cleaning
syntactic = regular expressions and such
semantics = schema/constraints/pointers/foreign keys/vocabulary not agreeing


Lab 6:

make sure numbers in the slides and on github match

Be very detailed
Describe what each line is doing
Better explain what each command is doing in SQL

Emphasize how closely related lab 6 is to the exam. I encourage asking questions and going to office hours

what is ddl, sql files?

how to use command to load ddl to .db file

Reemphasize the SELECT

SELECT from something filter and groupby

make sure you put the sqlite3 exe in the correct directory

Take these two schemas and create a relevant new schema that combines information from 
both of them

<img src="Screenshot 2024-10-03 at 3.09.36 PM.png" width = "500">
![[Screenshot 2024-10-03 at 3.09.36 PM.png]]

![[Screenshot 2024-10-03 at 3.09.11 PM.png]]

```
SELECT 'A1' as Airline, s.FlightNum, s.DepartureAirport,
        f.DepartureDate, s.DepartureTime, f.DepartureTime,
       s.ArrivalAirport, f.ArrivalDate, s.ArrivalTime, 
       f.ArrivalTime
FROM Airline1_Schedule as s, Airline1_Flight as f
WHERE s.FlightId = f.FlightId ;
```

USE SLACK

TA OH: https://illinois.zoom.us/s/83408069971

Management Drive: https://drive.google.com/drive/folders/1jkDnQz9u5tq6rXeyYyQQ9FwvSlzX5aDq

Slides: https://drive.google.com/drive/folders/15adR8wMVgdUtMhWVtyOXI2Kx8SoffCIX

Canvas Links:
(old) https://canvas.illinois.edu/courses/42022
(current) https://canvas.illinois.edu/courses/47996
	(syllabus) https://canvas.illinois.edu/courses/42022/assignments/syllabus


To-Do:
- [ ] Add office hours (1 hour)
- [ ] Add personal to the intro slides
- [ ] Watch Thursday lab lecture and today lecture

Questions
- What is the classroom (1302 Everitt Lab)
- Added to the Github repo

Course Outline (477 - Data Management, Curation & Reproducibility):
1. Course Intro 
	1. Lab: Made changes regarding sp to fa
2. Ethics, Laws, and Governances
3. Collection and Acquisition
4. Storage and Organization
5. Data and Information Modeling
6. Data Integration
7. Data Quality and Cleaning
8. Reproducibility, Replicability, and Transparency
9. Workflow Automation
10. Provenance
11. Metadata and Discovery
12. Preservation and Archiving
13. Communication and Workforce


**Assignments and Methods of Assessment**
	Homework assignments **24%**
	Quizzes **14%**
	Labs and exercises **14%**
	Midterm exam **20%**
	Final project **20%**
	Participation and instructor assessment **8%**



Cynthia Choi.