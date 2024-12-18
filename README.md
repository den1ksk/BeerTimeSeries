# BeerTimeSeries

## Описание проекта

Этот проект посвящен прогнозированию продаж пива с использованием методов машинного обучения и анализа временных рядов. В качестве данных используется датасет, основанный на Dominick's dataset, который содержит информацию о продажах пива, а также демографические данные.

## Цель проекта

Основная цель проекта - построить модель, способную точно прогнозировать спрос на пиво на основе исторических данных. Это позволит оптимизировать запасы, планировать маркетинговые кампании и принимать более обоснованные бизнес-решения.

## Используемые библиотеки и инструменты

*   **Python**
*   **pandas**
*   **numpy** 
*   **matplotlib** 
*   **seaborn** 
*   **xgboost** 
*   **statsmodels** 
*   **torch** 
*   **sklearn** 
*   **autogluon** 

## Структура проекта
```
├── beer_sales_data.parquet - Файл с данными о продажах пива.
├── beer_upc.parquet - Файл с описанием товаров пива.
├── demographic_data.parquet - Файл с демографическими данными магазинов
└── automacon.ipynb - Jupyter Notebook с кодом проекта
```

## Результаты
Использованы три различных подхода к прогнозированию:

1. **XGBoost**
   - Точность: R² = 0.9967
   - Средняя абсолютная ошибка (MAE): 117.36
   - Среднеквадратичная ошибка (RMSE): 167.07

2. **AutoGluon**
   - Точность: R² = 0.9958
   - Средняя абсолютная ошибка (MAE): 133.13
   - Среднеквадратичная ошибка (RMSE): 187.54

3. **LSTNet (Neural Network)**
   - Точность: R² = 0.9356
   - Средняя абсолютная ошибка (MAE): 0.071
   - Среднеквадратичная ошибка (RMSE): 0.169
