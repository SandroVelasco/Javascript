# Spread and Rest
Spread (propagação), rest (descanso)

## Spread
O operador spread serve para fazer cópias de arrays ou objetos. Veja exemplo abaixo.

```javascript
var myArray = ['Hello']
var copiedArray = [...myArray];
//output copiedArray: ['Hello'];
```

## Rest
O operador rest serve para ceder ilimitados argumentos para uma função. Veja exemplo abaixo.

```javascript
var myFunc = (...args) => {
  return args;
}
```

args representa um array.
