# git commit: Enviando arquivos para o repositório Git


Após adicionar arquivos no **index**, [clique aqui caso não saiba adicionar](p0002_add.md), precisamos levar esses arquivos para dentro do nosso repositório.

Até agora temos:

![arquivos monitorados](img/p0002-4.png)

Enquanto no **fluxo** do git,

![arquivos no index](img/p0003-0.png)

Ao colocar os arquivos dentro no repositório, precisamos informar ao **Git** o motivo desses arquivos, com o comando:

```
$ git commit -m 'escreva sua mensagem aqui'
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- pode-se usar aspas simples ou duplas para escrever a mensagem.

No nosso exemplo, temos:

```
$ git commit -m 'commit inicial'
```

![primeiro commit](img/p0004-0.png)

Conferindo o **estado** do **Git**, temos:

![status limpo](img/p0004-1.png)

E no fluxo,

![fluxo commit do git](img/p0004-2.png)

Esse conjunto de caracteres e números que aparece ao lado da palavra **commit** é a **chave (ou hash)** que identifica o próprio.

tags: git, commit, add, status
