# Instalando o VS Code no Linux pelo terminal
Primeiramente é preciso verificar a arquitetura do processador através do comando:
```
$ uname -m
```
No meu caso, é um sistema de 64 bits.

Para baixar o pacote, digite:
```
$ wget "https://go.microsoft.com/fwlink/?LinkID=760868" -O vscode.deb
```
O comando **wget** serve para fazer downloads de arquivos.

Os parâmetros **-O vscode.deb** para nomear o arquivo que está sendo baixado. **-O** O maiúsculo vem de output, seguido do nome do arquivo e sua extensão.

Para instalar o pacote, digite no terminal, no diretório onde o arquivo foi baixado:
```
$ sudo dpkg -i vscode.deb
```
**sudo** serve para pedir permissões de administrador temporariamente.

**dpkg** é o gerenciador de pacotes das distribuições baseadas em Debian.

**-i** é o comando que indica instalação

Caso precise corrigir dependências, digite o comando:
```
$ apt install -f
```

tags: linux, vscode, dpkg, instalacao