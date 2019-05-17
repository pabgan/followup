followup
========
This is an addon to use with [todo.txt-cli](https://github.com/todotxt/todo.txt-cli).

Followup on done tasks to not forget to check if they are completely finished from every end.

Usage
-----
Provide the ID of a task you want to follow up and optionally a date.
```
	todo.sh followup ID [date]
```
This will mark that task as done and create a new one with the same text and the starting date provided as a parameter, written in natural language as accepted by `date --date`.

If no date is provided *"next week"* will be used by default.

For example:

```
pablo@maFalda:~$ todo.sh add test
16 2019-05-17 test
TRABAJO-TODO: 16 added.

pablo@maFalda:~$ todo.sh followup 16 "next thursday"
16 x 2019-05-17 2019-05-17 test
TODO: 16 marked as done.
17 2019-05-17 @followup: test t:2019-05-23
TRABAJO-TODO: 17 added.
```
