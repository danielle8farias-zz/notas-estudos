# Terminal: Removendo programas obsoletos


Digite no terminal:

```
$ sudo apt autoremove
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

- **autoremove** remove versões antigas de programas já atualizados.

É importante frisar que as versões antigas do kernel também serão removidas com esse comando e, caso você tenha algum problema com o kernel atual, e deseje voltar ao kernel antigo, não será mais possível.

tags: linux, terminal, autoremove
