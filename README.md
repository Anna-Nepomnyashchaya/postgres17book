### postgres_17_study_book
#### Author Непомнящая Анна Вадимовна
## My first steps in learning Postgres


### Lesson 1

Развернула Postgres 17 в cloud.tp на виртуалке, поняла что не знаю пароль от sudo. Пока не смогла исправить эту проблему.

Поэтому воспользовалась betta фичей, в клауде перешла во вкладку PostgreSQL и нажала "Создать кластер"
Создался кластер PostgreSQL 14.13 (Debian 14.13-1.pgdg110+1)

Подключилась через teleport, чтобы не сильно расходовать ресурсы клауда, загрузила самый маленький датасет на 600 MB
```
wget https://storage.googleapis.com/thaibus/thai_small.tar.gz && tar -xf thai_small.tar.gz && psql "host=ip port=5000 dbname=thai user=postgres" < thai.sql
```

Выполнила
```
SELECT count(*) FROM book.tickets;
```
Получила результат
```
5185505
```
















