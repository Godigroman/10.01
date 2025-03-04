# Домашнее задание к занятию "`Базы данных`" - `Клименко Олег`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Легенда

Заказчик передал вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/resources/hw-12-1.xlsx), в котором сформирован отчёт.

![](https://cdn.discordapp.com/attachments/1258765702450380901/1260920515225452595/image.png?ex=6691133d&is=668fc1bd&hm=2e94d98cfec28323154c89db47460ed8b91ef77ded1cd3a0cc243697e7470554&)

На основе этого отчёта нужно выполнить следующие задания.

### Задание 1

Опишите не менее семи таблиц, из которых состоит база данных:

- какие данные хранятся в этих таблицах;
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL. Приведите решение к следующему виду:

**Сотрудники** (

- идентификатор, первичный ключ, serial,
- фамилия varchar(50),
- ...
- идентификатор структурного подразделения, внешний ключ, integer).

**Решение:**

### 1 сотрудники (

- идентификатор сотрудника, первичный ключ, SERIAL,
- Ф.И.О. VARCHAR(50),
- дата найма DATE,
- оклад DECIMAL(10,2),
- идентификатор должности, внешний ключ, INTEGER,
- идентификатор структурного подразделения, внешний ключ, INTEGER)

---

### 2 тип подразделения (

- идентификатор типа подразделения, первичный ключ, SERIAL,
- тип подразделения VARCHAR(20))

---

### 3 структурное подразделение (

- идентификатор структурного подразделения, первичный ключ, SERIAL,
- структурное подразделение VARCHAR(60),
- идентификатор типа подразделения, внешний ключ, INTEGER
- идентификатор филиала, внешний ключ, INTEGER)

---

### 4 адрес филиала (

- идентификатор филиала, первичный ключ, SERIAL,
- адрес филиала VARCHAR(60))

---

### 5 должность (

- идентификатор должности, первичный ключ, SERIAL,
- должность VARCHAR(50))

---

### 6 проект (

- идентификатор проекта, первичный ключ, SERIAL,
- название проекта VARCHAR(30))

---

### 7 назначение на проект (

- идентификатор сотрудника, внешний ключ, INTEGER,
- идентификатор проекта, внешний ключ, INTEGER,)

---
---
























