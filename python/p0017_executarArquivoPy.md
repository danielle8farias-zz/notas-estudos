# Executando arquivos/script do Python no Linux

Para executar um arquivo com a extensão **.py (script Python)**, podemos chamá-lo através do terminal junto ao nome do arquivo. Exemplo:

```
$ python3.7 nome_do_arquivo.py
```

No meu caso, estou usando o **Python 3.7**, mas se você estiver usando outro, basta mudar o nome.

Para saber qual versão do Python está na sua máquina

```
$ python3 -V
```

Outra maneira é utilizando uma **shebang** no seu arquivo. Desse modo o interpretador é acionado ao chamar o arquivo pelo terminal ou mesmo pela interface gráfica.

Para usar a shebang, adicione na primeira linha do seu arquivo

```py
#!/usr/bin/env python3.7
```

Ou

```py
#!/usr/bin/env python3
```

O **#!** é a shebang propriamente dita, o **/usr/bin** é o endereço absoluto (nome completo de todos os diretórios desde a raiz até o arquivo desejado). O **env** é um comando do Linux que, aqui, serve encontrar o interpretador sem definir seu caminho exato.

Antes de executar é preciso dar as permissões através do comando no terminal

```
$ chmod a-x nome_do_arquivo.py
```

O **chmod** vem de _change mode_ que é quem vai fazer as mudanças, o **a-x** significa _for **a**ll users, remove (**-**) the e*x*ecute permission_, ou seja, remova as permissões de execução para todos os usuários.

Para chamar o arquivo digite no terminal

```
$ ./nome_do_arquivo.py
```

tags: python, linux, shebang
