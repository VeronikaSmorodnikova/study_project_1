# study_project_1
Dating app data analyse (EDA, A/B testing, statistics)

В проекте представлен анализ A/B теста, который был проведен в дэйтинговом приложении. В ходе эксперимента была изменена стоимость премиум-подписки для новых пользователей. Стоимость пробного периода подписки не изменялась. В проекте проверялось, был ли эксперимент успешным и имеет ли он смысл среди определенных групп пользователей.

Проект содержит:
1. Деление пользователей на социально-демографические группы;
2. Анализ частоты входа в приложение и периода между регистрацией и оплатой подписки;
3. Поиск ошибок в данных, дубликатов, выбросов, подозрительных записей;
4. Анализ распределения дохода с пользователя в группах (тестовой и контрольных);
5. А/А тест для проверки качества системы сплитования трафика;
6. А/В тест (t-test, ANOVA, множественный ANOVA, Хи-квадрат, проверка на нормальность распределения и гомогенность дисперсии);
7. Визуализация данных.

Статистический анализ был проведен с помощью библиотек scipy.stats, pingouin, statsmodels, numpy.
Визуализация - seaborn, matplotlib.
