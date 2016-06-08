# JavaScript test

What will be printed to the console?

## Task 1
```javascript
function loop() {
  console.log(i);
  for (var i = 0; i < 5; i++) {
    console.log(i);
  }
  console.log(i);
}

loop();
```

## Task 2
```javascript
for (var i = 0; i < 5; i++) {
  setTimeout(function () {
    console.log(i);
  }, 1000);
}
```

## Task 3
```javascript
function override() {
  var a = 2
  b = 2;
}

var a = 1
  b = 1;

override();

console.log(a);
console.log(b);
```

## Task 4
```javascript
function printNames() {
  var names = ['John', 'Yoko', 'Elvis'];
  for (name in names) {
    console.log(name);
  }
}

printNames();
```

## Task 5
```javascript
function getUser() {
  return
  {
    name: 'John'
  };
}

var user = getUser();
console.log(user);
```

## Task 6
```javascript
console.log(1);
setTimeout(function () {
  console.log(2);
}, 0);
console.log(3); 
```

## Task 7
```javascript
var fruits = ['apple', 'banana'];
fruits.length = 1;
console.log(fruits);
```

## Task 8
```javascript
var obj = { x: 1 };
obj.y = obj = { x: 2 };
console.log(obj.y);
```

## Task 9
```javascript
var strings = ['10', '10', '10'];
console.log(strings.map(parseInt));
```

## Task 10
```javascript
console.log(9999999999999999);
console.log(0.1 + 0.2);
console.log(012);
```

## Task 11
```javascript
function Person(name) {
  this.name = name;
  this.sayName = function () {
    setTimeout(function () {
      console.log(this.name);
    }, 500);
  };
}

var person = new Person('John');
person.sayName();
```

## Task 12
```javascript
function Person(name) {
  this.name = name;
}

var name = 'Yoko';
var person = Person('John');
console.log(name);
```

## Task 13
```javascript
for (var i = 0; i < 3; i++) {
  subLoop();
}

function subLoop() {
  for (i = 0; i < 3; i++) {
    console.log(i);
  }
}
```

## Task 14
```javascript
function List() { };

List.prototype = {
  items: [],
  addItem: function (item) {
    this.items.push(item);
  }
};

var listA = new List();
var listB = new List();

listA.addItem('a1');
listB.addItem('b1');
listA.addItem('a2');

console.log(listA.items.length);
console.log(listB.items.length);
```
