# Database-Systems-CSCI-4380-01-Homework-1-solution

Download Here: [Database Systems, CSCI 4380-01 Homework #1 solution](https://jarviscodinghub.com/assignment/database-systems-csci-4380-01-homework-1-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Homework Statement. This homework is worth 4% of your total grade. If you choose to skip it, Midterm #1 will be worth 4% more. Remember, practice is extremely important to do well in this class. I recommend that not only you solve this homework, but also work on homeworks from past semesters. Link to those is provided in the Piazza resources page. This homework aims to teach you how to construct complex queries using relational algebra. Please do the parts in sequence. The questions get harder and build on your knowledge of relational algebra from previous parts. Each question is equal weight. Database Description. Suppose you are given the following database for keeping track of grades in this course. students(rin, fname, lname, email, optin date, optout date)
exams(name, id, exam date, maxgrade, points)
examgrades(rin, name, id, grade)
hws(id, name, points, given date, due date, maxgrade, nextexam name, nextexam id)
hwgrades(rin, id, submission date, grade)
Each student may have an opt-in date, if there is no date (i.e. the value is NULL) then the homeworks are optional for this student. If there is an opt-in and no opt-out date, then homeworks are required. If there are dates for both opt-in and opt-out, only the homeworks that have a due date within within the given dates are required. The exams relation contains both quizzes and exams, stored in name, id ﬁelds as ’Exam’, 1, ’Exam’, 2, ’Exam’, 3 (for ﬁnal), or ’Quiz’, 1, ’Quiz’, 2, etc. The id is used to show which exam comes after another. The grade for each exam references both the name and the id of the exam for each student and their grade. Homeworks are stored similarly in the hws relation with id 1,2,3, etc. For each homework, the upcoming (midterm or ﬁnal) exam is listed. As discussed, points for skipped homeworks will count towards the next exam. The name for each homework is ’hw’ for simplicity. The grades for each homework is stored similarly in hwgrades where id is the id of the homework. Note: All date ﬁelds are formatted as mon-day-year, e.g. 01-31-2016. You can assume that you can check if a date value X comes after another value Y by checking whether X > Y. Write the following queries using relational algebra (pay attention to the attributes required in the output!): Question 1. The following queries only need a single SELECT (σ), followed by a PROJECT (π) and RENAMING (ρ) as necessary:
(a) Return the ﬁrst and last name of all students who have opted in to the homeworks before ’9/25/2018’ and did not opt out.
(b) Return the id and points for all homeworks that are due before ’Exam’, 2.
1
Question 2. The following queries combine SELECT (σ), SET operations (∩,∪,−), PROJECTION (π) and RENAMING (ρ) as necessary:
(a) Find and return the name, id and points of all exams and homeworks given or had due dates before ’11/22/2018’.
(b) Find the id of homeworks that no student has submitted.
(c) Find and return the RIN of all students who turned in both homeworks 1 and 2.
Question 3. The following queries combine SELECT (σ) statements with any number of JOINS as neede (./, theta or natural) (or CARTESIAN PRODUCT), followed by a PROJECT (π) and RENAMING (ρ) as necessary:
(a) Find the ﬁrst and last name of all students who submitted homework #1.
(b) Find the RIN and Exam 1 grades of all students who submitted at least one homework due before Exam 1.
Question 4. Freeform, you decide which combination is needed. Any relational algebra operator is ﬁne. Remember to construct these in parts and provide comments on what each part is computing. This will make it possible for us to give partial credit.
(a) For each student, return their RIN, name, exam/homework name, exam/homework id, grade and points for all exams (including quizzes) and homeworks that they have a grade for.
(b) Find and return the RIN and Exam 1 grade of the students who did not complete any of the homeworks before Exam 1.
If you are ﬁnished with all these queries but ﬁnd yourself in need of a personal challenge, try to write this query to explore the expressive power of relational algebra (no hw credit for this question): Find and return the RIN of all students who have completed all the assigned homeworks. Also try to ﬁnd students who completed two homeworks in a row. (No credit for these questions, try them to challenge yourself.)
SUBMISSION INSTRUCTIONS. Submit a PDF document for this homework using Gradescope. No other format and no hand written homeworks please. No late submissions will be allowed.
The gradescope for homework submissions will become available by Tuesday September 11 the latest. We will announce it on Piazza.
