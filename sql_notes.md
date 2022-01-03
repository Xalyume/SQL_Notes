General syntax for making a raw SQL query:

SELECT column_name1, column_name2 FROM database
    WHERE conditional (WHERE is an optional filtering keyword)

in the conditional you can use the following additional operators:
IN - check if an item is in a provided list
BETWEEN - allows for range checking (the range is inclusive of both provided boundary values
)
LIKE - logical operator to apply an additional filter in your WHERE filter. The % wildcard symbol is used in conjunction with the the LIKE operation.
e.g - WHERE name LIKE 'J%' returns all names in a table that start with a capital J

Additional Notes:
Lists related to the IN operator must be in parenthesis
String values (not column names) must be wrapped in single quotes.
