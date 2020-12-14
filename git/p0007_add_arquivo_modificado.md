# git commit -am: Atualizando arquivo modificado no Git


Para atualizar um arquivo que foi modificado no repositório, existem dois caminhos.

```
$ git add <arquivo>
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.
- **add** vai adicionar ao git o(s) arquivo(s) que virá(ão) em seguida.
- digite o nome do arquivo sem os sinais **< >**.

seguido do **commit**

```
$ git commit -m 'sua mensagem aqui'
```

Exemplo:

Aqui temos o arquivo index.html que foi modificado.

![arquivo modificado](img/p0007-0.png)

Adicionando o arquivo com o comando ```git add```

![git add no arquivo modificado](img/p0007-1.png)

E fazendo o **commit**

![fazendo o commit do arquivo](img/p0007-2.png)


## Atalho

Também é possível fazer o **commit das modificações** através de um **atalho**:

```
$ git commit -am 'adição de modificação do arquivo'
```

O parâmetro **-a** adiciona todos os arquivos que foram modificados, sem a necessidade de adicionar cada um individualmente.

Exemplo:

Aqui temos vários arquivos modificados

![vários arquivos modificados](img/p0007-3.png)

Usando o atalho

![usando o atalho](img/p0007-4.png)

**Observação:**
É importante notar que se houver um arquivo novo (ainda não rastreado pelo **git**) o comando ```git commit -am``` faz a adição do commit **apenas dos arquivos rastreados que foram modificados**.

tags: git, modificado, add, commit -a, commit -am
