### JavaScript

`Ulashni 2 hili bor`

1. ```

   <!DOCTYPE html>
   <html lang="en">
   <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Document</title>
   </head>
   <body>

   </body>
   <script scr="./script.js"></script>
   </html>
   ```

2. ```


   <!DOCTYPE html>
   <html lang="en">
   <head>
   <meta charset="UTF-8">
   <meta name="viewport"            content="width=device-width, initial-scale=1.0">
   <title>Document</title>
   </head>
   <body>

   </body>


   <script>



   </script>
   </html>
   ```

### Containerlar

var , let , const

1. var - ohirigi berilgan o'zgaruvchini oladi va berilgan o'zgaruvchilarni ozgartirsa boladi

   ```
   var , let name = (111);
   name = 222;
   ```

2. const - har doim bir hil qoladigan o'zgaruvchi

   ```
   const a = (123);
   ```

### Document yoki consolga chiqarish ushun kodlar

alert , promt , confirm , console.log

    1. alert - text terish uchun hudud
    2. promt - bajarilgan alertdan kein chiqadigan hudud
    3. confirm - rozilik berishni soraydi
    4. console.log - consolga chiqarish uchun kod

# Различия между var, let и const в JavaScript

В JavaScript существует несколько способов объявления переменных: `var`, `let`, и `const`. Вот их основные различия:

## var

`var` был первым способом объявления переменных в JavaScript. Он имеет глобальную или функциональную область видимости, что может привести к нежелательным эффектам, таким как поднятие переменных (hoisting). Пример:

```javascript
console.log(x);
var x = 10;
console.log(x);
```

## let

let был добавлен в стандарт ECMAScript 6 (ES6). Он имеет блочную область видимости, что делает его более предсказуемым и безопасным для использования. Пример:

```javascript
console.log(x);
let x = 10;
console.log(x);
```

## const

const также был добавлен в стандарт ECMAScript 6 (ES6). Он также имеет блочную область видимости, но, в отличие от let, значение переменной const не может быть изменено после инициализации. Пример:

```JavaScript
const x = 10;
x = 20; //error

```

# Loops in JavaScript

JavaScript предоставляет несколько типов циклов для перебора коллекций данных или многократного выполнения кода. Три основных типа циклов: for, while и do- while. Каждый тип цикла имеет свой собственный синтаксис и варианты использования.

## for loop

Цикл for обычно используется, когда количество итераций известно до входа в цикл.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

## while loop

Цикл while используется, когда количество итераций заранее неизвестно, но цикл должен продолжаться до тех пор, пока заданное условие истинно.

```JavaScript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

## do-while loop

Цикл do- while аналогичен циклу while, но условие оценивается после тела цикла. Это означает, что цикл всегда будет выполняться хотя бы один раз.

```JavaScript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);

```

### function

##### 1 .

В JavaScript функция — это именованный блок кода, который выполняет части программы. Функция может содержаться и использоваться из других разделов кода, вызывая ее. Функциями JavaScript легко и просто манипулировать, и их можно часто использовать на практике.

Способ создания функции следующий:

```JavaScript
function funksiyaNomi(parametr1, parametr2, ...) {
  // Funksiya ichidagi kodlar
  // Agar parametrlar bo'lsa, ularni ishlatish mumkin
  return chiqishQiymati; // Agar kerak bo'lsa
}
```

Здесь:

- «functionName»: имя функции, используемое при вызове функции.
- «параметр1», «параметр2», ...: аргументы, передаваемые функции. Здесь переменные (параметры) заменяют данные, передаваемые в функцию.
- { // Коды внутри функции }: Функциональный блок объединяет выполнение внутри функции.
- «return exitValue;»: значение, возвращаемое после выполнения функции. Вместо этой части функция возвращает что-то, используя следующий оператор return.

##### 2.

Способ вызова функции следующий:

```JavaScript
var natija = funksiyaNomi(argument1, argument2, ...);
```

— Здесь переменная «result» хранит возвращаемое значение после выполнения функции.

Пример:

```JavaScript
function salom(name) {
  var salomMatn = "Salom, " + name + "!";
  return salomMatn;
}

