# Concatenação de strings com Python

Com as strings, também é possível fazer concatenação das mesmas. Exemplo:
```py
x = '11'
y = '11'
concat = x + y
print(concat)
```
```
1111
```
Como são duas strings o sinal de **+** não opera como soma. Mas é possível somar dois números e fazer a conversão do resultado, como mostrado no exemplo abaixo:
```py
print('Isso custa ', str(6 + 5),' reais.')
```
```
Isso custa  11  reais.
```
Outro exemplo de concatenação de strings:
```py
nome = 'Danielle'
sobrenome = 'Farias'
nome_completo = nome + sobrenome
print(nome_completo)
```
```
DanielleFarias
```
Usando esse mesmo exemplo, temos ainda:
```py
nome_completo1 = nome +' '+ sobrenome
print(nome_completo1)
print(f'{nome} {sobrenome}')
```
A saída de ambas é a mesma:
```
Danielle Farias
```

tags: python, concatenacao, string, programacao
