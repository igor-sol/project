Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

Необходимо построить модель с предельно большим значением F1-меры. Дополнительно измерить AUC-ROC и сравнить ее значение с F1-мерой.

На подготовленном датасете с применением метода upsampling и downsampling были обучены модели случайного леса и решающего дерева с различными гиперпараметрами.

На валидационной выборке по значениям метрик была выбрана лучшая модель - случайный лес с гиперпараметрами n_estimators=135, max_depth=8.

Была проведена проверка модели на адеватность. Метрики исходной модели значительно выше. Модель адекватна. 

На тестовой выборке метрика F1 выбранной модели 0.607. AUC_ROC составляет 0.852.