# [Exercícios com Python] Verificando uma palavra dentro de um string

## Enunciado

Faça um programa que leia o nome completo do usuário e procure pela palavra **Silva** nele.

## Resolução

Primeiramente, precisamos pedir ao usuário que digite seu nome completo através da função **input**.

```py
nome = input('Qual seu nome completo? ')
```

É possível ainda tratar essa string recebida para que desconsidere os espaços em branco no começo e no fim, com o método **strip**.

```py
nome = input('Qual seu nome completo? ').strip()
```

Convertendo todos os caracteres para letras minúsculas, temos

```py
nome = input('Qual seu nome completo? ').strip().lower()
```

Agora vamos verificar sem na string passada existe a palavra **Silva**, através do comando

```py
"silva" in nome
```

Aqui é necessário fazer a distinção entre caracteres maiúsculo e minúsculo, pois o operador lógico **in** retornará **True(Verdadeiro)** ou **False(Falso)**. Como acima fizemos a transformação para letras minúsculas, usamos **"silva"**.

Colocando dentro da função **print** para que apareça na tela.

```py
print("silva" in nome)
```

Formatando o print e deixando o retorno mais amigável para o usuário,

```py
print(f'Seu nome tem Silva? {"silva" in nome}')
```

- A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. E colocamos a expressão do operador lógico entre chaves **{}** dentro da string.

No código final, usando também o módulo que criamos no exercício [Criando cabeçalho e rodapé para os scripts Python](p0028_exCriandoModuloPy.md), temos

```py
from mensagem import cabecalho, rodape

cabecalho('tem "silva" no seu sobrenome?')
nome = input('Qual seu nome completo? ').strip().lower()
print(f'Seu nome tem Silva? {"silva" in nome}')
rodape()
```

Do mesmo jeito que usamos a palavra **Silva**, podemos usar qualquer outra palavra no lugar para encontrá-la dentro de uma string.

tags: python, modulo, string, in
