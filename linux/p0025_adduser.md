# Terminal: Adicionando usuário


Para adicionar um novo usuário, digite no terminal

```
$ sudo adduser <nome_do_novo_usuário>
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **adduser** para adicionar o novo usuário.

- digite o nome do novo usuário sem os sinais **< >**.

Em seguida será pedido que seja definido uma senha para o novo usuário, além de nome completo e outros detalhes opcionais e que podem ser deixados em branco.

Após ser confirmada a pergunta, o usuário já estará disponível.

Para ver os dados do usuários do sistema, inclusive o novo, digite:

```
$ cat /etc/passwd
```

> sobre o comando [cat, clique aqui](p0011_cat.md).

- no diretório **etc/** temos arquivos de configuração, scripts de inicialização, entre outros.

O arquivo **passwd** contém as seguintes informações:

```
<usuário>:<senha>:<id_do_usuário>:<id_do_grupo_primário>:<descrições_como_nome_completo_entre_outros>:<diretório_home>:<nome_do_shell>
```

Por exemplo, no meu caso temos:

```
danielle8farias:x:1000:1000:Danielle Farias,,,:/home/danielle8farias:/bin/bash
```

- **danielle8farias**, meu nome de usuário;

- **x**, indica que a senha está encriptada;

- **1000**, id do usuário;

- **1000**, id do grupo primário do qual o usuário faz parte;

- **Danielle Farias,,,**, meu nome e outras informações pessoais, que no meu caso estão em branco;

- **/home/danielle8farias**, meu diretório home;

- **/bin/bash**, o shell que estou usando, que é o Bash.

tags: adduser, terminal, linux, usuario
