# Tipos booleanos em Python

![True or False](.img/trueFalse.jpg)

Os tipos booleanos são dois: True(verdadeiro) ou False(falso).

Apesar de aparentemente simples, com eles é possível fazer diversos tipos de programas e suas interações.

De maneira geral, booleanos são usados para retornar respostas de comparações. Exemplo:

```py
print(10 > 9)
```

A saída será:

```
True
```

Indicando que é verdade que o número 10 é maior do que o 9.

```py
print(10 == 9)
```

Saída:

```
False
```

Indicando que é falso a afirmação de 10 igual a 9.

E ainda,

```py
print(10 < 9)
```

O retorno será:

```
False
```

Pois 10 não é menor do que 9.

Podemos usá-lo também para verificar se uma variável é de um determinado tipo através da função **isinstance()**. Exemplo:

```py
x = 100 #atribuindo a variável x o valor 100
print(isinstance(x, float))
```

O retorno será

```
False
```

Pois 100 é um inteiro, não um decimal e por isso a tipagem é **int** e não **float**.

tags: python, booleanos, true, false
