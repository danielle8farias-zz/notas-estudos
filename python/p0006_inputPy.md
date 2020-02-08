# Função input do Python

A função **input** imprime uma mensagem na tela (a mensagem é opcional) e captura o que foi digitado pelo usuário antes de dar continuidade ao programa. Exemplo:

```py
input('Qual o seu nome? ')
```

Essa função recebe sempre uma string.

Para não perder o dado digitado, podemos atribuí-lo a uma variável.

```py
nome = input('Qual o seu nome? ')
```

Assim, basta digitar o nome da variável para recuperar o que foi digitado.

É possível ainda tratar essa string recebida para que desconsidere os espaços em branco no começo e no fim, com o método **strip**.

```py
nome = input('Qual o seu nome? ').strip()
```

Para imprimir o dado digitado na tela, use a função print com o nome da variável.

```py
print(nome)
```

Para usar o print acrescido de uma frase, fazemos:

```py
print(f'Seja bem-vindo {nome}!')
```

A letra **f** dentro da função permite a formatação. As chaves **{}** servem para marcar a variável que será incluída. As aspas simples marcam o início e o fim do que será imprimido na tela.

O script final ficará:

```py
nome = input('Qual o seu nome? ').strip()
print()
print(f'Seja bem-vindo {nome}!')
```

O **print()** vazio serve para pular uma linha.

tags: python, print, input, strip
