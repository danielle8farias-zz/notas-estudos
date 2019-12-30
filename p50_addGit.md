# Adicionando arquivos no Git

Entre na pasta a qual você pretende fazer o versionamento e no terminal digite:
```
$ git init
```
Desse modo a pasta **.git** será criada. É essa pasta que armazenará as imagens das versões do projetos criados.

Para saber o estado atual do git, basta digitar:
```
$ git status
```
No nosso caso será
```
No ramo master
No commits yet

nada para enviar (crie/copie arquivos e use "git add" para registrar)
```

![fluxo inicial do git](./img/fluxoGit1.png)

Vamos criar alguns arquivos para teste:
```
$ touch arquivo1 arquivo2
```
Digitando novamente o git status, temos:
```
No ramo master
No commits yet

Arquivos não monitorados:
  (utilize "git add <arquivo>..." para incluir o que será submetido)

	arquivo1
	arquivo2

nada adicionado ao envio mas arquivos não registrados estão presentes (use "git add" to registrar)
```

![working directory com dois arquivos](./img/fluxoGit2.png)

Para adicionar os dois arquivos
```
$ git add arquivo1
$ git add arquivo2
```
Ou
```
$ git add arquivo1 arquivo2
```

Para adicionar todos os arquivos do diretório
```
$ git add .
```

Para adicionar todos os arquivos de uma determinada extensão
```
$ git add *.txt
```

Verificando o estado do git, temos
```
No ramo master
No commits yet

Mudanças a serem submetidas:
  (utilize "git rm --cached <arquivo>..." para não apresentar)

	new file:   arquivo1
	new file:   arquivo2
```
Aqui, estamos no index (staging area). Algo como uma sala de espera do git.

![arquivos no index](./img/fluxoGit3.png)

tags: git, init, add, status
