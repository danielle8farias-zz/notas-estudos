# Divisão inteira com JavaScript

Para efetuar uma divisão e retornar apenas o valor inteiro, devemos utilizar a função **parseInt**.
Desse modo, temos:
```js
parseInt(11/5)
```
O resultado será 5.

Fazendo o script, teremos:
```js
let a = 11;
let b = 2;

let resultado = parseInt(a / b);

console.log(resultado);
```
A função **parseInt** também é usada para a conversão de **string** para **inteiros**. Exemplo:
```js
let onze = parseInt("11");
console.log("O tipo da variável 'onze' é: ", typeof onze);
```

tags: parseint, javascript, divisao, string
