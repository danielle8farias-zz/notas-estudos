# String em Python

**String** é, basicamente, uma sequência de caracteres imutável. Quando precisamos manipular dados como frases e palavras, usamos o tipo string.

Para declarar uma string, usa-se aspas simples (apóstrofo) ou duplas. Exemplo:
```py
print('Isso é uma string.')
print("Isso também é uma string.")
```

Caso seja preciso usar as aspas dentro da string, faz-se o seguinte:
```py
print("She's inteligent.")
```
Usa-se as aspas duplas fora, para que se possa usar as aspas simples dentro.
```py
print('Ela disse: "Eu não sei!"')
```
Ou usa-se as aspas simples fora, quando necessário usar as aspas duplas dentro.

Outra alternativa é usar a **contrabarra** como escape.
```py
print('She\'s inteligent.')
```
```
She's intelligent.
```
Desse modo o interpretador do Python ignora o caractere especial seguinte, que no nosso caso é o apóstrofo.

tags: python, string, contrabarra, escape
