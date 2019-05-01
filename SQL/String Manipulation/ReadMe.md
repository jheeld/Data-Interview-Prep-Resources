## String Functions

From [Basics of String Manipulations:](https://www.decisivedata.net/blog/cleaning-messy-data-sql-part-3-sql-functions-clean-strings) 
> SUBSTRING() is the foundation of all string cleanup. It returns a portion of a string using this syntax: SUBSTRING(Original string, Starting position, Length of new string).

> LEN() returns the length of a string. This is especially useful when used in combination with SUBSTRING(). Its syntax is LEN(String).

> LEFT() and RIGHT() are similar to SUBSTRING(), except that instead of indicating a starting position, they either start from the start or the end of the string respectively. Both have the syntax (Original string, Length of new string).

> LTRIM() and RTRIM() remove spaces from the start and end of a string, respectively. For example, LTRIM(‘ Active’) would return ‘Active’.

> CHARINDEX() allows you to determine if a string contains a certain character. If it does, it will return an integer that indicates the position in the string of your desired character. If the character is not present, it returns zero. The syntax is CHARINDEX(Character you’re searching for, String you’re searching in, [Position to start searching from]). The last parameter is optional; the default is 1 (the beginning of the string).


> ISNUMERIC() tells you if a string can be successfully converted into a numeric data type. If so, it returns one, and if not, zero. The syntax is ISNUMERIC(String).

### Useful Links

* [Dirty Joins](https://www.essentialsql.com/how-to-join-dirty-data-in-sql-server/)
