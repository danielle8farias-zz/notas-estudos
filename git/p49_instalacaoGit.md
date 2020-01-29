# Instalando e configurando o Git no Linux

Para instalar o Git no Linux, digite:
```
$ sudo apt install git
```

Verifique se a instalação foi feita corretamente digitando:
```
$ git --version
```
Você receberá o retorno da versão instalada.

Antes de começar a usá-lo é preciso fazer as configurações iniciais.
```
$ git config --global user.name <seu nome>
```
Digite seu nome sem os sinais de < e >.

Em seguida:
```
$ git config --global user.email <seu@email.com>
```
Digite seu email sem os sinais de < e >.

Configurando o editor padrão:
```
$ git config --global core.editor nano
```
No meu caso, estou usando o **nano**.

Para verificar as suas configurações:
```
$ git config --list
```

tags: git, linux, configuracao, instalacao
