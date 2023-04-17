# Модуль 1 - Домашнее задание

## Архитектура Аналитического решения (Фармацевтическая компания)

[Ссылка на файл в draw.io](https://github.com/nikita-volynets/Data-learn-homework/blob/fa1775525d017a9bc974455457bf65e0bc965867/Module%201/Ar%D1%81hitecture_Pharma.drawio)

Создал с помощью draw.io схему аналитического решения для Фармацевтической компании.

![Schema](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Architecture_Pharma.JPG)

## Аналитика в Excel (Superstore)

[Ссылка на файл с Дэшбордом в Excel](https://github.com/nikita-volynets/Data-learn-homework/blob/f080ab1d5acdc44fa0dd994820fb1acf0e49c38c/Module%201/Excel%20Dashboard%20-%20Superstore.xlsx)

### Функционал Excel

С помощью Excel создал Дэшборд на основе данных из исходного файла Superstore.

+ С помощью функции **XLOOKUP** подтянул данные по Региональным Менеджерам и по Возвратам в основную таблицу
```
=XLOOKUP(B4,Returns!B:B,Returns!A:A,"No",)
=XLOOKUP(O6,People!B:B,People!A:A,0,)
```

+ С помощью функции **TEXT** привел дату в нужный формат 

```
=TEXT([@[Order Date]],"гггг-ММ (ММММ гг)")
```

+ Создал сводные таблицы по различным метрикам для Дэшборда

![Pivot](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Pivot.JPG)

+ Для вычисление некоторых метрик использовал вычисляемые столбцы в сводных таблицах

![Calculated](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Calculated_Column.JPG)

+ Отключил авторегулирование размера в сводных таблицах для улучшения быстродействия

![Autofit](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Autofit.JPG)

### Дэшборд

1. Overview - Название, фильтры в виде срезов и ключевые метрики

![Overview](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Overview.JPG)

2. Динамика выручки и прибыли, а также прибыль по сотрудникам

![Dynamic](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Dynamic.JPG)

3. Продажи продуктов по категориям, а также ТОП-5 клиентов в каждой категории

![Category](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Category.JPG)

4. Прибыль по штатам США

![Geo](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Geo.JPG)

