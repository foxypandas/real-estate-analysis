# Real Estate Listing Analysis / Анализ объявлений о продаже недвижимости

## EN

This project explores a real estate listings dataset with a focus on apartment characteristics, pricing patterns, publication activity, and the factors that may influence apartment prices.

The analysis includes data preprocessing, exploratory data analysis, visualization, and interpretation of the main relationships between property features and listing prices. The repository contains both English and Russian notebook versions for portfolio presentation.

### Project Goal

The goal of the project is to analyze apartment listings and identify the factors associated with price formation, listing duration, and location-based differences.

The findings may support the future development of automated systems for detecting anomalous or potentially fraudulent listings.

### Project Structure

```text
real_estate_exploratory_analysis/
├── data/
│   └── real_estate_data.csv
├── images/
├── notebooks/
│   ├── real_estate_eda_ru.ipynb
│   └── real_estate_eda_en.ipynb
├── scripts/
├── .gitignore
└── README.md
```
### Notebooks

	•	real_estate_eda_ru.ipynb — full Russian version of the analysis
	•	real_estate_eda_en.ipynb — full English version of the analysis

### Dataset Description

The dataset contains information about apartment listings, including:
	•	listing price
	•	total area
	•	living area
	•	kitchen area
	•	number of rooms
	•	floor and total number of floors
	•	ceiling height
	•	distance to the city center
	•	proximity to airports, parks, and ponds
	•	publication date
	•	number of listing days

### Main Steps of the Analysis
	1.	Data loading and initial inspection
	2.	Data preprocessing and handling missing values
	3.	Type correction and feature engineering
	4.	Outlier detection and filtering
	5.	Exploratory data analysis
	6.	Analysis of relationships between price and apartment characteristics
	7.	Analysis of listing activity by weekday, month, and year
	8.	Summary of key findings

### Key Questions

The project aims to answer the following questions:
	•	What are the main characteristics of apartment listings in the dataset?
	•	Which factors are most strongly associated with price?
	•	How does price depend on total area, kitchen area, number of rooms, and floor type?
	•	How does location affect price per square meter?
	•	How long do listings typically remain active?
	•	Does the publication date appear to influence price?

### Main Findings
	•	Apartment price is positively associated with total area.
	•	Listings with a larger number of rooms tend to have higher average prices, although extreme values can distort this relationship.
	•	Kitchen area alone does not appear to be a decisive pricing factor.
	•	Floor type affects average price: first-floor apartments tend to be cheaper, while middle-floor apartments are generally more expensive.
	•	Price per square meter is influenced by location and tends to decline as distance from the city center increases.
	•	Most listings are concentrated in a limited range of common apartment characteristics.
	•	The weekday and month of publication appear to have limited explanatory power with respect to price.

### Visualizations

The project includes saved visualizations in the images/ folder, including:
	•	distributions of key numerical features
	•	correlation heatmap
	•	price distribution
	•	room count distribution
	•	ceiling height analysis
	•	days on market distribution
	•	price vs total area
	•	average price by number of rooms
	•	average price by floor type
	•	average price by weekday, month, and year
	•	price per square meter by location
	•	price per square meter vs distance to Saint Petersburg city center

### Tools and Libraries
	•	Python
	•	pandas
	•	matplotlib
	•	seaborn
	•	pathlib

### How to Run
	1.	Clone the repository
	2.	Open the project folder
	3.	Install the required libraries
	4.	Run the notebooks from the notebooks/ directory

### Future Improvements
	•	add a Polars-based version of the analysis
	•	compare pandas and Polars workflows
	•	extend the project with additional statistical analysis
	•	improve reproducibility and environment configuration

## Author

Olesya Lisitskaya

⸻

## RU

Этот проект посвящён анализу датасета с объявлениями о продаже недвижимости. Основное внимание уделено характеристикам квартир, ценовым закономерностям, активности публикации объявлений и факторам, которые могут влиять на стоимость объектов.

Анализ включает предобработку данных, исследовательский анализ, визуализацию и интерпретацию ключевых связей между характеристиками недвижимости и ценой. В репозитории представлены как английская, так и русская версии ноутбука для портфолио.

