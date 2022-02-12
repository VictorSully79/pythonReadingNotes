# Automation

notes taken from <https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial>

## Python Regex

- Regex checks to see if a pattern of text exists. It's often used to verify or validate the format of strings in programming.

- Regular Expressions in Python are suported by the "re" module and need to be imported.

## Basic Patterns

- Used to perform matches on ordinary characters. They match themselves exactly.

- Match function will return a match. Otherwise it is "None"

## Wild Card Characters:

- These charcters have special meaning. They do not match themselvers but denote something else.

- The "Search" function can scan a string or sequence. The "Group" function returns a string matched by the "re".

## Repetitions

- Special charachters can be used to check for repitition.

- See <https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial> for more information.

## Grouping

- The "group" function allows regex to pick up parts of matching text.

- You can also group useing "<>".

## Greedy vs. Non-Greedy Matching

- Normally regex will try and match as much of the string as possible.  This is called a greedy match.

- Add "?" to match as little as possible. 