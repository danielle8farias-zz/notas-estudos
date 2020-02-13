# [Exercícios com Python] Retorna inteiro de número decimal

## Enunciado

Faça um programa que leia um número decimal dado pelo usuário e retorne apenas o número inteiro.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('Digite um número com casa decimal: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **float**, pois queremos receber um número decimal (com ponto flutuante).

```py
num = float(num)
```

É possível usar o mesmo nome das variáveis para atualizar os seus tipos, sem a necessidade de criar novas.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = float(input('Digite um número com casa decimal: '))
```

Agora basta imprimir a mensagem na tela junto com os dados coletados.

```py
print(f'A parte inteira do número é {num:.0f}')
```

Essa formatação é um pouco mais elaborada, como podemos ver.

- A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá.
- Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.
- Após a variável **num**, dentro das chaves, colocamos os dois pontos **(:)**.
- Em seguida colocamos um ponto **(.)**, pois não precisamos de espaços (isso é útil para alinhar colunas).
- Por último vem o número de casas decimais que queremos, no caso **zero (0)**, seguido de **f** que indica ponto flutuante.

O código final será:

```py
num = float(input('Digite um número com casa decimal: '))
print(f'A parte inteira do número é {num:.0f}')
```

tags: python, strings, literais, arredondamento
