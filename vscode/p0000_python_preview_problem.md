# Erro ao usar a extensão Python Preview do VSCode

- [Página da extensão no Marketplace.](https://marketplace.visualstudio.com/items?itemName=dongli.python-preview)

- [Repositório da extensão no GitHub.](https://github.com/dongli0x00/python-preview)


## Descrição do problema

Extensão rodava apenas com Python 2. Não conseguia achar o caminho da variável de ambiente.

# Solução

Com a extensão instalada e o VSCode fechado ir até o diretório:

```
$ .vscode/extensions/dongli.python-preview-0.0.4/out/debugger/debugClients/
```

E editar o arquivo

```
$ nano localDebugClient.js
```

Na linha 68 ou procure por

```
let pythonPath = 'python'
```

e mude para

```
let pythonPath = 'python3'
```

Salve o arquivo e saia do editor.

Agora vamos para outro diretório:

```
$ cd .vscode/extensions/dongli.python-preview-0.0.4/out/features
```

Abrir o arquivo

```
$ nano previewManager.js
```

procure pela linha 54 ou por

```
pythonPath: 'python'
```

e mude para

```
pythonPath: 'python3'
```

Salve o arquivo e saia do editor.

> CTRL + _ (ctrl + shift + sinal de menos) para buscar por uma determinada linha no Nano.

tags: vscode, python, preview, extensão
