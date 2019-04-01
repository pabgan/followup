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
pablo@maFalda:~$ todo.sh followup 48 "next thursday"
2019-04-04
48 x 2019-04-01 2019-04-01 test task
TODO: 48 marked as done.
x 2019-04-01 2019-04-01 test task
48 2019-04-01 @followup: test task t:2019-04-04
PERSONAL-TODO: 48 added.
```
