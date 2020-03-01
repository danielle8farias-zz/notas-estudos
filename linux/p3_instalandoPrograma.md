# Instalando programas no Linux

Essa instrução serve para as distros Linux que usam o gerenciador de pacotes Debian (.deb).

```
$ sudo apt install nome_do_programa
```

Provavelmente, após esse comando o sistema irá pedir a senha que você configurou no início da instalação do sistema.

Para fazer a instalação sem a pergunta que confirmação, basta acrescentar o **-y** ao final do comando.

```
$ sudo apt install nome_do_programa -y
```

**sudo** serve para pedir permissões de administrador temporariamente.

**apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

**install** é o comando de instalar, indicando ao apt o que fazer.

tags: linux, instalacao, apt, terminal
