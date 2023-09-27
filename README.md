# Автомобильный каталог и фильтр

Этот скрипт Python представляет собой автомобильный каталог и функцию фильтрации, которая позволяет выбирать автомобили по определенным параметрам. В каталоге хранятся данные о различных моделях автомобилей, такие как цена, объем двигателя, время разгона до 100 км/ч, привод, дата выпуска и страна-производитель.

## Использование скрипта

Для использования этого скрипта, вам потребуется Python. Вы можете скопировать и вставить его в свою среду разработки или запустить его в командной строке. Вот, как его использовать:

1. Определите данные о различных моделях автомобилей в словаре `cars`. Каждая модель имеет уникальный ключ, который представляет собой кортеж с названием машины и ее классом.

2. Вызовите функцию `filter_cars` с каталогом машин, параметром для фильтрации и критерием. Например, `filter_cars(cars_catalog, 'Цена', 50000)` вернет список автомобилей с ценой 50000.

3. Результат будет представлен списком автомобилей, удовлетворяющих заданным критериям.

## Пример
``
```python
cars = {
    ("Машина1", "Седан"): {
        "Цена": 50000,
        "Объем двигателя": 2.0,
        "Время разгона до 100 км": 7.5,
        "Привод": "Задний",
        "Дата Выпуска": "2022-01-15",
        "Страна производитель": "Германия"
    },
    # ... (другие модели автомобилей) ...
}

cars_catalog = []
for car, car_info in cars.items():
    cars_catalog.append({car: car_info})

filtered_cars = filter_cars(cars_catalog, 'Цена', 50000)
print(filtered_cars)
```

Этот код выведет список автомобилей с ценой 50000.

С помощью этого скрипта вы можете легко фильтровать и находить интересующие вас автомобили в автомобильном каталоге, используя различные параметры и критерии.