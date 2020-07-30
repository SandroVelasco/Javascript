# Destructuring
Destructuring significa desestruturar. Em javascript, significa que você pode destruturar um objeto ou array e pegar apenas algumas de suas partes. Veja exemplo(s) abaixo.

## Array destructuring
```javascript
var myArray = ['Hello', 'World'];
var [elementOne, elementTwo] = myArray;
// Output: elementOne = 'Hello', elementTwo = 'World';
```

## Object destructuring
```javascript
var myObj = {
  name: 'Sandro',
  age: 20
}

var {name, age} = myObj;
// Output: name = myObj.name, age = myObj.age
```
