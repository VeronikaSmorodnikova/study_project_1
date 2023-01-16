# study_project_1 

**Используемые библиотеки python:** pandas, scipy , numpy, pingouin, statsmodels, datetime, matplotlib.pyplot, seaborn.  

**Цели:** 
1. Проверить, был ли успешным эксперимент, в ходе которого была изменена стоимость премиум-подписки для новых пользователей.
2. Проверить, имеет ли изменение стоимости подписки смысл среди определенных групп пользователей.

**Полученные результаты:**
1. Эксперимент не был успешен, т.к. после изменения стоимости премиум подписки ARPU статистически значимо не изменился.

2. Увеличение стоимости премиум подписки не вызвало уменьшение частоты ее оформления, однако retention имеет довольно низкие значения в обоих группах.
Большая часть пользователей оплачивали подписку 1 раз, а поскольку оплата подписки происходит ежемесячно, можно сделать вывод, что наши пользователи не очень заинтересованы в продлении подписки.

3. О неуспешности эксперимента также свидетельствуют различия в конверсии в оформление подписки между группами. В контрольной группе значение конверсии больше. Соотношение пользователей, сконвертировавшихся в целевое действие, значимо отличается в группах. Можно сделать вывод, что увеличение стоимости премиум подписки привело к уменьшению конверсии, и за счет этого ARPU в группах значимо не различается.

4. При сравнении групп значимое влияние на размер дохода total revenue от пользователя показал только фактор количества визитов. Что может объясняться простой логикой - чем чаще пользователь посещает приложение, тем больше он, скорее всего, платит за различные продукты. Значимых различий в доходе total revenue между пользователями из разных стран и разных возрастов не наблюдается.

5. Наличие премиум подписки, как правило, зависит от того, была ли у пользователя подписка ранее, и того, как часто пользователь посещает приложение, при этом возраст не оказывает значимого влияния на соотношение пользователей с премиум подпиской и без нее.

**Проект содержит:**
1. Деление пользователей на социально-демографические группы;
2. Анализ частоты входа в приложение и conversion window до момента оплаты подписки;
3. Поиск ошибок в данных, дубликатов, выбросов, подозрительных записей;
4. Анализ среднего дохода с пользователя ARPU и среднего дохода с платящего пользователя ARPPU (в тестовой и контрольной группах);
5. А/А тест для проверки качества системы сплитования трафика;
6. А/В тест (t-test, bootstrap, множественный ANOVA, Хи-квадрат, проверка на нормальность распределения и гомогенность дисперсии);
7. Визуализация данных.
