# [Exercícios com Python] Boas-vindas

## Enunciado

Faça um programa que leia um nome e mostre uma mensagem de boas-vindas com o nome dado.

## Resolução

Primeiramente, precisamos pedir ao usuário o nome dele através de uma mensagem na tela com a função **input**.

```py
nome = input('Qual o seu nome? ')
```

Aqui criamos a variável **nome** e iremos atribuir a ela aquilo que o usuário digitar. Lembre-se que o input recebe apenas dados do tipo strings.

É importante deixar um espaço para ao final da string dentro da input, por questões estéticas. Assim o que o usuário digitar não ficará colado logo depois da frase.

Decidi também usar mais duas funções. A **upper** para transformar todas as letras recebidas pela variável em maiúsculas e a **strip** que retirara espaços em branco no começo e no fim do dado passado pelo usuário, caso ele resolva fazer isso.

```py
nome = input('Qual o seu nome? ').upper().strip()
```

Agora podemos retornar na tela a mensagem de boas-vindas com o nome capturado.

```py
print(f'Seja bem-vinda(o) {nome}!')
```

A letra **f** logo após o primeiro parentese do print serve para indicar a formatação da string que aparecerá. Desse modo podemos chamar a variável entre chaves **{nome}** e dentro da string.

O código final será:

```py
nome = input('Qual o seu nome? ').upper().strip()
print(f'Seja bem-vinda(o) {nome}!')
```

tags: python, exercicio, boasVindas, input
