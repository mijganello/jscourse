### 15. Выбор DOM-элементов в JavaScript

Для взаимодействия и манипулирования элементами на веб-странице с помощью JavaScript необходимо сначала выбрать соответствующий DOM-элемент. В JavaScript существует несколько методов для выбора элементов.

#### 1. `getElementById`

Этот метод возвращает элемент по его атрибуту `id`. Идентификаторы должны быть уникальными на странице.

```javascript
let element = document.getElementById("myId");
```

#### 2. `getElementsByTagName`

Возвращает коллекцию элементов по имени тега.

```javascript
let paragraphs = document.getElementsByTagName("p"); // получить все элементы <p>
```

#### 3. `getElementsByClassName`

Возвращает коллекцию элементов по имени класса.

```javascript
let items = document.getElementsByClassName("myClass"); // получить все элементы с классом "myClass"
```

#### 4. `querySelector`

Возвращает первый элемент, соответствующий указанному CSS-селектору.

```javascript
let firstButton = document.querySelector("button"); // получить первую кнопку на странице
```

#### 5. `querySelectorAll`

Возвращает NodeList, содержащий все элементы, соответствующие указанному CSS-селектору.

```javascript
let allButtons = document.querySelectorAll("button"); // получить все кнопки на странице
```

#### 6. `parentElement` и `children`

Эти свойства позволяют перемещаться по иерархии DOM.

```javascript
let parent = element.parentElement; // получить родительский элемент
let childElements = element.children; // получить всех дочерних элементов
```

#### 7. `nextElementSibling` и `previousElementSibling`

Эти свойства позволяют перемещаться между соседними элементами на одном уровне.

```javascript
let nextSibling = element.nextElementSibling; // получить следующий элемент на одном уровне
let prevSibling = element.previousElementSibling; // получить предыдущий элемент на одном уровне
```

#### Краткий обзор:

1. **Выбор элементов** в JavaScript основан на их атрибутах, таких как id или class, или на их отношениях в DOM.
2. Методы, такие как `querySelector` и `querySelectorAll`, предоставляют гибкий способ выбора элементов с использованием CSS-селекторов.
3. После выбора элемента вы можете манипулировать им, изменяя его свойства, применяя стили или добавляя слушателей событий.
