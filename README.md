### 9. Массивы и их методы в JavaScript

#### Массивы

Массивы в JavaScript представляют собой упорядоченные коллекции элементов. Каждый элемент в массиве имеет индекс, начиная с 0.

**Пример создания массива:**

```javascript
let fruits = ["apple", "banana", "cherry"];
console.log(fruits[0]); // apple
```

#### Некоторые основные методы массивов:

1. **push** - добавляет один или несколько элементов в конец массива и возвращает новую длину массива.

```javascript
fruits.push("date");
console.log(fruits); // ["apple", "banana", "cherry", "date"]
```

2. **pop** - удаляет последний элемент из массива и возвращает его.

```javascript
let lastFruit = fruits.pop();
console.log(lastFruit); // date
```

3. **shift** - удаляет первый элемент из массива и возвращает его.

```javascript
let firstFruit = fruits.shift();
console.log(firstFruit); // apple
```

4. **unshift** - добавляет один или несколько элементов в начало массива и возвращает новую длину массива.

```javascript
fruits.unshift("apple");
console.log(fruits); // ["apple", "banana", "cherry"]
```

5. **slice** - возвращает новый массив, содержащий копию части исходного массива.

```javascript
let someFruits = fruits.slice(1, 3);
console.log(someFruits); // ["banana", "cherry"]
```

6. **splice** - изменяет содержимое массива, удаляя, заменяя или добавляя новые элементы.

```javascript
fruits.splice(1, 1, "orange");
console.log(fruits); // ["apple", "orange", "cherry"]
```

7. **forEach** - выполняет указанную функцию один раз для каждого элемента в массиве.

```javascript
fruits.forEach(fruit => {
    console.log(fruit);
});
```

8. **map** - создает новый массив с результатами вызова указанной функции для каждого элемента массива.

```javascript
let capitalizedFruits = fruits.map(fruit => fruit.toUpperCase());
console.log(capitalizedFruits); // ["APPLE", "ORANGE", "CHERRY"]
```

9. **filter** - создает новый массив со всеми элементами, которые проходят тест, предоставленный функцией.

```javascript
let longFruits = fruits.filter(fruit => fruit.length > 5);
console.log(longFruits); // ["orange"]
```

10. **reduce** - применяет функцию к аккумулятору и каждому элементу массива (слева направо), чтобы свести его к одному значению.

```javascript
let totalLength = fruits.reduce((acc, fruit) => acc + fruit.length, 0);
console.log(totalLength); // длина всех строк в массиве
```

11. **find** - возвращает первый элемент в массиве, который удовлетворяет предоставленному тесту.

```javascript
let foundFruit = fruits.find(fruit => fruit.startsWith("o"));
console.log(foundFruit); // orange
```

12. **indexOf** и **lastIndexOf** - возвращают первый и последний индекс указанного элемента соответственно.

```javascript
console.log(fruits.indexOf("orange")); // 1
```

13. **some** и **every** - проверяют, удовлетворяют ли некоторые или все элементы предоставленному тесту.

```javascript
console.log(fruits.some(fruit => fruit.length > 5)); // true
console.log(fruits.every(fruit => fruit.length > 5)); // false
```

14. **concat** - используется для объединения двух или более массивов.

```javascript
let moreFruits = fruits.concat(["grape", "melon"]);
console.log(moreFruits); // ["apple", "orange", "cherry", "grape", "melon"]
```

Это лишь часть методов, которые предоставляют массивы в JavaScript. Каждый из этих методов имеет свою специфику и может быть полезен в разных ситуациях.
