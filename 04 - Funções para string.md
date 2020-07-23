# Funções - String
Olá, seja bem-vindo! Em 23 de julho de 2020, tomei a liberdade de criar este documento para futuras consultas, tendo em vista que funções para manipular strings são muito utilizadas.

## Sumarização
1. **string.length:** Retorna a quantidade de caracteres de uma string.
2. **string.slice():** Corta a string e retorna o que o programador deseja.
3. **string.toUpperCase():** Transforma a string para caixa alta.
4. **string.toLowerCase():** Transforma a string para caixa baixa.

## string.length
Retorna a quantidade de caracteres de uma string.

### Exemplo de uso
```javascript
var message = "Hello";
message.length; //Output: 5
```

## string.slice()
Corta a string e retorna o que o programador deseja.

### Sintaxe

string.slice( <initial position>, <end position> );

### Exemplo de uso
```javascript
var message = "Hello world";
message.slice(0,5); //Output: Hello
```

## string.toUpperCase e string.toLowerCase()
Transforma a string para caixa alta ou caixa baica.

### Exemplo de uso
```javascript
var message = "Hello world";
message.toUpperCase();
message.toLowerCase();
```
