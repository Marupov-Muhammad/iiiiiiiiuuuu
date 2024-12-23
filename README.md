Методҳои маъмул барои кор бо массивҳо
1. Илова ва ҳазфи элементҳо:
push(): Иловаи элемент ба охири массив.
pop(): Ҳазфи элемент аз охири массив.
unshift(): Иловаи элемент ба аввали массив.
shift(): Ҳазфи элемент аз аввали массив.
javascript
Копировать код
let fruits = ["apple", "banana"];
fruits.push("cherry"); // ["apple", "banana", "cherry"]
fruits.pop(); // ["apple", "banana"]
2. Идоракунии элементҳо:
splice(start, deleteCount, item1, item2, ...): Илова ё ҳазфи элементҳо дар массив.
slice(start, end): Гирифтани қисми массив бе тағйир додани массиви аслӣ.
javascript
Копировать код
let numbers = [10, 20, 30, 40, 50];
let sliced = numbers.slice(1, 3); // [20, 30]
numbers.splice(2, 1, 25); // [10, 20, 25, 40, 50]
3. Ҷустуҷӯ ва санҷиш:
indexOf(value): Баргардонидани индекси элемент (ё -1 агар набошад).
includes(value): Санҷидани мавҷудияти элемент.
javascript
Копировать код
let items = ["apple", "banana", "cherry"];
console.log(items.indexOf("banana")); // 1
console.log(items.includes("grape")); // false
4. Таҳлилу таҳрир:
map(): Табдили ҳар як элемент ба массиви нав.
filter(): Филтр кардани элементҳо бо асоси шарт.
reduce(): Фишурдасозии массив ба як арзиши ягона.
forEach(): Гузариш аз болои ҳар як элемент.
javascript
Копировать код
let numbers = [10, 20, 30, 40];

// Таҳлил бо map
let doubled = numbers.map(num => num * 2); // [20, 40, 60, 80]

// Филтр бо шарт
let filtered = numbers.filter(num => num > 20); // [30, 40]

// Ҷамъ бо reduce
let sum = numbers.reduce((total, num) => total + num, 0); // 100

// Гузариш бо forEach
numbers.forEach(num => console.log(num));
Мисоли умумӣ:
javascript
Копировать код
let tasks = ["Homework", "Shopping", "Cleaning"];

// Иловаи вазифа
tasks.push("Exercise"); // ["Homework", "Shopping", "Cleaning", "Exercise"]

// Филтр кардани вазифаҳои дорои зиёда аз 7 ҳарф
let longTasks = tasks.filter(task => task.length > 7);
console.log(longTasks); // ["Homework", "Cleaning"]
Хулоса
Массивҳо дар JavaScript як қисми муҳими коркарди маълумоти гурӯҳӣ мебошанд. Онҳо барои нигаҳдорӣ, таҳлил, идоракунӣ ва ҷустуҷӯи маълумот методҳои тавоно пешниҳод мекунанд, ки барои таҳияи барномаҳо хеле муфиданд.
