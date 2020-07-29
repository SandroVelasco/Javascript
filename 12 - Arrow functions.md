# Arrow functions
Por que usar arrow functions? 

1. Sintaxe menor.
2. Permite utilizar a palavra-chave "this".

## Formas de uso
1. Forma longa
```javascript
let myFunc = (a, b, c) => {
  return a + b + c;
}
```

2. Forma curta
```javascript
// O return é implicito.
// Com vários parâmetros
let myFunc = (a, b, c) => a + b + c;

// Com apenas 01 parâmetro
let myFunc = a => a + b + c;

// Sem parâmetro
let myFunc = () => ...;
```
