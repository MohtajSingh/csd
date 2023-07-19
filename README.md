const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello World!');
  console.log(req.querry.name);
})

app.get('/peanut', (req, res) => {
    res.send('Hello Class!');
    console.log(req.querry);
  })

app.listen(3000)
