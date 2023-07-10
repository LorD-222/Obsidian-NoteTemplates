---
tags: [Daily]
---
### Задачи на сегодня
#### 📝 Планируемые

- [ ] План 1
- [ ] План 2
- [ ] План 3

#### 🎯 Дополнительно выполненные

- [ ] План 1
- [ ] План 2
- [ ] План 3
---

### 📅 За день

#### 🗞 Новости

{{Запишите здесь интересные или важные новости, которые вы прочитали или услышали сегодня}}

#### 🧠 Что я узнал

{{Запишите здесь любые новые факты, навыки или информацию, которые вы узнали сегодня}}

---
### 📈 Показатели

В часах:
Work Time:: 
Sleep Time:: 
Learning Time:: 
Physical Activity:: 

От 1 до 10
Happiness:: 
Stress:: 
Health:: 
Productivity:: 

---
### 🗒️ Заметки сегодняшнего дня

```dataview
list from ""
where (
    ((file.mtime >= date(<% tp.date.now("YYYY-MM-DD") %>) and file.mtime < date(<% tp.date.now("YYYY-MM-DD", 1) %>)) or 
    (file.ctime >= date(<% tp.date.now("YYYY-MM-DD") %>) and file.ctime < date(<% tp.date.now("YYYY-MM-DD", 1) %>))) 
    and !contains(file.folder, "RSS")
)
sort file.ctime desc
```
