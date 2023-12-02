# Harvard CS50 - Computer Science Projects
Hello, world! This is CS50, Harvard University's introduction to the intellectual enterprises of computer science and the art of programming.

Topics include:
--
Computer Science. Computational Thinking. Problem Solving: Inputs, Outputs. Representation: Unary, Binary, Decimal, ASCII, Unicode, RGB. Abstraction. Algorithms. Running Times. Pseudocode. Scratch: Functions, Arguments, Return Values; Variables; Boolean Expressions, Conditionals; Loops; Events; Threads.

This is a 12-week course:
--

Week 1 - Scratch.

Week 2 - C.

Week 3 - Arrays.

Week 4 - Algorithms.

Week 5 - Memory (Hexadecimal, Pointer, Defining Custom Types, Dynamic Memory Allocation, Call Stacks, File Pointers).

Week 6 - Data Structures (Queue, Stack, Singly-Linked list, Doubly-Linked List, Binary Search Tree, Hash table, Tries).

Week 7 - Python
--
(Strings, Dot notation, Loops, Tuples, Dictionaries, Libraries, File reading, Writing; other topics: Floating point imprecision, Integer Overflow).
Python syntax: Variables, Conditionals, Loops, Arrays, Lists, Tuples, Dictionaries, Functions, Objects, Style.

Week 8 - SQL
--
Structured Query Language (Relational databases,...). Potential problems: race conditions, SQL injection attacks (little Bobby Tables).

SQL is a programming language whose purpose is to query a database.

MySQL is one open-source platform on which you can establish the type of relational database that SQL is most adept at working with.

SQLite is another platform.

Many installations of SQL come with a GUI tool called phpMyAdmin which can be used to execute database queries in a more user-friendly way.

5 common Data types in SQLite:
--
BLOB(Binary large objects)

INTEGER

NUMERIC(YYYY-MM-DD)

REAL(float, decimal point with some number of digits thereafter)

TEXT

CRUD functions:
--
        to create data: CREATE, INSERT.
        to read data: SELECT.
        to update data: UPDATE.
        to delete data: DELETE, DROP.
 
Other functions: 
--
AVG, COUNT, DISTINCT, LOWER, MAX, MIN, UPPER,...
WHERE, LIKE, ORDER BY, LIMIT, GROUP BY.

Example of functions & queries:
--
SELECT * FROM favorites;  (to select all).

SELECT * FROM people WHERE name LIKE 'Steve C%';

SELECT * FROM people WHERE name LIKE 'Steve C%';

SELECT COUNT(show_id) FROM genres WHERE genre = 'Comedy';

SELECT title FROM shows WHERE id IN (SELECT show_id FROM genres WHERE genre = 'Comedy') ORDER BY title LIMIT 10;

Nested query:
SELECT title FROM shows WHERE id IN (SELECT show_id FROM stars WHERE person_id = (SELECT id FROM people WHERE name = 'Steve Carell'));

Join query:
SELECT * FROM shows 
JOIN ratings ON shows.id = ratings.show_id 
WHERE title = 'The Office';

SELECT * FROM students 
JOIN assignments ON students.id = assignments.student_id
JOIN houses ON houses.id = assignments.house_id;

CREATE TABLE movies (
                    id INTEGER,
                    title TEXT NOT NULL,
                    year NUMERIC,
                    PRIMARY KEY(id)
                );
                
CREATE TABLE stars (
                movie_id INTEGER NOT NULL,
                person_id INTEGER NOT NULL,
                FOREIGN KEY(movie_id) REFERENCES movies(id),
                FOREIGN KEY(person_id) REFERENCES people(id)
            );

UPDATE favorites SET language = 'C' WHERE language ='C++';  (to replace data in the column).

DELETE FROM favorites WHERE problem = 'Tideman';

CREATE INDEX title_index ON shows (title);

IMDb = Internet Movie Database.

TSV = Tab Separated Value.

Week 9 - HTML, CSS, JavaScript.
--
**1. How the internet works?** (first 50 mins)

IP = Internet Protocols 

TCP = Transmission Control Protocol

DNS = Domain Name System

DNS = Domain Name System

HTTP = Hypertext Transfer Protocol

HTTP = Hypertext Transfer Protocol

TLD = Top Level Domain

curl = connect URL

200 OK

301 Moved Permanently

302 Found

304 Not Modified

307 Temporary Redirect

401 Unauthorized

403 Forbidden

404 Not Found

418 I'm a Teapot

500 Internal Server Error

503 Service Unavailable


**2. HTML**

Tags:

'ul' means Unordered List

'ol' means Ordered List

'ls' means List

'tr' means Table Row

'div' means Division of the page

Attributes

**3. CSS**

CSS is not a programming language. It is a markup language to support the aesthetics of the page, things such as font size, colors, margin,...

Properties

Type selector

Class selector

ID selector

Attribute selector
   
Week 10 - Flask.
--

Week 11 - Emoji.

Week 12 - Cybersecurity.

*Notes:
--

Ctrl+C to interrupt computer

PRIMARY KEY: is the unique identifier & the unique ID inside of the table.

FOREIGN KEY: is the reference to that primary key from another table, a separate table.

Does FOREIGN KEY have to set the relationship? when you create the table, the programmer or the database administrator would create that relationship by using those keywords: primary key and foreign key that teaches the database what is related to what.
