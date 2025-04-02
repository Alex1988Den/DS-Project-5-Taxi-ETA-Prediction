# Проект по предсказанию длительности поездки на такси в Нью-Йорке

## Описание
Этот проект включает в себя создание модели машинного обучения для предсказания длительности поездки на такси в Нью-Йорке. Мы используем несколько методов, включая **линейную регрессию**, **деревья решений**, **случайный лес**, **градиентный бустинг** и **полиномиальные регрессии**, чтобы выбрать лучший подход для данной задачи.

Основная цель проекта — предсказать длительность поездки на такси с помощью анализа данных о поездках в Нью-Йорке. Мы применяем различные методы, включая обработку данных, анализ признаков, выбор гиперпараметров и оценку моделей на основе метрик, таких как **RMSLE** (Root Mean Squared Logarithmic Error) и **MeAE** (Median Absolute Error).

## Структура данных
Данные для обучения моделей включают:
- **Длительность поездки** (в секундах)
- **Координаты начала и конца поездки**
- **Количество пассажиров**
- **Время суток и день недели**
- **Метеорологические данные** (температура, видимость, осадки и т.д.)

## Данные
- Для проекта используются два набора данных:
  1. [**Набор данных о поездках на такси в Нью-Йорке**](https://drive.google.com/file/d/1ecWjor7Tn3HP7LEAm5a0B_wrIfdcVGwR/view) — данные о такси, включая координаты, время и другие параметры.
  2. [**Набор данных о погодных условиях в Нью-Йорке**](https://drive.google.com/file/d/1X_EJEfERiXki0SKtbnCL9JDv49Go14lF/view) — метеорологическая информация для улучшения точности предсказаний.

## Метрики
Модели оцениваются с использованием следующих метрик:
- **RMSLE**: корень из среднеквадратичной ошибки логарифмов, используется для оценки точности предсказаний.
- **MeAE**: медианная абсолютная ошибка, которая позволяет измерить точность модели на валидационной выборке.

## Модели
В проекте использованы следующие модели:
- **Линейная регрессия**
- **Полиномиальная регрессия (2-ой степени)**
- **Дерево решений**
- **Случайный лес**
- **Градиентный бустинг (Gradient Boosting)**

Каждая модель была протестирована на обучающих и валидационных выборках, с целью достижения минимального значения **RMSLE** и **MeAE**.

## Установка и использование
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/username/Taxi-Trip-Duration-Prediction.git
   cd Taxi-Trip-Duration-Prediction

    Установите зависимости:

pip install -r requirements.txt

Запустите Jupyter Notebook или выполните скрипты:

    jupyter notebook

Примечания

    Для ускорения обучения моделей был использован GPU в случае с XGBoost и LightGBM.

    Для каждой модели проводился тщательный отбор гиперпараметров, что позволило добиться оптимальных результатов.

    Важно, что в данном проекте используется логарифмированная версия целевой переменной, что улучшает стабильность модели при предсказаниях с большими значениями.

Контакты

Для вопросов или предложений, пожалуйста, свяжитесь со мной по [aleksandr.denissov@brave.ee].


### Пояснение:
- **Описание**: Включает описание цели проекта, используемых данных и подходов.
- **Данные**: Ссылки на файлы, которые используются в проекте.
- **Метрики**: Описание метрик для оценки моделей.
- **Модели**: Перечисление использованных моделей.
- **Установка и использование**: Инструкции по запуску проекта.
- **Контакты**: Секция для связи с вами или вашими коллегами.
