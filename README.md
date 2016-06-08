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
    name: 'admin'
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
var foo = { n: 1 };
foo.x = foo = { n: 2 };
console.log(foo.x);
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
