# Ignorando arquivos no Git

Para arquivos dentro do diretório, os quais você não quer incluí-los no repositório, precisamos criar o seguinte arquivo:
```
$ touch .gitignore
```
Abrindo esse arquivo, vamos digitar dentro dele o que queremos deixar de fora do repositório. Exemplo:

Ocultando do git uma pasta e um diretório. Temos

![git ignore](./img/gitignore.png)

Assim temos uma pasta como primeiro item, pois ela termina com a barra.

No terceiro item estamos adicionando na lista qualquer arquivo que termine com a extensão **txt**.

É importante notas que devemos informar um tipo de arquivo por linha.

Dentro do diretório, temos:
```
$ ls
changelog  readme  secreto/  secreto1  secreto2.txt
```

Quando verificamos o estado do git teremos:
```
No ramo master
Arquivos não monitorados:
  (utilize "git add <arquivo>..." para incluir o que será submetido)

	.gitignore

nada adicionado ao envio mas arquivos não registrados estão presentes (use "git add" to registrar)
```

![arquivos ignorados pelo git](./img/fluxoGit8.png)

Os arquivos descritos dentro do arquivo .gitignore não aparece no estado atual do Git.

tags: git, ignore, diretorio, arquivo
