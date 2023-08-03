# Concept

The basic idea comes from original textbooks. There are a text with some word skips. User should fill this gaps correctly.

Most of the tests can be copied from original textbooks. It can be single sentense or large text.

For this activity I should create text formatter which will convert text with special tags to qml task. Programm should display text with tag corrections. Of the end of page will be placed comboboxes which will be connected with skiped words.

> ## Todo
> 
> - [x] Write concept
> - [x] Create table Tests

---

## Test example

Task is text with braces which will contain correct insertation.

私{は}猫{を}大好き。
Possible insertations: \[は,が,を,x\]

---

## Database

Table "Tetst" should contain
- id of a test
- test text
- possible insertations

```
create table if not exists Tests (id INTEGER NOT NULL UNIQUE, content TEXT NOT NULL, insertations TEXT NOT NULL, PRIMARY KEY(id AUTOINCREMENT))
```

---

## Text formatter

---

## Implement