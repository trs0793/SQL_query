# SQL_query (English)
### 1) Goal and Task Statement #1:

Educational courses consist of various lessons, each containing several small tasks. **The task was to write an optimal query that provides information about the number of very diligent students**. A diligent student is defined as one who correctly solved 20 tasks in the current month.

Tools used in project execution:

- Sorting with ORDER BY
- Filters with HAVING and aggregate functions like COUNT
- Time structure manipulation with toStartOfMonth

### Result:
The number of very diligent students = 136

### 2) Goal and Task Statement #2:

The educational platform offers students courses in a trial model: a student can solve only 30 tasks for free each day. For unlimited tasks in a specific discipline, the student needs to purchase full access. The team conducted an experiment where a new payment screen was tested.

**The task was to extract the following information about user groups in a single query:**

- ARPU (Average Revenue Per User)
- ARPPU (Average Revenue Per Paying User)
- Conversion rate (CR) to purchase
- CR of an active user to purchase
- CR of a user active in mathematics (subject = 'math') to purchase the mathematics course

ARPU is calculated considering all users in the groups.
An active user is defined as someone who has correctly solved more than 10 tasks in any discipline over time.
An active user in mathematics is defined as someone who has correctly solved 2 or more tasks in mathematics over time.

**Tools used in project execution:**

- Grouping with `GROUP BY`
- Sorting with `ORDER BY`
- Filters with `WHERE`, `HAVING`, and aggregate functions like `COUNT`, `COUNTIf`, `SUM`, `uniqExact`
- Complex joins with `FULL`, `INNER JOIN`
- Time structure manipulation with `toStartOfMonth`
- Subquery usage

### Result:

In a single query, I extracted financial metrics for the company: ARPU, ARPPU, and conversion rates (CR) for users in the test and control groups for comparison.

# SQL_query (Rusian)
### 1) Цель и условие задачи №1:

Образовательные курсы состоят из различных уроков, каждый из которых состоит из нескольких маленьких заданий. **Необходимо было написать оптимальный запрос, который даст информацию о количестве очень усердных студентов.** Под усердным студентом мы понимаем студента, который правильно решил 20 задач за текущий месяц.

Во время выполнения проектов я применял следующе инструменты:

- сортировки ORDER BY;
- фильтры HAVING и агрегатные функции COUNT
- изменение структуры времени toStartOfMonth;

### Результат:
Количестве очень усердных студентов = 136

### 2) Цель и условие задачи №2:

Образовательная платформа предлагает пройти студентам курсы по модели trial: студент может решить бесплатно лишь 30 задач в день. Для неограниченного количества заданий в определенной дисциплине студенту необходимо приобрести полный доступ. Команда провела эксперимент, где был протестирован новый экран оплаты.

**Мне необходимо было в одном запросе выгрузить следующую информацию о группах пользователей:**

- ARPU (Среднее значение зароботка компании с клиента)
- ARPPU (Среднее значение зароботка компании с платящего клиента)
- CR в покупку 
- СR активного пользователя в покупку 
- CR пользователя из активности по математике (subject = ’math’) в покупку курса по математике

ARPU считается относительно всех пользователей, попавших в группы.
Активным считается пользователь, за все время решивший больше 10 задач правильно в любых дисциплинах.
Активным по математике считается пользователь, за все время решивший 2 или больше задач правильно по математике.

**Во время выполнения проектов я применял следующе инструменты:**

- группировки GROUP BY;
- сортировки ORDER BY;
- фильтры WHERE, HAVING и агрегатные функции COUNT, COUNTIf, SUM, uniqExact;
- выполнение сложных джоинов FULL, INNER JOIN;
- изменение структуры времени toStartOfMonth;
- использование подзапросов.

### Результат:

Одним запросом вывел финансовые показатели компании ARPU, ARPPU, и конверсии CR пользователей в тестовой и контрольной группе для сравнения.
