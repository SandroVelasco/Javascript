# High order functions e callback functions
High order functions são as funções que podem receber funções como parâmetro. Callback functions são funções que são utilizadas, através da sua referência, em outras funções. Vamos ver alguns exemplos a seguir.

## Exemplo
```javascript
function sum(num1, num2) {
  return num1 + num2;
}

function multiply(num1, num2) {
  return num1 * num2;
}

// operator = função
function calculator(num1, num2, operator) {
  return operator(num1, num2);
}

// chamada
calculator(1, 5, sum) // output: 6
```