var salomXabari = salom("Doston");
console.log(salomXabari);
```

Этот код использует функцию hello и передает ей значение модификатора вместо аргумента Epic. В результате вывода «Salom , Doston!» текст выводится на консоль.

# DOM Element

### 1. Прием элементов:

- getElementById(id) - elementni identifikatori bo'yicha oladi
- getElementsByClassName(className) - ma'lum bir sinfga ega barcha elementlarni oladi
- getElementsByTagName(tagName) - ma'lum bir teg bilan barcha elementlarni oladi
- querySelector(selektor) - berilgan CSS selektoriga mos keladigan birinchi elementni oladi

### 2. Изменить содержимое:

- innerHTML - elementning HTML tarkibini o'zgartiradi
- textContent - elementning matn tarkibini o'zgartiradi

### 3. Управление атрибутами:

- getAttribute(name) - atribut qiymatini oladi
- setAttribute(nom, qiymat) - atribut qiymatini o'rnatadi

### 4. Создайте новые элементы:

- createElement(tagName) - yangi HTML elementini yaratadi
- createTextNode(text) - yangi matn tugunini yaratadi

### 5. Управление стилями и классами:

- style.property = qiymat; // element uslubini o'zgartiradi
- classList.add(className), classList.remove(className), classList.toggle(className)

# DOM API в JavaScript

DOM (Document Object Model) - это структура объектов, представляющая содержимое веб-страницы, которая позволяет JavaScript взаимодействовать с HTML и CSS для изменения содержимого, структуры и стилей страницы.

## Основные концепции

### Узлы DOM

Узлы DOM представляют собой отдельные элементы HTML, такие как теги, атрибуты и текстовые узлы. Каждый элемент в дереве DOM является узлом.

### Элементы

Элементы DOM представляют собой объекты, представляющие HTML-теги. Они предоставляют доступ к атрибутам, стилям и содержимому элемента.

### Узлы текста

Узлы текста представляют собой содержимое текста в HTML-элементах.

### DOM API

DOM API - это интерфейс JavaScript для работы с узлами и элементами DOM. Он включает в себя методы для создания, удаления, изменения и доступа к узлам и элементам.

## Основные операции с DOM

### Получение элементов

JavaScript позволяет получать доступ к элементам DOM с помощью методов `getElementById`, `getElementsByClassName`, `getElementsByTagName`, `querySelector` и `querySelectorAll`.

### Изменение содержимого

С помощью JavaScript можно изменять содержимое элементов DOM, используя свойства `innerHTML` и `textContent`, а также методы `appendChild`, `removeChild`, `createElement`, `createTextNode` и другие.

### Изменение стилей

JavaScript позволяет изменять стили элементов DOM, используя свойство `style`.

### Обработка событий

JavaScript позволяет добавлять обработчики событий к элементам DOM с помощью методов `addEventListener`, `removeEventListener` и других.

## Пример использования DOM API

```javascript
// Получаем элемент по id
const element = document.getElementById("myElement");

// Изменяем текст элемента
element.textContent = "Новый текст";

// Изменяем стиль элемента
element.style.color = "red";

// Добавляем обработчик события
element.addEventListener("click", function () {
  alert("Элемент был кликнут");
});
```


# LocalStorage в JavaScript

LocalStorage - это механизм, предоставляемый веб-браузерами, для хранения данных в виде пар ключ-значение. Данные, сохраненные в LocalStorage, остаются доступными даже после закрытия вкладки или перезапуска браузера. Это делает LocalStorage полезным для сохранения состояния приложений и других важных данных на стороне клиента.

## Использование LocalStorage

### Установка значения

Для сохранения значения в LocalStorage используется метод `setItem(key, value)`. Например:

```javascript
localStorage.setItem('username', 'John');
```

## Получение значения
Чтобы получить сохраненное значение из LocalStorage, используется метод getItem(key). Например:

```JavaScript
let username = localStorage.getItem('username');
console.log(username); // Выведет "John"
```

## Удаление значения
Для удаления значения из LocalStorage используется метод removeItem(key). Например:

```JavaScript
localStorage.removeItem('username');
```

## Очистка LocalStorage
Для удаления всех данных из LocalStorage можно использовать метод clear(). Например:

```
localStorage.clear();
```

## Ограничения LocalStorage
Хотя LocalStorage предоставляет удобный способ хранения данных на стороне клиента, у него есть некоторые ограничения:

- Локальное хранилище ограничено по объему (обычно около 5 МБ).
- Данные в LocalStorage хранятся в виде строк, поэтому при необходимости сохранения сложных объектов они должны быть сериализованы и десериализованы.
- Данные в LocalStorage доступны только для того же источника (домена, протокол и порт), который их сохранял.