# Verificando modificações no repositório

Para saber o que foi modificado em um arquivo do repositório, mas que ainda não foi adicionado usamos o comando:
```
$ git diff
```

Exemplo:
Supondo que fiz uma alteração no arquivo readme, cujo conteúdo anterior era o texto abaixo:

*Finite but unbounded hearts of the stars brain is the seed of intelligence rogue rich in mystery are creatures of the cosmos.*

Assim, ao digitar o comando **diff**, temos:
```
diff --git a/readme b/readme
index 3b2cf57..e35008a 100644
--- a/readme
+++ b/readme
@@ -1 +1,4 @@
 Finite but unbounded hearts of the stars brain is the seed of intelligence rogue rich in mystery are creatures of the cosmos.
+
+Adipisci velit stirred by starlight consectetur sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt with pretty stories for which there's little good evidence from which we spring and billions upon billions upon billions upon billions upon billions upon billions upon billions.
+
```
Assim podemos ver que partes do arquivo foram modificadas.

Para verificar os arquivos que estão no index, usamos o comando:
```
$ git diff --staged
```

Para verificar todos os commit feitos, usamos
```
$ git log
```
O retorno será o histórico de todos os commits e uma chave para cada um deles. É atraves dessa chave que fazemos a transição entre as versões do arquivo/projeto.

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
