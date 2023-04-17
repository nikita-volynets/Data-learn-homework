# Module 1 - Homework

## Architecture of Analytical solution (Pharmaceutical company)

[Ссылка на файл в draw.io](https://github.com/nikita-volynets/Data-learn-homework/blob/fa1775525d017a9bc974455457bf65e0bc965867/Module%201/Ar%D1%81hitecture_Pharma.drawio)

Created with draw.io Architecture of Analytical solution for pharmaceutical company.

![Schema](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Architecture_Pharma.JPG)

## Analytics in Excel (Superstore)

[Ссылка на файл с Дэшбордом в Excel](https://github.com/nikita-volynets/Data-learn-homework/blob/f080ab1d5acdc44fa0dd994820fb1acf0e49c38c/Module%201/Excel%20Dashboard%20-%20Superstore.xlsx)

### Excel features

Created Dashboard with Excel based on the raw Supersotre file.

+ Used **XLOOKUP** function and added data about Regional Managers and Returns to the main table.
```
=XLOOKUP(B4,Returns!B:B,Returns!A:A,"No",)
=XLOOKUP(O6,People!B:B,People!A:A,0,)
```

+ Used **TEXT** function to convert date to the needed format.

```
=TEXT([@[Order Date]],"гггг-ММ (ММММ гг)")
```

+ Created Pivot tables with various metrics for the Dashboard.

![Pivot](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Pivot.JPG)

+ Used Calculated fields in Pivot tables for specific metrics

![Calculated](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Calculated_Column.JPG)

+ Disabled auto-size adjustment in pivot tables to improve performance

![Autofit](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Picture_Autofit.JPG)

### Dashboard

1. Overview - Name, slice filters and key metrics

![Overview](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Overview.JPG)

2. Sales and profit dynamic and profit by representatives

![Dynamic](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Dynamic.JPG)

3. Sales by categories, TOP-5 customers by category

![Category](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Category.JPG)

4. Profit by the US states

![Geo](https://github.com/nikita-volynets/Data-learn-homework/blob/ed9a6955b87b96913e4409e4b978bc22574571df/Module%201/Images/Image_Geo.JPG)

