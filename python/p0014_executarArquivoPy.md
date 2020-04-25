# Executando arquivos/script do Python no Linux

Para executar um arquivo com a extensão **.py (script Python)**, podemos chamá-lo através do terminal junto ao nome do arquivo. Exemplo:

```
$ python3.8 nome_do_arquivo.py
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

No meu caso, estou usando o **Python 3.8**, mas se você estiver usando outro, basta mudar o nome.

Para saber qual versão do Python 3 está na sua máquina

```
$ python3 -V
```

Caso não tenha nenhuma versão do Python 3, eu ensino a fazer a instalação do [Python3.8 aqui](../linux/p0013_instalandoPython3.8.md).

Outra maneira  de executar um **script Python** é utilizando uma **shebang** no seu arquivo. Desse modo o interpretador é acionado ao chamar o arquivo pelo terminal ou mesmo pela interface gráfica.

Para usar a shebang, adicione na primeira linha do seu arquivo

```py
#!/usr/bin/env python3.8
```

Ou

```py
#!/usr/bin/env python3
```

- o **#!** é a shebang propriamente dita;
- o **/usr/bin** é o endereço absoluto (nome completo de todos os diretórios desde a raiz até o arquivo desejado);
- o **env** é um comando do Linux que, aqui, serve encontrar o interpretador sem definir seu caminho exato.

Antes de executar é preciso dar as permissões ao arquivo através do comando no terminal

```
$ chmod a+x nome_do_arquivo.py
```

- **chmod** vem de _change mode_ que é quem vai fazer as mudanças;
- o **a+x** significa _for **a**ll users, remove the e**x**ecute permission_, ou seja, remova as permissões de execução para todos os usuários.

Para chamar o arquivo digite no terminal

```
$ ./nome_do_arquivo.py
```

- O **ponto-barra** juntos serve para indicar o caminho do executável;
- o **ponto** significa diretório atual;
- a **barra** serve para separar o diretório do nome do arquivo

tags: python, linux, shebang, terminal
