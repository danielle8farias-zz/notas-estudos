# Declarando variável em Python

Para entender o que são variáveis, podemos usar a analogia de que uma variável é uma caixa onde guardamos algo, mas onde só podemos guardar um único item.

![analogia de uma variável com uma caixa](img/p0005-0.png)

É preciso dar nome as caixas, para chamá-las posteriormente.

Conceitualmente, variáveis são espaços na memória que serão reservados para guardar dados.

Para fazer a declaração de uma variável em Python, basta digitar o nome da variável, seguido do sinal de **igual** (que em Python serve para fazer a atribuição) e o tipo de dado escolhido.

Exemplo de variável do tipo **int**:

```py
numero = 11
```

Exemplo de variável do tipo **float**:

```py
area = 20.45
```

Exemplo de variável do tipo **boolean**:

```py
condicao = True
```

Exemplo de variável do tipo **string**:

```py
nome = 'Danielle'
```

Você pode declarar quantas variáveis quiser. Desse modo:

```py
num1 = 13
num2 = 17.98
planeta = 'Júpiter'
```

Ou desse:

```py
num1, num2, planeta = 13, 17.98, 'Júpiter'
```

Também é possível fazer a atribuição do valor de uma variável para outra. Exemplo:

```py
num1 = 23
num2 = num1
# imprimindo na tela ambos os números
print(f'1º número: {num1}')
print(f'2º número: {num2}')
```

Saída:

```
1º número: 23
2º número: 23
```

A tipagem em Python é dinâmica. Isso significa que o próprio interpretador da linguagem infere o tipo da variável a partir da atribuição que foi feita, sem a necessidade de que o programador explicite isso.

Para declarar uma constante, usa-se letras maiúsculas:

```py
PI = 3.14159
```

## Regras para nomear uma variável:

- Deve iniciar com uma letra ou um underscore **_**;
- Não pode começar com um número;
- Após a primeira letra, pode conter números e underscores;
- São case sensitive, isto é, uma variável chamada **nome** é diferente de Nome, NOME, NoMe e demais variações.

### Boas práticas:

Recomenda-se o uso de nomes de variáveis autoexplicativos. Por exemplo:

```py
nome_planeta = "Júpiter"
numero_posicao = 5
numero_satelites = 79
rotacao_horas = 9.8
```

tags: python, variavel, constante, tipos
