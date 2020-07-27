# Terminal: Desinstalando programas no Linux


Essa instrução serve para as distros Linux baseadas no Debian (Ubuntu, Mint e derivados).

```
$ sudo apt remove nome_do_programa
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

- **remove** é o comando para remover, indicando ao apt o que fazer.

Provavelmente, após esse comando o sistema irá pedir a **senha** que você configurou no início da instalação do sistema operacional; além do pedido de confirmação da desinstalação.

Você também pode usar o **dpkg** para remover pacotes **.deb** assim,

```
$ sudo dpkg -r nome_do_pacote.deb
```

- **dpkg** do inglês, *Debian Package*, é uma ferramenta que gerencia pacotes .deb.

- **r** é o comando de remover, indicando ao dpkg o que fazer.

tags: linux, desinstalacao, apt, terminal, dpkg
