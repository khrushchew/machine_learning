### UniMachineLearning
README.md
markdown
Копировать
Редактировать
# Лабораторная работа №1: Классификация  
**Дисциплина:** Машинное обучение  
**Тема:** Классификация  

## Описание  
В данной лабораторной работе проводится анализ и сравнение эффективности трех алгоритмов классификации:  
- Метод K ближайших соседей (k-Nearest Neighbors, KNN)  
- Метод опорных векторов (Support Vector Machine, SVM)  
- Модель случайного леса (Random Forest)  

Работа включает в себя следующие этапы:  
1. **Теоретическое введение** — описание используемых алгоритмов.  
2. **Предобработка данных** — заполнение пропусков, удаление ненужных переменных, стандартизация и кодирование категориальных данных.  
3. **Обучение и тестирование моделей** — настройка гиперпараметров, обучение моделей и их оценка на тестовых данных.  
4. **Анализ результатов** — визуализация ROC-AUC кривых, оценка метрик качества и важности признаков.

## Используемые технологии  
- Python  
- Библиотеки:  
  - `sklearn` (KNeighborsClassifier, SVC, RandomForestClassifier, RandomizedSearchCV, GridSearchCV)  
  - `pandas` и `numpy` для работы с данными  
  - `matplotlib` и `seaborn` для визуализации  

## Предобработка данных  
Перед обучением моделей выполняется:  
- Заполнение пропусков.  
- Удаление выбросов с использованием диаграмм рассеяния и ящиков с усами.  
- Кодирование категориальных переменных с помощью `OneHotEncoding`.  
- Стандартизация числовых данных с использованием `SimpleScaler`.  

## Модели и результаты  
### KNN (Метод K ближайших соседей)  
- Настройка гиперпараметров через `RandomizedSearchCV`.  
- Оценка по метрикам: Precision, Recall, F1-score, ROC-AUC.  
- Визуализация ROC-AUC кривых для тестовой и валидационной выборок.  

### SVM (Метод опорных векторов)  
- Подбор гиперпараметров с использованием `GridSearchCV`.  
- Построение ROC-AUC кривых и анализ производительности.  

### Random Forest (Случайный лес)  
- Настройка гиперпараметров через `RandomizedSearchCV`.  
- Построение графика feature importance.  

## Визуализация  
Для каждого этапа анализа представлены:  
- Гистограммы, матрицы корреляций и диаграммы рассеяния для исследования данных.  
- ROC-AUC кривые для оценки моделей.  
- График важности признаков (`Feature Importance`) для модели случайного леса.  

## Выводы  
Проведён сравнительный анализ эффективности алгоритмов классификации на одном наборе данных.  
- **Все модели продемонстрировали высокую точность и стабильные значения метрик качества.**  
- Наибольшую точность классификации показала модель случайного леса, что подтверждается её высокой метрикой ROC-AUC и визуализацией важности признаков.  

## Запуск  
1. Установите необходимые библиотеки:  
   ```bash
   pip install -r requirements.txt
Запустите Jupyter Notebook или Python-скрипт с реализацией анализа.
Файлы проекта
data/ — Папка с набором данных.
notebooks/ — Jupyter Notebook с кодом выполнения лабораторной работы.
results/ — Графики и отчёты о выполнении работы.
Авторы
Студент: Попов Н.А.
Преподаватель: Турсуков Н.О.
Университет: СПбГЭТУ «ЛЭТИ», кафедра Вычислительной техники.
