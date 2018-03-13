# Тест для разработчика

Тест для разработчика в компанию BestPlace.

Нужно скачать этот файл, заполнить соответствующие поля и прислать модифицированный md-файл по почте.


### 1. Напишите, какие бывают типы http запросов (Request methods)? 

~~~
# Напишите тут типы запросов.

OPTIONS
GET
HEAD
POST
PUT
PATCH
DELETE
TRACE
CONNECT

~~~


Нужно заполнить таблицу действий над ресурсами согласно REST-подходу.

*Поставьте «галочки» в нужных ячейках*.

|      | A                                  | /books | /books/17 |
| ---- | ---------------------------------- | ------ | --------- |
| 1    | Получить коллекцию                 |    √   |           |
| 2    | Создать новую запись о книге       |        |       √    |
| 3    | Изменить отдельную запись о книге  |        |     √      |
| 4    | Удалить всю коллекцию книг         |     √   |           |
| 5    | Удалить отдельную запись о книге   |        |      √     |
| 6    | Получить запись об отдельной книге |        |     √      |



### 2. Разница между процессом и потоком

*Поставьте «галочки» в нужных ячейках*.

|      | Свойство                                                   | Процессы | Потоки |
| ---- | ---------------------------------------------------------- | -------- | ------ |
| 1    | Взаимодействуют только через механизмы, предоставляемые ОС |     √     |        |
| 2    | Делят между собой память                                   |          |    √    |
| 3    | Владеют ресурсами                                          |      √    |        |
| 4    | Хранят больше информации о состоянии                       |      √    |        |
| 5    | "Легче" происходит переключение контекста                  |          |    √    |
| 6    | Имеют отдельное адресное пространство                      |      √    |        |
| 7    | Могут создавать объекты такого же типа                     |          |     √   |
| 8    | Могут владеть объектами того же типа                       |      √    |        |



### 3. Медиана трех чисел

Нужно написать функцию, которая возвращает среднее по значению число из трех чисел.

Для [5, 1, 2] результат будет 2.

*Решать можно на python или js*

~~~javascript
// Сигнатура на js
function median3(a, b, c) {
    // Впишите код тут, если решаете на js
    return 0
}
~~~



~~~python
# Сигнатура на python
def median3(a, b, c):
    # Впишите код тут, если решаете на python
    return 0
~~~



### 4. В чем проблема этого кода? Как улучшить?

*Это js-вопрос. Для теста на бекенд этот вопрос можно пропустить*

~~~javascript
var done = false;

$.ajax(url, function() {
    done = true;
});

while (!done) {
    doSomething();
}
~~~


~~~js
// Опишите проблему и напишите код, который её исправляет

//Проблема в том что цикл будет занимать время ЦП ожидая тру,
//целесообразней передать в колбек то что требуется сделать в итоге
$.ajax(url, doSomthing())

~~~



### 5. Баблинг событий интерфейса

*Это js-вопрос. Для теста на бекенд этот вопрос можно пропустить*

https://javascript.ru/forum/events/30175-nepoluchaetsya-zapretit-perekhod-po-ssylke.html

Допустим, мы повесили обработчик на событие “click” гиперссылки. Что нужно дописать в обработчике, чтобы прекратить обработку события и предотвратить переход по этой ссылке?


~~~javascript
// Напишите код тут


~~~


### 6. Заполните таблицу сложности алгоритмов

*Поставьте «галочки» в нужных ячейках*.

|      | A                                                  | O(1) | O(ln(N)) | O(N) | O(N*ln(N)) | O(N^2) | Другой вариант |
| ---- | -------------------------------------------------- | ---- | -------- | ---- | ---------- | ------ | ------------ |
| 1    | Вставка в красно-черное дерево                     |      |          |      |            |        |              |
| 2    | Быстрая сортировка в среднем                       |      |          |      |            |        |              |
| 3    | Вставка в хеш-таблицу                              |      |          |      |            |        |              |
| 4    | Поиск в связном списке                             |      |          |      |            |        |              |
| 5    | Двоичный поиск в отсортированном массиве           |      |          |      |            |        |              |
| 6    | Обход красно-черного дерева от большего к меньшему |      |          |      |            |        |              |
| 7    | Вставка в хеш-таблицу в случае коллизии            |      |          |      |            |        |              |
| 8    | "Пузырьковая" сортировка                           |      |          |      |            |        |              |
| 9    | Удаление из массива (со сдвигом)                   |      |          |      |            |        |              |
| 10   | Поиск в хеш-таблице                                |      |          |      |            |        |              |


### 7. arr.push(a) эквивалентен

~~~javascript
// Закоментируйте неправильные варианты
arr[0] = a
arr[arr.length] = a
arr[arr.length - 1] = a
arr[-1] = a
~~~



### 8. Нужно отметить несколько верных утверждений о различных БД

*Поставьте «галочки» в нужных ячейках*.

|      | A                                                            | MongoDB | MySQL | Postgres |
| ---- | ------------------------------------------------------------ | ------- | ----- | -------- |
| 1    | Хранит документы                                             |         |       |          |
| 2    | Хранит строки данных                                         |         |       |          |
| 3    | Гарантирует атомарность изменения нескольких коллекций/таблиц |         |       |          |
| 4    | Позволяет эффективно сделать запрос к полю JSON              |         |       |          |
| 5    | Требует описания "схемы" данных, таблицы                     |         |       |          |
| 6    | Гарантирует атомарность на уровне документа/строки           |         |       |          |
| 7    | Удовлетворяет критериям ACID                                 |         |       |          |
| 8    | Поддерживает репликацию на несколько машин                   |         |       |          |


### 9. Что может происходить в браузере, когда пользователь вводит адрес (https://ya.ru) в адресной строке и нажимает Enter?

*Поставьте «галочки» в нужных ячейках*.

|      | A                                     |      |
| ---- | ------------------------------------- | ---- |
| 1    | Сжатие исходных JS кода               |      |
| 2    | Проверка сертификатов                 |      |
| 3    | Парсинг HTML                          |      |
| 4    | Запуск PHP скриптов сайта             |      |
| 5    | Исполнение Javascript                 |      |
| 6    | Парсинг CSS                           |      |
| 7    | Загрузка данных html страницы по HTTP |      |
| 8    | Деобфускация JS кода                  |      |
| 9    | TLS handshake                         |      |
| 10   | DNS запрос по UDP                     |      |
| 11   | Построение DOM-дерева                 |      |


### 10. В чем различие между протоколами TCP и UDP?

*Поставьте «галочки» в нужных ячейках*.

|      | A                                                    | TCP  | UDP  |
| ---- | ---------------------------------------------------- | ---- | ---- |
| 1    | Гарантирует доставку данных                          |      |      |
| 2    | Лучше подходит для задач условно "реального времени" |      |      |
| 3    | Требует установки соединения                         |      |      |
| 4    | Обеспечивает более высокую скорость передачи данных  |      |      |
| 5    | Работает внутри IP сетей                             |      |      |
| 6    | Гарантирует последовательность доставки              |      |      |


### 11. Задача "выколотый массив"

```arr``` - массив чисел от 1 до N, в котором одно число выкинули, а остальной массив перемешали. Требуется написать функцию, которая принимает на вход массив ```arr``` и возвращает удаленное число. Решение должно быть линейным, не должно модифицировать исходный массив и использовать дополнительную память.

*Решать можно на python или js*

```javascript
// Сигнатура на js
function findMissing(arr) {
    // Впишите код тут, если решаете на js
    return 0
}
```

```python
# Сигнатура на python
def find_missing(arr):
    # Впишите код тут, если решаете на python
    return 0
```
