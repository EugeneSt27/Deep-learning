# Лабораторная работа 2. LLM и Трансформер   

## Список задач:   
### 1. Введение и подготовка данных:
- Подготовить текстовый корпус для обучения модели.   
- Разделить данные на тренировочный, валидационный и тестовый наборы.   
- Очистить данные с применением методов, таких как удаление пунктуации, стоп-слов, и лемматизация.   
- Преобразовать текст в числовое представление через токенизацию.   
### 2. Изучение архитектуры трансформера:
- Разобраться в основных компонентах трансформера:
  - Self-Attention.
  - Multi-Head Attention.
  - Feed-Forward Network.
- Изучить механизмы позиционного кодирования и остаточных связей.
- Описать ключевые преимущества трансформера по сравнению с RNN и LSTM.
### 3. Создание модели на основе трансформера:   
- Инициализировать трансформер (например, GPT, BERT) и подготовить его для fine-tuning.
- Настроить гиперпараметры модели, такие как количество слоев, размерность векторного представления, число эпох и скорость обучения.
### 4. Обучение модели:
- Провести обучение трансформера на подготовленных данных.
- Применить различные оптимизаторы (Adam, SGD, RMSProp) и исследовать их влияние на процесс обучения.
- Использовать learning rate scheduler для управления скоростью обучения.
### 5. Оценка модели:
- Измерить производительность модели с использованием метрик:
- Perplexity для оценки уверенности модели.
- BLEU и ROUGE для оценки качества генерации текста.
- Сравнить результаты при использовании разных оптимизаторов и scheduler'ов.
### 6. Интерактивное тестирование модели:
- Разработать интерфейс для взаимодействия с моделью.
- Реализовать чат-бота, способного отвечать на запросы пользователей.
- Настроить параметры генерации (например, max_length, top_k, top_p) и проанализировать их влияние на ответы модели.
### 7. Анализ результатов:
- Провести эксперименты с различными гиперпараметрами и методами обучения.
- Построить графики зависимости потерь и Perplexity от числа эпох.
- Провести ручную оценку сгенерированных ответов на смысловую релевантность.