# String em JavaScript

Strings são úteis para guardar dados que podem ser representados na forma de texto.

Exemplo de um script fazendo uso da string:
```js
let nome = "Danielle";
console.log(nome);
```
Para fazer a concatenação de strings, usa-se o operador **+**. Exemplo:
```js
let primeiroNome = "Danielle";
let ultimoNome = "Farias";
let nomeCompleto = primeiroNome + " " + ultimoNome;
console.log(nomeCompleto);
```
As aspas duplas e o espaço entre elas na terceira linha serve para que as duas palavras não fiquem grudadas uma a outra.

Uma das operações mais básicas na string é checar seu tamanho. Para o código acima, temos:
```js
console.log(nomeCompleto.length);
```
Também é possível o acesso direto a um caractere da string.
```js
console.log(nome[0]);
```
Nesse caso estamos pegando a primeira letra.

tags: string, javascript, texto, tamanho
