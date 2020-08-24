# Terminal: Gerenciando grupos


Um determinado grupo, no Linux, pode conter várias pessoas e restrições (ou permissões) a determinadas partes do sistema. Quando um usuário é criado, é também criado um grupo com o nome desse usuário.

Para ver os grupos dos usuários existentes no seu sistema, digite:

```
$ cat /etc/group
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- no diretório **etc/** temos arquivos de configuração, scripts de inicialização, entre outros.

- **group** é o arquivo do sistema que define os grupos aos quais os usuários pertencem.

> sobre o comando [cat, clique aqui](p0011_cat.md).

O arquivo **group** contém as seguintes informações:

```
<nome_do_grupo>:<senha>:<id_do_grupo>:<usuários_que_são_membros_do_grupo_separados_por_vírgulas>
```

Exemplo:

```
cdrom:x:24:danielle8farias,vict0rfarias
```

- **cdrom**, nome do grupo;

- **x**, indica que a senha está encriptada;

- **24**, id do grupo;

- **danielle8farias** e **vict0rfarias**, são os membros que pertencem a esse grupo.

## Ver grupos de um determinado usuário

Para saber quais grupos um determinado usuário é membro, digite:

```
$ groups <nome_do_usuário>
```

- digite o nome do usuário sem os sinais **< >**.

## Ver id do grupo de um determinado usuário

Para visualizar a id do grupo de um usuário, digite:

```
$ id -g <nome_do_usuário>
```

## Ver id de todos os grupos de um determinado usuário

Para visualizar as ids de todos os grupos de um usuário, digite:

```
$ id -G <nome_do_usuário>
```

## Criando novo grupo

Para criar um grupo, digite:

```
$ sudo groupadd <nome_do_novo_grupo>
```

- **sudo** serve para pedir permissões de administrador temporariamente.

## Excluindo grupo

Para excluir um grupo, digite:

```
$ sudo groupdel <nome_do_grupo>
```

## Adicionando usuário a um grupo

Para adicionar um usuário a um determinado grupo, digite:

```
$ sudo usermod -a -G <nome_do_grupo> <nome_do_usuário_que_deseja_adicionar_ao_grupo>
```

- **usermod**, adiciona ou modifica informações de um usuário já existente no sistema.

Outra maneira de fazer isso, é com o comando:

```
$ sudo gpasswd -a <nome_do_usuário> <nome_do_grupo>
```

- **gpasswd** é comando que permite administrar o arquivo **/etc/group**;

- **-a** para adicionar um novo usuário ao grupo.

## Excluindo usuário de um grupo

Para excluir um determinado usuário de um grupo, digite:

```
$ sudo gpasswd -d <nome_do_usuário> <nome_do_grupo>
```

- **-d** para deletar um determinado usuário do grupo.

tags: linux, terminal, group
