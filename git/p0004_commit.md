# git commit: Enviando arquivos para o repositório Git

Depois de usar o comando de adicionar arquivos no git

```
$ git add nome_do_arquivo
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

Para confirmar as alterações e enviar os arquivos para o seu repositório, fazemos

```
$ git commit -m "escreva sua mensagem aqui"
```

A mensagem descrita entre aspas duplas serve para identificar a ação sobre os arquivos.

Conferindo o estado do git, temos algo como

![status limpo](img/p0004-0.png)

No fluxo do git,

![fluxo commit do git](img/p0004-1.png)

> abaixo do nome do arquivo está escrito a chave (ou hash) que identifica o commit

tags: git, commit, add, status
