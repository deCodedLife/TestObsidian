# Concept 

#japanese

The progress system is essentially the number of points that are reset each day. When completing the exercise, for each completed task, the user receives a certain number of points. Progress should be categorized. Actions in the current category do not affect progress in others.

All this in the compartment must be synchronized with statistics on the server [[Sync]]

---

> ## Todo
>
> - [ ] Add scoring animation
> - [x] Add progressbar
> - [ ] Add effects

---

## Database


```
create table if not exists Stats (id INTEGER NOT NULL UNIQUE, date TEXT NOT NULL, score TEXT NOT NULL, PRIMARY KEY(id AUTOINCREMENT))

create table if not exists User (id INTEGER NOT NULL UNIQUE, name TEXT NOT NULL, serverUri TEXT NOT NULL, PRIMARY KEY(id AUTOINCREMENT))
```

- [x] Add table Stats
- [x] Add table User

## Interface

To indicate user progress is using standart progressbar in  [QtQuick.Controlls 2](https://doc.qt.io/qt-5/qml-qtquick-controls2-progressbar.html). It should be placed at the top of action page.

---

| ![[progress_showcase0.jpg]] | ![[progress_showcase1.jpg]] |
| --- | --- |