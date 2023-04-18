# SQL (BigQuery) statements and commands guide

The 3 key statements in the SQL language are the following:
- SELECT = the column you want to pull the data from (e.g. students_age column)
- FROM = where is the column located (i.e. in which table?) (e.g. students_2023uptake table)
- WHERE = is used to pull data that matches a certain condition (e.g. only female students)
-     SELECT 
        students_age
      FROM
        students_2023uptake
      WHERE
        sex = 'F';

Things to rember:
- semicolon ; at the end of the statement
- asterisk select all the columns in the table
-     SELECT*
- comments
-     can be placed /* here */
      or after -- here
- wildcard
-     'cho%' (chocolate, choice, chore, etc.)

Operators. The WHERE clause can be conbined with:
- AND - displays a record if all the conditions separated by AND are TRUE
- OR - displays a record if any of the conditions separated by OR is TRUE

The AND and OR operators are used to filter records based on more than one condition

- NOT - displays a record if the condition(s) is NOT TRUE
<br />

The following are the main commands/clause:
-	DISTINCT - selects only unique values
-	    SELECT 
	      DISTINCT students_age
-	COUNT - it counts the instances
-	    SELECT
	      COUNT(DISTINCT students_age)
-	AS - creates an alias variable/column
-	    SELECT
	      COUNT(DISTINCT students_age) AS count_of_distinct_ages
-	LIKE - search for a pattern
-	    SELECT
          first_name
        FROM
          students_2023uptake
        WHERE
          first_name LIKE 'Mar%'; (i.e. Martin, Mark, Marta, etc.)
-	UPDATE - updates data in a database
-	DELETE - deletes data from a database
-	INSERT INTO - inserts new data into a database
-	CREATE DATABASE - creates a new database
-	ALTER DATABASE - modifies a database
-	CREATE TABLE - creates a new table
-	ALTER TABLE - modifies a table
-	DROP TABLE - deletes a table
-	CREATE INDEX - creates an index (search key)
-	DROP INDEX - deletes an index
