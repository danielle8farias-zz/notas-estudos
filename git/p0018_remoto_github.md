# Enviando um projeto para o repositório remoto no GitHub

![Octocat](img/p0018-0.png)

Acesse sua conta no [GitHub](https://github.com/). Caso ainda não tenha, basta criá-la (é fácil e rápido).

Clique o sinal de mais para abrir o menu e em seguida em **New repository**.

![criando novo repositório no GitHub](img/p0018-1.png)

Dê o nome de sua preferência, além da descrição e indique se seu repositório será público ou privado.

![criando repositório](img/p0018-2.png)

Para finalizar, clique em **Create repository**.

Em seguida aparece uma tela com três opções:

![tela de configuração rápida](img/p0018-3.png)

- A primeira diz respeito a crianção de um **novo repositório** (inclui a inicialização do Git no diretório).

- A segunda diz respeito a um **repositório já existente** e que desejo colocar no GitHub (é a situação que irei utilizar).

- A terceira diz respeito a **importação** de um código de outro repositório.

Sendo assim, dentro da pasta do nosso projeto, digitamos o comando:

```
$ git remote add origin <link para o repositório do seu projeto>
```

para fazer a ligação com o repositório remoto.

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.
- substitua o \<link para o repositório do seu projeto> pelo link sem os sinais **<>**

No meu caso:

```
$ git remote add origin https://github.com/danielle8farias/cautious-waffle.git
```

Logo após

```
$ git push -u origin master
```

Isso significa as modificações no **branch(ramo)** local, denominado **master** será **empurrado(push)** para o remoto chamado **origin**. O **-u** é uma atalho para o comando **--set-upstream**; ficando definido esse **branch** como uso padrão até que você o modifique novamente. Das próximas vezes em que você precisar empurrar seu código para o GitHub basta usar o comando **git push** para esse mesmo **branch**.

Em seguida, será pedido seu **nome de usuária** e sua **senha do GitHub**:

![entrando com usuário e senha do GitHub](img/p0018-4.png)

Se tudo estiver certo o retorno será algo similar a:

![retorno do comando push](img/p0018-5.png)

Fazendo a associação entre os branchs **master(local)** e **origin(remoto)**.

## Verificando o repositório remoto

Caso precise verificar se há um repositório remoto em algum diretório local, digite:

```
$ git remote
```

O retorno será o nome do branch remoto.

Para saber mais detalhes desse repositório remoto, digite no terminal:

```
$ git remote -v
```

E o retorno será o link para o repositório remoto.

tags: git, github, repositorio, remoto
