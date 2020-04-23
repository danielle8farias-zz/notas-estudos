# Etiquetas (tags) no Git

## Criando etiquetas

Etiquetas servem para melhor identificar os arquivos que estão sendo trabalhados. Para criar uma etiqueta usamos

```
$ git tag -a <etiqueta> -m "insira sua mensagem aqui"
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.
- substitua o \<etiqueta> pelo nome da sua etiqueta sem os sinais **<>**

Exemplo:

```
$ git tag -a v1.0 -m "versão 1.0"
```

![etiqueta no git](img/p0011-0.png)

Para verificar todas as etiquetas digite

```
$ git tag
```

E o retorno serão todas as etiquetas já criadas.

É importante notar que a etiqueta é criada no **commit** atual. Para criar uma etiqueta em um **commit** passado fazemos

```
$ git tag -a <etiqueta> <chave do commit> -m "insira sua mensagem aqui"
```

- substitua o \<chave do commit> pelo número da chave do **commit** desejado, sem os sinais **<>**

Exemplo:

```
$ git tag -a v0.1 c5d15de -m "versão beta"
```

Para verificar a **chave do commit** use o comando

```
$ git log --oneline
```

Para saber detalhes de uma etiqueta específica

```
$ git show <etiqueta>
```

## Usando etiquetas (tags) no Git

Para utilizar a etiqueta, usa-se o comando:

```
$ git checkout <etiqueta>
```

Desse modo é possível visualizar o projeto a partir do **commit** associado a essa etiqueta.

Para voltar ao estado original

```
$ git checkout <nome do ramo original>
```

Para excluir uma etiqueta, digite

```
$ git tag -d <etiqueta>
```

tags: git, tag, etiqueta, show
