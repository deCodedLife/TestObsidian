# Concept

My app is based on "TRY N5" textbook. This textbook cointain a list of topics. So I should create a page where user can select topic and start learning or practice.

> ## Todo
> 
> - [x] Create database

---

## Database

Topics table should contain:
- id
- topic

```
create table if not exists Topics (id INTEGER NOT NULL UNIQUE, topic TEXT NOT NULL, PRIMARY KEY (id AUTOINCREMENT))
```

