# Event Listener
Um breve guia sobre Event Listener. O Event Listener funciona como uma escuta que é adicionada a um determinado elemento, que, aguarda pelo acionamento de alguma ação. Um exemplo de ação, poderia ser, a ação de clique em um elemento.

## Sintaxe e exemplo de uso
```javascript
document.querySelector("button").addEventListener(<evento>, <função anônima ou de callback>);

// Método por função anônima
document.querySelector("button").addEventListener("click", function() {
  alert("Botão clicado!");
});

// Método por função de callback
function handleClick() {
  alert("Botão clicado!");
}

document.querySelector("button").addEventListener("click", handleClick);
```
