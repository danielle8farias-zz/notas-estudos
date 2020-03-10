# Estruturas de tomada de decisão (desvio condicional) em Python

![desvio condicional](./img/meme_carro_desvio.png)

As estruturas de tomada de decisão são utilizadas quando o programa precisa decidir, entre mais de uma opção, qual caminho tomar.

## Condicional simples

O **if** é uma estrutura de condição que permite avaliar uma expressão passada e, de acordo com o resultado, executar um determinada bloco de comandos.

```py
if (expressão que pode ser verdadeira ou falsa):
    <executa se verdade>
```

Se a condição após o **if** for verdade, o bloco de comando dentro dele será executado. Esse bloco de comando precisa estar indentado (recuo com a tecla TAB).

Exemplo:

```py
num1 = int(input('Digite um número inteiro: '))
num2 = int(input('Digite outro número inteiro: '))

subtracao = num1 - num2

if subtracao > 0:
    print('O resultado é positivo')

print(f'Valor da subtração = {subtracao}')
```

Acima, podemos conferir que, se o valor da subtração der maior do que zero (número positivo), então o programa imprime na tela a mensagem *"O resultado é positivo"*.

O último print, com o valor da subtração, será sempre impresso, independente de entrar no **if** ou não, pois ele está fora da indentação. O interpretador entende que esse bloco de comando não faz parte da condicional.

tags: python, if, else, elif
