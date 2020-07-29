# Funções para array
Um guia sobre as funções que podem ser utilizadas para manipulação de arrays.

## Sumarização
1. **array.length**: Retorna a quantidade de elementos de um array.
2. **array.includes(<elemento>)**: Retorna um boolean com relação a existência de um elemento dentro do array.
3. **array.map(callback)**: Função cujo retorno produz o elemento do novo Array.

## Uso
Observação: As funções mais básicas não serão listadas aqui por falta de necessidade.

### array.includes(<elemento>)
Verifica se o elemento informado como argumento contém no array e retorna um boolean.

#### Código
```javascript
var myArray = ["Sandro"];
myArray.includes("Sandro"); //Output: true
```

### array.map(<callback>)
Retorna um array com os elementos modificados de acordo com a função de callback.
  
#### Código
```javascript
let myArray = ['Hello', 'World'];

myNewArray = myArray.map(word => {
    return "Concatenate: " + word;
});

console.log(myNewArray);
//output: 
myNewArray[0] = Concatenate: Hello
myNewArray[1] = Concatenate: World
```
