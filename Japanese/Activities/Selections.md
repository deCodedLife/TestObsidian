# Concept

This page are simmillar with [[Tests]]. But instead of multiple selection it will be single. One question and multiple answers. User should choose correct answer for current task. 

> ## Todo
> 
> - [x] Create Selections database

---

## Database

Table Selections should contain
- id of task
- question
- answers
- correct answer

```
create table if not exists Selections (id INTEGER NOT NULL UNIQUE, question TEXT NOT NULL, variants TEXT NOT NULL, answer TEXT NOT NULL, PRIMARY KEY(id AUTOINCREMENT) )
```

---

## Implementation

![[Submit.png]]

All content will be placed on long card. Question and answers will be separated by horizontal line. And it will be a submit button at right bottom corner. Also there should be some japanese backgrounds as option.