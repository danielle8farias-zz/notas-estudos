# [Exercícios com Python] Cálculo de área

## Enunciado

Faça um programa que leia a altura e largura da parede em metros; calcule a área e a quantidade
de tinta necessária para pintá-la, sabendo que cada litro pinta 2m².

## Resolução

Primeiramente, precisamos pedir ao usuário a altura e a largura da parede (em metros) através da função **input**.

```py
largura = input('Informe a largura da parede(m): ')
altura = input('Informe a altura da parede(m): ')
```

Aqui é importante lembrar que a função **input** só recebe **strings**. Então , devemos fazer a conversão desse dado para **float**, pois queremos que receba também número decimal.

```py
largura = float(largura)
altura = float(altura)
```

É possível usar o mesmo nome das variáveis para atualizar seus tipos, sem a necessidade de criar novas.

Outra maneira mais prática de realizar a conversão é fazê-la no momento da captura do dado. Assim:

```py
largura = float(input('Informe a largura da parede(m): '))
altura = float(input('Informe a altura da parede(m): '))
```

Agora, fazendo o cálculo da área:

```py
area = largura*altura
```

>caso ache necessário, faça uma revisão de matemática sobre [cálculo da área do retângulo](https://www.youtube.com/watch?v=W3pE970YBrE).

E o cálculo da quantidade de tinta:

```py
quantidade_tinta = area/2
```

> caso ache necessário, faça uma revisão de matemática sobre [regra de três simples](https://www.youtube.com/watch?v=7gK3-QG363o).

Imprimindo a mensagem na tela junto com os dados calculados, temos

```py
print(f'A área da parede = {area:.2f}m².')
print(f'A quantidade de tinta necessária: {quantidade_tinta:.2f} litros.')
```
Essa formatação é um pouco mais elaborada, como podemos ver.

- A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá.
- Desse modo podemos chamar as variáveis entre chaves **{}** dentro da string.
- Após as variáveis **area** e **quantidade_tinta**, dentro das chaves, colocamos os dois pontos **(:)**.
- Em seguida colocamos um ponto **(.)**, pois não precisamos de espaços (isso é útil para alinhar colunas).
- Por último vem o número de casas decimais que queremos, no caso **duas (2)**, seguido de **f** que indica ponto flutuante.

O código final será:

```py
largura = float(input('Informe a largura da parede(m): '))
altura = float(input('Informe a altura da parede(m): '))

area = largura*altura
quantidade_tinta = area/2

print(f'A área da parede é {area:.2f}m².')
print(f'A quantidade de tinta necessária é {quantidade_tinta:.2f} litros.')
```

tags: python, area, literais, regraDeTres
