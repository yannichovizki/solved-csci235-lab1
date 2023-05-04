Download Link: https://assignmentchef.com/product/solved-csci235-lab1
<br>
This laboratory includes the tasks related to implementation of advanced SQL statements and PL/SQL Trigger.

More implementation related information can be found in “How to … ?” Cookbook available through Moodle or at:

Prologue

Download and unzip a file Lab1.zip. You should get the following files:

dbcreate.sql and dbdrop.sql.

Execute a script dbcreate.sql to create the relational tables of a sample database used in this laboratory. The sample database contains information about the applicant, skills, positions, applications, skills possessed by applicants, skills needed by the positions.

You can use a script dbdrop.sql to drop all relational tables created by dbcreate.sql later. Do not drop the relational tables now.

<h1>Tasks</h1>

<strong>Task 1 Triggers</strong>

<ul>

 <li>Implement and comprehensively test a <strong>statement trigger</strong> that verifies the following consistency constraint.</li>

</ul>

<em>“Maximum number of subjects offered in a session is 7”. </em>

<em>Hint: use the following SQL statement to test: </em>

<em>INSERT INTO RunningSubject VALUES (‘CSCI236’, ‘AUTUMN’, 2015, 150); </em>

<ul>

 <li>Implement and comprehensively test a <strong>row trigger</strong> that verifies the following consistency constraint.</li>

</ul>

<em>“When inserting a new staff record, the staff number must be continuous”. </em>

“Continuous” in staff number means, for example, that the first number must have a number 1, the second number must have a number 2, and each next number must have a

number greater by one than a number of the previous position.

When ready save your CREATE TRIGGER statement and all SQL statements that comprehensively test a trigger in a script L1.sql.

Comprehensive testing means that the trigger must reject SQL statements that violate the consistency constraint and accept SQL statements that do not violate the consistency constraint. It is a part of your task to find what SQL statements should be tested. Whenever SQL statement violates the consistency constraint a trigger must return ORA-…

error message. Use a procedure RAISE_APPLICATION_ERROR(-20001,’YOUR MESSAGE HERE’)to return ORA-… error message. If SQL statement does not violate the consistency constraint then a trigger must return no messages.

Your report must include listing of all SQL statement processed. To achieve that put the following SQL*Plus commands:




SET ECHO ON

SET FEEDBACK ON

at  the beginning of SQL script L1.sql.




<strong>Deliverables </strong>

Submit SQL script L1.sql. The report MUST have no errors other than reported by a trigger and the report MUST list all SQL statements processed. The report MUST include ONLY SQL statements and control statements that implement the specifications of Task 1 and NO OTHER statements.

A report that contains no listing of executed SQL statements scores no marks!




A report that contains any kind of processing errors other than reported by a trigger scores no marks!




Submission of a file with a different name and/or different extension and/or different type scores no marks!

<strong> </strong><strong>                                                                                                                                      </strong>

<strong> </strong>

It is expected that all tasks included within <strong>Laboratory 1</strong> will be solved <strong>individually without any cooperation</strong> with the other students.  If you have any doubts, questions, etc. please consult your lecturer or tutor during lab classes or office hours. Plagiarism will result in a <strong><u>FAIL</u></strong> grade being recorded for that assessment task.




<em>End of specification </em>