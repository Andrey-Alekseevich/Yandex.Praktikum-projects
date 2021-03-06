# Отток клиентов банка.
На основе исторических данных о поведении клиентов банка необходимо спрогнозировать значение целевого признака - уйдёт клиент из банка в ближайшее время или нет.

## Задача
Основная задача - найти и построить модель с предельно большим значением F1-меры. Выбранную нужно довести метрику до 0.59.
Дополнительно измерим AUC-ROC, сравнивним её значение с F1-мерой.

## Данные
Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

**Признаки**
 - RowNumber — индекс строки в данных
 - CustomerId — уникальный идентификатор клиента
 - Surname — фамилия
 - CreditScore — кредитный рейтинг
 - Geography — страна проживания
 - Gender — пол
 - Age — возраст
 - Tenure — количество недвижимости у клиента
 - Balance — баланс на счёте
 - NumOfProducts — количество продуктов банка, используемых клиентом
 - HasCrCard — наличие кредитной карты
 - IsActiveMember — активность клиента
 - EstimatedSalary — предполагаемая зарплата
 
**Целевой признак**
 - Exited — факт ухода клиента

## Используемые библиотеки
Библиотеки: *pandas, numpy, matplotlib, sklearn, catboost*

## Ключевые методы работы

#### Обучение с учителем (Reinforcement Learning). 
 - градиентный бустинг
 - random forest
 - logistic regression

#### Работа с несбалансированными данными, методы устранения дисбаланса.
 - upsample 
 - donwsample
 
#### Parameter tuning and cross validation.