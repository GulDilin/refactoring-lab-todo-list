# refactoring-lab-todo-list
Laboratory works of DB Refactoring. Software Engineering Course ITMO 4-year. Simple cli client server app for tasks management 

## How to run
1. Start api server
2. Start client

More info in client and server repos

## Task description
### English
Requirements

Main menu need to contain next functions:

    add new task
    actual tasks search by tags
    exit

For choose menu point user should write a number
Task structure

    title
    description
    deadline
    tags

Functionality requirements

    To choose a menu point user need to type a number
    When user add a task, all fields should be included
    Tags input processing ends with blank line
    String with words separated by space is using for tags search. Tasks need to be returned sorted by deadline date.

### Russian
Требования

Главное меню программы включает следующие пронумерованные пункты:

    добавление новой задачи
    поиск задач по тэгам вывод N наиболее актуальных задач
    выход.

    Для выбора нужного пункта меню пользователь вводит соответствующий номер.
    При добавлении новой задачи пользователь последовательно вводит тему задачи, описание, дату к которой задача должна быть готова и тэги.
    Ввод тэгов продолжается до тех пор, пока пользователь не введет пустую строку.
    Для поиска пользователь вводит через пробел ключевые слова, наличие которых среди тэгов задачи является критерием выборки. Вывод актуальных задач осуществляется в отсортированном по дате готовности порядке.

### Example of interraction:
```shell
V:\> todo.exe
Enter the number of action and press [Enter]. Then follow instructions.
Menu:
1. Add task
2. Search task
3. Last tasks
   4.Exit
> 1
New task
Title: some task
Description: some text
Deadline: 10.11.2012
Tags (finish on empty line)
1: tagA
2: tagB
3:
Menu:
1. Add task
2. Search task
3. Last tasks
   4.Exit
> 2
Search tasks by tag: tagC
No such tasks
Menu:
1. Add task
2. Search task
3. Last tasks
   4.Exit
> 3
Actual tasks:
1. Title: some task
   Description: some text
   Deadline: 10.11.2012
   Tags: tagA, tagB
   Menu:
1. Add task
2. Search task
3. Last tasks
   4.Exit
> 4
V:\>
```
