Описание проекта
Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Вам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 
Постройте модель с предельно большим значением F1-меры. Чтобы сдать проект успешно, нужно довести метрику до 0.59. Проверьте F1-меру на тестовой выборке самостоятельно.\

Используемые модели
В ходе работы были испытаны 3 модели: решающее дерево, случайный лес, логистическая регрессия. В ходе анализа исходных данных был обнаружен дисбаланс классов, после чего были приняты следующие попытки это исправить: апсэмплинг, даунсэмплинг, понижение порога, сбалансирование вклассов (ЛР).

Результаты
Лучшие метрики показал метод случайного леса с использованием даунсэмплинга данных, его f1-метри составила 0.60.
Среди исследованных моделей рекомендую использовать случайный лес с следующими гиперпараметрами: n_estimators=110, max_depth=15, min_samples_leaf=1.

