# git diff: Verificando modificações no repositório

Para saber o que foi modificado em um arquivo do repositório, mas que ainda não foi adicionado, usamos o comando:

```
$ git diff
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

Exemplo:
Supondo que fiz uma alteração no arquivo readme, cujo conteúdo anterior era o texto abaixo:

![texto 1](img/p0008-0.png)

Adicionamos mais um trecho, ficando o arquivo assim

![texto 2](img/p0008-1.png)

Assim, ao digitar o comando **diff**, temos:

![git diff](img/p0008-2.png)

Assim podemos ver (na cor verde) quais partes do arquivo foram modificadas.

Para verificar as mudanças dos arquivos que estão no **index**, usamos o comando:

```
$ git diff --staged
```

Para verificar todos os commit feitos, usamos

```
$ git log
```

O retorno será o histórico de todos os **commits**, do último ao primeiro, e uma **chave** para cada um deles, em amarelo (mostarda). É através dessa **chave** que fazemos a transição entre as versões do arquivo/projeto.

![git log](img/p0008-3.png)

O comando

```
$ git log -p
```

faz a junção dos comandos **log** e **diff**. Pressione ENTER para descer a página e ao chegar ao fim, pressione **q**.

Com o comando

```
$ git log -p -<n>
```

sendo o **\<n>** o número de commits que gostaria de ver, a partir do último.

tags: git, diff, staged, log
