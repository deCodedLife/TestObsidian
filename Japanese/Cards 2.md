# Concept

#japanese

Cards was created for learning kanji. Card is square with rounded corners which contain some text. When user tap to card it will change content information.

If user get tired he can switch to [[Compare game]] which will do same concept, but in a game like mode.

> ## Todo
> 
> - [x] Card element
> - [x] Content switching
> - [x] Card disapearing
> - [x] Drag animation
> - [x] Connect score

---

## Card switching

For switching to next kanji drag animation was implemented. Now user can hold card and flip it to right or left side. Card will disapear and after new card with next kanji will appear.

| ![[DragAnimation.jpg]] | ![[DisapearAnimation.jpg]] |
| --- | --- |

---

## Database

Words table should contain
- word id
- Japanese kanji
- Russian translation
- Onyoumi and Kunyomi

```
create table if not exists Words (id INTEGER NOT NULL UNIQUE, ja TEXT NOT NULL, ru TEXT NOT NULL, pr TEXT NOT NULL, PRIMARY KEY(id AUTOINCREMENT) )
```