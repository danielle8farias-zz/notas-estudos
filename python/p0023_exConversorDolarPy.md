# [Exercícios com Python] Conversor de Reais em Dólares

## Enunciado

Faça um programa que leia um valor em Reais e faça a conversão para Dolar.

![meme do dolar mortal kombat](./img/memedolarMK.jpg)

## Resolução

Primeiramente, precisamos pedir ao usuário o valor através da função **input**.

```py
real = input('Valor em Reais: R$')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **float**, pois o valor pode ter centavos (ponto flutuante).

```py
real = float(real)
```

É possível usar o mesmo nome da variável para atualizar o seu tipo, sem a necessidade de criar uma nova.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
real = float(input('Valor em Reais: R$'))
```

Agora fazendo a divisão do valor informado pela cotação do Dólar no dia:

```py
dolar = real/4.36
```

Imprimindo a mensagem na tela junto com os dados.

```py
print(f'Com R${real:.2f} você pode comprar US${dolar:.2f}')
```

Essa formatação é um pouco mais elaborada, como podemos ver.

- A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá.
- Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.
- Após as variáveis **real** e **dolar**, dentro das chaves, colocamos os dois pontos **(:)**.
- Em seguida colocamos um ponto **(.)**, pois não precisamos de espaços (isso é útil para alinhar colunas).
- Por último vem o número de casas decimais que queremos, no caso **2**, seguido de **f** que indica ponto flutuante.

O código final será:

```py
real = float(input('Valor em Reais: R$'))
dolar = real/4.36

print(f'Com R${real:.2f} você pode comprar US${dolar:.2f}')
```

tags: python, strings, literais, decimais
