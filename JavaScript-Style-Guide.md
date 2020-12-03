# JavaScript-Style-Guide-by-Gard0  `// Советы по стилю кода JS`

## Главное

#### Код должен быть максимально `читаемым и понятным`.

* Взять сложную задачу и написать такой код для её решения, который и правильно работает, и легко читается, понятен для людей. 

## Синтаксис

#### Шпаргалка с правилами синтаксиса

* [Learn.javascript.ru](https://learn.javascript.ru/coding-style#sintaksis)

## Фигурные скобки

#### Фигурные скобки пишутся с открывающей скобкой на той же строке, что и соответствующее ключевое слово – не на новой строке. Перед открывающей скобкой должен быть пробел. Вот пример:

   ```javascript
    if (condition) {
      // делай это
      // ...и это
      // ...и потом это
    }
   ```
 
 ## Длина строки
 
 #### Никто не любит читать длинные горизонтальные строки кода
 
 ##### Лучше так
 
```javascript
// обратные кавычки ` позволяют разделять строку на части
let str = `
  Рабочая группа TC39 организации Ecma International -
  это группа JavaScript-разработчиков, теоретиков и авторов движков JavaScript,
  которые вместе с сообществом занимаются поддержкой и развитием языка JavaScript.
`;
```

 ##### Или так
 
```javascript
if (
  id === 123 &&
  moonPhase === 'Waning Gibbous' &&
  zodiacSign === 'Libra'
) {
  letTheSorceryBegin();
}
```

* Максимальную длину строки согласовывают в команде. Обычно это `80` или `120` символов.

## Точка с запятой

* Точки с запятой должны присутствовать после каждого выражения, даже если их, казалось бы, можно пропустить.

## Уровни вложенности

#### Уровней вложенности должно быть немного

```javascript
for (let i = 0; i < 10; i++) {
  if (!cond) continue;
  ...  // <- нет лишнего уровня вложенности
}
```

## Размещение функций

#### Сначала код, затем функции

* При чтении кода мы сначала хотим знать, что он делает. Если сначала идёт код, то это тут же становится понятно.

```javascript
// код, использующий функции
let elem = createElement();
setHandler(elem);
walkAround();

// --- вспомогательные функции ---
function createElement() {
  ...
}

function setHandler(elem) {
  ...
}

function walkAround() {
  ...
}
```

## Руководства по стилю кода

#### Используй опыт других разработчиков. Вот пример

* [Google JavaScript Style Guide](https://google.github.io/styleguide/javascriptguide.xml)
* [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
* [Idiomatic.JS](https://github.com/rwaldron/idiomatic.js)
* [StandardJS](https://standardjs.com/)
* [Learn.javascript.ru](https://learn.javascript.ru/coding-style)
