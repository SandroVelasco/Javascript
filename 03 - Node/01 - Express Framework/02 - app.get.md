# Get method
Um breve guia sobre o funcionamento do método GET com o Express.

## Uso
```javascript
//app.get(<rota>, <callback func>);

app.get("/", (req, res) => {
  res.send("<h1>Hello, there!</h1>");
});
```
