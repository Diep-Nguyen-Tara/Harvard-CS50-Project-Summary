# Harvard CS50 - Computer Science Projects
Hello, world! This is CS50, Harvard University's introduction to the intellectual enterprises of computer science and the art of programming.

Topics include: Computer Science. Computational Thinking. Problem Solving: Inputs, Outputs. Representation: Unary, Binary, Decimal, ASCII, Unicode, RGB. Abstraction. Algorithms. Running Times. Pseudocode. Scratch: Functions, Arguments, Return Values; Variables; Boolean Expressions, Conditionals; Loops; Events; Threads.

This is a 12-week course:
--

Week 1 - Scratch.

Week 2 - C.

Week 3 - Arrays.

Week 4 - Algorithms.

Week 5 - Memory (Hexadecimal, Pointer, Defining Custom Types, Dynamic Memory Allocation, Call Stacks, File Pointers).

Week 6 - Data Structures (Queue, Stack, Singly-Linked list, Doubly-Linked List, Binary Search Tree, Hash table, Tries).

Week 7 - Python 3 (Strings, Dot notation, Loops, Tuples, Dictionaries, Libraries, File reading, Writing; other topics: Floating point imprecision, Integer Overflow).
Python syntax: Variables, Conditionals, Loops, Arrays, Lists, Tuples, Dictionaries, Functions, Objects, Style.

Week 8 - SQL - Structured Query Language (Relational databases,...).

5 Data types in SQLite:
--
BLOB(Binary large objects), INTEGER, NUMERIC(YYYY-MM-DD), REAL(float, decimal point with some number of digits thereafter), TEXT,...

PRIMARY KEY column: the database will use that column as the unique identifier.

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

Example of functions:
--
SELECT * FROM favorites;  (to select all).

SELECT COUNT(show_id) FROM genres WHERE genre = 'Comedy';

SELECT title FROM shows WHERE id IN (SELECT show_id FROM genres WHERE genre = 'Comedy') ORDER BY title LIMIT 10;

UPDATE favorites SET language = 'C' WHERE language ='C++';  (to replace data in the column).

DELETE FROM favorites WHERE problem = 'Tideman';

IMDb = Internet Movie Database.
TSV = Tab Separated Value.

Week 9 - HTML, CSS, JavaScript.

Week 10 - Flask.

Week 11 - Emoji.

Week 12 - Cybersecurity.

*Notes:
--

Ctrl+C to interrupt computer
