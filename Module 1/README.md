# Модуль 1 - Домашнее задание

## Архитектура Аналитического решения (Фармацевтическая компания)

[Ссылка на файл в draw.io](https://github.com/nikita-volynets/Data-learn-homework/blob/fa1775525d017a9bc974455457bf65e0bc965867/Module%201/Ar%D1%81hitecture_Pharma.drawio)

Создал с помощью draw.io схему аналитического решения для Фармацевтической компании.

![Schema](https://github.com/nikita-volynets/Data-learn-homework/blob/c819970be16a2bf72dccdb6e068cb853df11386c/Module%201/Architecture_Pharma.JPG)

## Аналитика в Excel (Superstore)

### Функционал Excel

С пощью Excel создал Дэшборд на основе данных из файла Superstore.

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

![Pivot](https://github.com/nikita-volynets/Data-learn-homework/blob/9c651703a0e10c3e905815c947f5f84691e51a83/Module%201/Picture_Pivot.JPG)

+ Для вычисление некоторых метрик использовал вычисляемые столбцы в сводных таблицах

![Calculated](https://github.com/nikita-volynets/Data-learn-homework/blob/9c651703a0e10c3e905815c947f5f84691e51a83/Module%201/Picture_Calculated_Column.JPG)

+ Отключил авторегулирование размера в сводных таблицах для улучшения быстродействия

![Autofit](https://github.com/nikita-volynets/Data-learn-homework/blob/9c651703a0e10c3e905815c947f5f84691e51a83/Module%201/Picture_Autofit.JPG)

### Бизнес-логика и создание Дэшборда
