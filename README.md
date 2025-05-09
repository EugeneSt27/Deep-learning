**Лабораторная работа 1: Классификация изображений с использованием CNN, предобработка и аугментация на различных датасетах, анализ метрик**   


**Раздел 1. Подготовка данных и работа с несколькими датасетами**      

Для глубокого понимания устойчивости модели и способности к обобщению полезно использовать несколько датасетов с разными характеристиками, такими как:
• CIFAR-10: Небольшие цветные изображения с разнообразными классами (животные, объекты).  
• Fashion-MNIST: Черно-белые изображения одежды, подходящие для классификации текстур и форм.  
• SVHN: Цветные изображения цифр из уличных знаков, что помогает оценить устойчивость модели к вариативности и сложным фонам.  

**Раздел 2. Сравнение предобработки для разных типов данных**    

**Раздел 3. Создание и оптимизация архитектуры CNN (CIFAR)**    

  1. Количество и размер сверточных фильтров
    - Использование меньшего количества фильтров (16 и 32) с ядрами 3x3 и 5x5   
    - Увеличение числа фильтров (64 и 128) для более сложных признаков   
    - Слой с фильтром 7x7 и 256 каналами   


  2. Пулинг (Pooling) слои   
    - Max Pooling с размером 2x2, stride 2   
    - Max Pooling с большим размером ядра (3x3) для более сильного снижения размерности   
    - Average Pooling для сглаживания признаков   


  3. Batch Normalization
    - Batch Normalization после каждого сверточного слоя   
    - Batch Normalization только в начале и конце сети   


  4. Dropout   
    - Умеренный Dropout (0.2)  
    - Сильный Dropout (0.5)   
    - Комбинация разных значений Dropout в одном слое  

 
  5. Полносвязные слои   
    - Полносвязный слой с малым количеством нейронов   
    - Последовательное применение нескольких полносвязных слоев (по сути, базовый класс SimpleCNN)   

**Раздел 4: Анализ гиперпараметров и оптимизация с использованием нестандартных методов (CIFAR)**

  1. Learning rate   
    - Использование Cyclic Learning Rate  


  2. Batch size   
    - Динамическое изменение Batch Size   
    - Gradient Accumulation  

  3. Количество фильтров и слоев    
    - Progressive Layer Growth   
    - Random Filter Pruning  


**Раздел 5: Анализ различных метрик производительности (CIFAR)**
