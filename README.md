# Проект Анализ данных 2024

## Описание проекта 

Данный проект посвящен анализу данных о билетах авиакомпаний с целью исследования различных аспектов авиаперевозок, включая ценообразование, предпочтения по времени отправления, влияние конкуренции на цены и услуги, а также другие важные характеристики рейсов.

## Используемые технологии и библиотеки

`Python`: язык программирования, используемый для обработки и анализа данных.

`Pandas` и `Numpy`: библиотеки для манипуляции с данными и анализа.

`Matplotlib` и `Seaborn`: библиотеки для визуализации данных.

`Sklearn`: библиотека для обучения моделей.



## Структура проекта:
- `parser_tuturu.ipynb` - блокнот с парсером, который с сайта tutu.ru достает информацию по авиабилетам.
- `raw_data.txt` - данные, полученные с помощью парсера.
- `data.txt` - предобработанные данные.
- `from_raw_to_clear.ipynb` - блокнот с кодом, который обрабатывает файл `raw_data.txt` в `data.txt`.
- `DA_project.ipynb` - блокнот, в котором происходит вся обработка датасета `data.txt`, визуализация, проверка гипотез, выводы, обучение модели предсказания цены билеты.

## Гипотезы
- цена авиабилета не зависит от времени отправления (исследовать среднюю стоимость билета в среднем по часам суток)
- цена авиабилета не зависит от дня недели (исследовать среднюю стоимость билета в среднем по дням недели)
- авиакомпании назначают одинаковые цены за билеты (исследовать зависимость авиабилета от авиакомпании)
- если по маршруту выполняется малое количество рейсов, то цена авиабилетов по данному маршруту выше
- цена на авиабилеты не зависит от самолета 
- на короткие рейсы билеты чаще всего продаются (и соотв покупаются) в утренние и вечерние часы, на длинные рейсы чаще в вечерние часы
- при высокой конкуренции на маршруте (много авиакомпаний продают билеты на определенное направление) предоставлется больше услуг (больше размер багажа, возможность возврата, возможность обмена)

## Модель МО

Мы ставим задачу предсказания цены авиабилета, поэтому будем использовать линейную регрессию.

