# [Exercícios com Python] Separação dos dígitos

## Enunciado

Faça um programa que leia um número de 0 a 9999 e mostre cada um dos dígitos separados.

## Resolução

Primeiramente, precisamos pedir ao usuário um número através da função **input**.

```py
num = input('Digite um número inteiro: ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **int**.

```py
num = int(num)
```

É possível usar o mesmo nome da variável para atualizar seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
num = int(input('Digite um número inteiro: '))
```

Agora vamos separar a(s) unidade(s). Para isso criamos a variável **unidade** e atribuímos a ela, o resto da divisão por 10.

```py
unidade = num % 10
```

Desse modo pegaremos o último algarismo; aquele que é correspondente a unidade.

>caso necessário, faça uma revisão de matemática sobre [sistema de numeração decimal](https://www.youtube.com/watch?v=uxsh-s4OgLE).

Agora vamos separar a(s) dezena(s). Criamos a variável **dezena** e atribuímos a ela divisão inteira por 10 (desse modo retiramos a unidade) e em seguida fazemos o resto da divisão por 10 (desse modo pegando o último algarismo).

```py
dezena = num // 10 % 10
```

Agora vamos separar a(s) centena(s). Criamos a variável **centena** e atribuímos a ela divisão inteira por 100 (desse modo retiramos a dezena) e em seguida fazemos o resto da divisão por 10 (desse modo pegando o último algarismo).

```py
centena = num // 100 % 10
```

Agora vamos separar a(s) unidade(s) de milhar(es). Criamos a variável **milhar** e atribuímos a ela divisão inteira por 1000 (desse modo retiramos a centena) e em seguida fazemos o resto da divisão por 10 (desse modo pegando o último algarismo).

```py
milhar = num // 1000 % 10
```

Imprimindo a mensagem na tela junto com os dados calculados, temos

```py
print(f'Unidade: {unidade}')
print(f'Dezena: {dezena}')
print(f'Centena: {centena}')
print(f'Unidade de Milhar: {milhar}')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.

O código final será:

```py
num = int(input('Digite um número inteiro: '))

unidade = num % 10
dezena = num // 10 % 10
centena = num // 100 % 10
milhar = num // 1000 % 10

print(f'Unidade: {unidade}')
print(f'Dezena: {dezena}')
print(f'Centena: {centena}')
print(f'Unidade de Milhar: {milhar}')
```

tags: python, literais, modulo, divisaoInteira