### Цель проекта

Цель проекта — проанализировать объявления о продаже квартир и выявить факторы, связанные с формированием цены, длительностью экспозиции и различиями между локациями.

Результаты анализа в дальнейшем могут быть полезны для разработки автоматизированных систем обнаружения аномальных или потенциально мошеннических объявлений.

### Структура проекта
```text
real_estate_exploratory_analysis/
├── data/
│   └── real_estate_data.csv
├── images/
├── notebooks/
│   ├── real_estate_eda_ru.ipynb
│   └── real_estate_eda_en.ipynb
├── scripts/
├── .gitignore
└── README.md
```

### Ноутбуки
	•	real_estate_eda_ru.ipynb — полная версия анализа на русском языке
	•	real_estate_eda_en.ipynb — полная версия анализа на английском языке

### Описание датасета

Датасет содержит информацию об объявлениях о продаже квартир, включая:
	•	цену объекта
	•	общую площадь
	•	жилую площадь
	•	площадь кухни
	•	количество комнат
	•	этаж и общее число этажей
	•	высоту потолков
	•	расстояние до центра города
	•	близость к аэропортам, паркам и водоёмам
	•	дату публикации
	•	длительность размещения объявления

### Основные этапы анализа
	1.	Загрузка данных и первичный осмотр
	2.	Предобработка данных и работа с пропусками
	3.	Корректировка типов данных и создание новых признаков
	4.	Поиск и фильтрация выбросов
	5.	Исследовательский анализ данных
	6.	Анализ связи цены с характеристиками квартиры
	7.	Анализ активности публикаций по дням недели, месяцам и годам
	8.	Формулировка основных выводов

### Ключевые вопросы

Проект отвечает на следующие вопросы:
	•	Каковы основные характеристики квартир, представленных в датасете?
	•	Какие факторы сильнее всего связаны с ценой?
	•	Как цена зависит от общей площади, площади кухни, количества комнат и типа этажа?
	•	Как локация влияет на цену за квадратный метр?
	•	Как долго объявления обычно остаются активными?
	•	Влияет ли дата публикации на цену?

### Основные выводы
	•	Цена квартиры положительно связана с общей площадью.
	•	Объекты с большим количеством комнат в среднем стоят дороже, хотя экстремальные значения могут искажать эту зависимость.
	•	Площадь кухни сама по себе не выглядит решающим фактором ценообразования.
	•	Тип этажа влияет на среднюю цену: квартиры на первом этаже обычно дешевле, а объекты на средних этажах — дороже.
	•	Цена за квадратный метр зависит от локации и, как правило, снижается по мере удаления от центра города.
	•	Большая часть объявлений сосредоточена в диапазоне типичных характеристик жилья.
	•	День недели и месяц публикации, по-видимому, слабо объясняют различия в цене.

### Визуализации

Проект содержит сохранённые визуализации в папке images/, включая:
	•	распределения ключевых числовых признаков
	•	тепловую карту корреляций
	•	распределение цен
	•	распределение по количеству комнат
	•	анализ высоты потолков
	•	распределение длительности размещения объявления
	•	зависимость цены от общей площади
	•	среднюю цену по числу комнат
	•	среднюю цену по типу этажа
	•	среднюю цену по дням недели, месяцам и годам
	•	цену за квадратный метр по населённым пунктам
	•	зависимость цены за квадратный метр от расстояния до центра Санкт-Петербурга

### Инструменты и библиотеки
	•	Python
	•	pandas
	•	matplotlib
	•	seaborn
	•	pathlib

### Как запустить
	1.	Клонировать репозиторий
	2.	Открыть папку проекта
	3.	Установить необходимые библиотеки
	4.	Запустить ноутбуки из папки notebooks/

### Возможные улучшения
	•	добавить версию анализа на Polars
	•	сравнить пайплайны на pandas и Polars
	•	расширить проект дополнительным статистическим анализом
	•	улучшить воспроизводимость и настройку окружения

## Автор

Олеся Лисицкая
