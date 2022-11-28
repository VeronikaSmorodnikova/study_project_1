# study_project_1
Dating app data analyse (EDA, A/B testing, statistics)

В проекте представлен анализ A/B теста, который был проведен в дэйтинговом приложении. В ходе эксперимента была изменена стоимость премиум-подписки для новых пользователей. Стоимость пробного периода подписки не изменялась. В проекте проверялось, был ли эксперимент успешным и имеет ли он смысл среди определенных групп пользователей.

## Проект содержит:  
1. Деление пользователей на социально-демографические группы;
2. Анализ частоты входа в приложение и периода между регистрацией и оплатой подписки;
3. Поиск ошибок в данных, дубликатов, выбросов, подозрительных записей;
4. Анализ распределения дохода с пользователя в группах (тестовой и контрольных);
5. А/А тест для проверки качества системы сплитования трафика;
6. А/В тест (t-test, ANOVA, множественный ANOVA, Хи-квадрат, проверка на нормальность распределения и гомогенность дисперсии);
7. Визуализация данных.

Статистический анализ был проведен с помощью библиотек scipy.stats, pingouin, statsmodels, numpy.
Визуализация - seaborn, matplotlib.


## Описание данных  
Всего есть три группы: тестовая (test), контрольная 1 (control_1) и контрольная 2 (control_2). Для каждой из них:

**users_*.csv – информация о пользователях:**  

uid – идентификатор пользователя  
age – возраст  
attraction_coeff – коэффициент привлекательности (от 0 до 1000)  
coins – число монеток (внутренняя валюта)  
country – страна    
visit_days – в какие дни после регистрации пользователь посещал приложение (напр. в 1, затем в 7)  
gender – пол  
age_filter_start  – фильтр поиска, мин. значение   
age_filter_end  – фильтр поиска, макс. значение   
views_count – число полученных оценок   
was_premium – был ли когда-либо премиум (либо пробный период премиум-статуса, либо купленный за деньги)  
is_premium –  является ли премиум  
total_revenue – нормированная выручка   
 
**transactions_*.csv – информация о платежах пользователей:**  

uid – идентификатор пользователя  
country – страна  
joined_at – дата и время регистрации  
paid_at – дата и время покупки  
revenue – нормированная выручка  
payment_id – идентификатор платежа  
from_page – откуда пользователь перешел на страницу оплаты  
product_type – тип продукта (trial_premium – пробная премиум-подписка, premium_no_trial – премиум-подписка без пробной, coins – подписка за внутреннюю валюту, other_type – другое)  
 
**Файлы:**  

users_test – информация о пользователях в тестовой группе.    
users_control_1 – информация о пользователях в первой контрольной группе.   
users_control_2 – информация о пользователях во второй контрольной группе .   
transactions_test – информация о платежах пользователей в тестовой группе.   
transactions_control_1 – информация о платежах пользователей в первой контрольной группе.   
transactions_control_2 – информация о платежах пользователей во второй контрольной группе.   
