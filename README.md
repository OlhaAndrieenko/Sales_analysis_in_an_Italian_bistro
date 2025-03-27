# Аналіз продажів в італійському бістро за 2024 рік.

Представлений набір даних містить дані про продажі в італійському бістро, надаючи детальну інформацію про ефективність меню, тенденції доходів і вподобання клієнтів протягом року (2024). Набір даних відображає реальну роботи ресторану та дозволяє аналізувати сезонні тенденції, періоди пікових продажів і поведінку клієнтів. Мета цього аналізу - покращення стратегії продажів, враховуючи наведені вище фактори.

## Профіль колонок набору даних:
| Назва стовпця          | Опис                     
|---------------|-------------------------|
| Date           | Дата замовлення       | 
| Time           | Час замовлення        |
| Menu Item      | Пункт меню, назва страви |
| Category (Appetizer, Main Course,  Dessert)       | Категорія страви (Закуски, Основні страви, Десерти)      |
| Quantity*      | Кількість страв в замовленні   
| Price (per item) | Вартість однієї страви         | 
| Revenue     | Дохід від замовлення            
| Payment (Method Credit Card, Cash, Mobile Payment)| Спосіб оплати (Кредитна картка, Готівка, Мобільний платіж) |
| Customer (Type Dine-In, Takeaway, Delivery)| Тип клієнта (Обіди в закладі, На винос, Доставка)   |
 
Цей набір даних включає такі ключові змінні, як пункти меню, категорії (закуски, основні страви, десерти), обсяги продажів, ціни, дохід, способи оплати (кредитна картка, готівка, мобільний платіж) і типи клієнтів (обіди, на винос, доставка), що дозволять виконати аналіз діяльності бістро, виявити можливості для розвитку.

Датасет взято за посиланням: https://www.kaggle.com/datasets/divyanshisen/italian-bistro-sales-data-a-year-in-numbers

Формат даних xlsx.

## Використані аналітичні методи та інструменти
Цей проект використовує різні методи аналізу даних , щоб відповісти на ключові питання, пов’язані з роботою бістро.

### Інструменти:
- Бібліотеки Python:
  - numpy, pandas: маніпулювання та аналіз даних.
  - matplotlib, seaborn: візуалізація даних.
- scipy: статистичні тести (тест хі-квадрат, p-value).
- Tableau - візуалізація результатів аналізу.

## Питання включені до аналізу:
 1. Який загальний дохід бістро за рік і як він змінювався щомісяця?
 2. Які страви є популярнішими в залежності від сезону?
 3. Яка категорія страв є найпопулярнішою та приносить найбільший дохід?
 4. Яка страва приносить найбільший дохід і чи є вона найпопулярнішою серед страв меню?
 5. Який розроділ клієнтів за їх типом? Як розподіляються замовлення та дохід за типом клієнтів?
 6. Які способи оплати найбільше використовуються клієнтами?
 7. Чи є зв'язок між типом клієнта та способом оплати?
 8. Як розподіляються замовлення в залежності від типу клієнтів за часом доби?
 9. Як змінювався дохід в залежності від часу доби?
 10. Кореляція між кількістю замовлень та доходом.

 ## Висновки до проведеного аналізу продажів італійського бістро за 2024 рік.
 1. Річний дохід склав 247730,5. Найвищим дохід був в серпні (22827,5), найнижчим в лютому (19113,0) та червні (19110,5).
 2. Найпопулярнішими стравами в залежності від сезону є:
     - зима - Spaghetti Carbonara;
     - весна - Fettuccine Alfredo;
     - літо - Fettuccine Alfredo і Panna Cotta;
     - осінь - Tiramisu.
 3. Найпопулярнішою категорією страв є основні страви (найвищий рівень замовлень та доходу). Десерти займають 2-ге місце за популярність, але приносять менший дохід, ніж закуски, які є найменш популярною категорією страв.
 4. Найдохіднішою є страва Fettuccine Alfredo, найпопулярнішою за кількістю замовлень є страва Tiramisu.
 5. Кількість клієнтів за типом (Dine-In, Takeaway, Delivery) суттєво не відрізняється між собою. Але все ж таки лідерами є клієнти Takeaway.
 6. Найчастіше розраховувались готівкою, найрідше кредитною картою. Але, слід зауважити, що розбіжності в показниках не великі.
 7. Під час аналізу виявлено відсутність статистично значущого зв’язку між способом оплати та типом клієнта.
 8. Різниця між типами клієнтів в залежності від часу доби показує, що замовлення Takeaway мають сплески у певні години, тоді як замовлення Dine-In, Delivery більш рівномірно розподілені.
 9. Дохід від замовлень має пікові значення у періоди часу з 11:00 по 16:00, з 20:00 по 23:00.
 10. Між кількістю замовлень та доходом існує сильний позитивний зв'язок – чим більше страв у замовлення, то вищий дохід.

  ## Рекомендації для покращення роботи бістро:
 - запроваджувати сезонні акції в періоди низького попиту (лютий, червень) для збільшення доходу;
 - розвивати меню основних страв, оскільки вони найпопулярніші та найбільш прибуткові.
 - приділити більше уваги закускам, які приносять дохід більший за десерти, але менш популярні.
 - популяризувати безготівкові методи оплати для швидшого обслуговування клієнтів.
 - збільшити рекламу та промоакції вранці для стимулювання ранкових замовлень.

