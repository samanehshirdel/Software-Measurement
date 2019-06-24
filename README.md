# Software-Measurement(SOEN 6611) - summer 2019
The quality of a software is measured by different metrics. In this project, 6 different metrics are calculated from 5 different open source projects and correlation among these metrics is found. 
## Professor -Jinqiu Yang
## Team G 
| Name       | Student_ID           | Email_ID  |
| ------------- |:-------------:| -----:|
| Maria Ahmed    | 40070844  |ritu329@gmail.com |
| Mahy Salama    |  40074737      |   mahyhanysalama@gmail.com |
|Shehnaz Ansari  | 40070137     |   shehnaz1191@gmail.com |
|Samaneh Shirdel | 40075615      |   samaneh.shirdelk@gmail.com |
|Gagandeep Jaswal| 40066862      |   gagandeepjaswal227@gmail.com |
## Metrics calculated
1. Statement Coverage - covers only the true conditions. Through statement coverage we can identify the statements executed and where the code is not executed because of blockage. 
2. Branch Coverage - covers both the true and false conditions unlikely the statement coverage. Branch coverage is a testing method, which aims to ensure that each one of the possible branch from each decision point is executed at least once and thereby ensuring that all reachable code is executed. 
3. Mutation Score - is used to measure the quality of the test suites means for test suite effectiveness. A test suite having high mutation score detects more real faults than the test suite having low mutation score.
4. Cyclomatic Complexity - measures the number of linearly independent paths that can be executed through a piece of source code. 
5. Relative Code Churn - is a measure of the amount of the code changed within software over a period of time. Three different measures have been used to find relative code churn given beow:-
Measure1 = (Changing LOC + Removing LOC) / KLOC 
Measure2 = (Adding LOC + Changing LOC)/ KLOC 
Measure2 = (Adding LOC + Changing LOC+ Removing LOC)/ KLOC
6. Post-release Defect Density - Defect density is a measure of the total known defects divided by the size of the
software entity being measured.
Post-release defect density = number of known bugs reported in issue tracker for a version / KLOC of that version 
## Selected Open Surce Projects
1. Apache Commons Collections - _[Project Information](https://commons.apache.org/proper/commons-collections/)_
2. Apache Commnons Configuration- _[Project Information](https://commons.apache.org/proper/commons-configuration/)_
3. Apache Commons Math- _[Project Information](https://commons.apache.org/proper/commons-math/)_
4. Apache Commons Codec- _[Project Information](https://commons.apache.org/proper/commons-codec/)_
5. Apache Commons Text- _[Project Information](https://commons.apache.org/proper/commons-text/)_
## Tools Used
1. Jacoco 
2. PIT test 
3. CLOC

### Commands Used To Run the Tools for Collecting Data
1. Cloc - can be downloaded at this  _[link](https://commons.apache.org/proper/commons-collections/)_
* To find Lines of Code
** Cloc projectname>filename.csv -- To collect data in csv file
* To find relative code churn 
** cloc --diff project1 project2>filename.csv
2. Jira Query
* project = roject_name AND affectedVersion =version_number and issuetype =bug and  status in (Resolved, Closed) ORDER BY key DESC

