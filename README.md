# README #  

NAME: Alexander Owen  
URL: http://ix.cs.uoregon.edu/~aowen/htbin/cis399/proj2-flask/  
GITHUB URL: https://github.com/alexanderowen/proj2-flask  

CIS 399 Assignment 1 Winter 2016   

Small web page that displays the syllabus for CIS 399. Updated from source repo to display date 
and highlight the current week.

Main changes from the source repo are in  
-flask_syllabus.py  
-pre.py    

with minor changes to  
-syllabus.html  
-syllabus.css    

In order to display the date, the first day of each week is determined in pre.py. This information 
is passed over to flask_syllabus.py and stored in the flask session data. The first day of each week is 
then displayed using Jinja2 in syllabus.html.    

In order to highlight the current week, the first day of week 1 is passed from the pre.py function 'process()' 
to flask_syllabus.py. The helper function 'get\_week()' then determines which week the current day falls under.
This is passed over to the .html file and Jinja2 associates a html id with the appropriate tag.  


