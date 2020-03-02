# Instalando o Python 3.8 e o IDLE

Antes de começar a instalação propriamente dita, é necessário verificar se o sistema possui algumas bibliotecas que nos ajudarão a compilar o código fonte do Python. Assim, digite:

```
$ sudo apt install build-essential checkinstall
```

**sudo** serve para pedir permissões de administrador temporariamente.

**apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

**install** é o comando de instalar, indicando ao apt o que fazer.

E também

```
$ sudo apt install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev zlib1g-dev
```

Entre no diretório **opt**

```
$ cd /opt
```

Esse diretório existe para abrigar pacotes de software opcionais e que, quando instalados, não causem incompatibilidade com outros programas mais antigos (no caso, outras versões do Python).

Em seguida fazemos download do arquivo

```
$ sudo wget https://www.python.org/ftp/python/3.8.2/Python-3.8.2.tar.xz
```
>para verificar a versão mais recente, visite o site [python.org](https://www.python.org/downloads/).

Agora, vamos extrair o arquivo com o comando

```
$ tar -xvf Python-3.8.2.tar.xz
```

O **tar** é um software que permite unir dois ou mais arquivos em um. Ele é usado como um complemento para o compactador, mas não é o compactador.

Os parâmetros **x** é o que extrai os arquivos, o **v** exibe os detalhes dessa operação e o **f** especifica o arquivo que será usado; seguido do nome do arquivo.

Entramos na pasta recém criada

```
$ cd Python-3.8.2
```

e com o comando

```
$ sudo ./configure --enable-optimizations
```

Aqui usamos a flag **--enable-optimizations** para otimizar a compilação.

Fazendo a compilação

```
$ sudo make altinstall
```

O comando **make** serve determinar automaticamente quais partes de um programa grande precisam ser recompiladas e emitir os comandos necessários para recompilá-las.

O **altinstall** é usado para impedir que o programa compilado tome o lugar padrão do arquivo binário python em /usr/bin/python.

Verficando se a instalação foi feita corretamente:

```
$ python3.8 -V
```

Agora podemos voltar para o diretório **opt**

```
$ cd /opt
```

E remover o arquivo baixado

```
$ sudo rm -f Python-3.8.2.tar.xz
```

**rm** é o comando para deletar arquivos e diretórios.

**-f**  exclui arquivos somente leitura imediatamente, sem qualquer confirmação.

## Instalando o IDLE

No terminal, digite

```
$ sudo apt install idle-python3.8
```

tags: python, instalacao, idle, linux
