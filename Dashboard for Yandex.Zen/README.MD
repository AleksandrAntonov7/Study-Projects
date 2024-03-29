# [Dashboard for Yandex.Zen](https://public.tableau.com/app/profile/aleksandr.antonov/viz/__16496753424850/_)
# Описание:
В целях оптимизации отчетности необходимо построить дашборд для менеджеров по анализу контента.

Дашборд позволит ответить на следующие вопросы:
- Сколько взаимодействий пользователей с карточками происходит в системе с разбивкой по темам карточек?
- Как много событий генерируют источники с разными темами?
- Как соотносятся темы карточек и темы источников?

## Данные:
Выгрузка данных из системы Яндекс.Дзен за 24.09.2019 (таблица dash_visits.csv):
- `record_id` — уникальный идентификатор записи в файле
- `item_topic` — тема карточки
- `source_topic` — источник карточки (тема)
- `age_segment` — возрастной сегмент пользователя
- `dt` — дата и время события
- `visits` - количество событий (взаимодействий) с карточками Яндекс.Дзен

## Использованные библиотеки:
- pandas
- sqlalchemy.create_engine
- tableau

## В проекте использованы следующие этапы:
- [Выгрузка](https://github.com/AleksandrAntonov7/Study-Projects/blob/main/Dashboard%20for%20Yandex.Zen/%D0%92%D1%8B%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D1%84%D0%B0%D0%B9%D0%BB%D0%B0%20dash_visits.ipynb) данных (`Jupyter Notebook`)
- Построение дашборда (`Tableau`)
- Подготовка [презентации](https://github.com/AleksandrAntonov7/Study-Projects/blob/main/Dashboard%20for%20Yandex.Zen/%D0%9F%D1%80%D0%B5%D0%B7%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D1%8F%20%D0%AF%D0%BD%D0%B4%D0%B5%D0%BA%D1%81.%D0%94%D0%B7%D0%B5%D0%BD.pdf) для пользователей дашборда (`PowerPoint` → `pdf`)

## Выводы:
- Пользователи взаимодействуют с карточками крайне неравномерно: есть периоды высокой активности, есть периоды минимального взаимодействия.
- Наибольшее количество взаимодействий с карточками по темам «Наука», «Отношения», «Интересные факты»; наименьшее – «Женская психология», «Шоу» и «Знаменитости».
- Самые популярные источники: «Семейные отношения», «Россия» и «Полезные советы.
- Темы карточек и темы источников могут соотноситься различным образом.

## Ссылка на интерактивный дашборд (Tableau):
[Дашборд](https://public.tableau.com/app/profile/aleksandr.antonov/viz/__16496753424850/_)
