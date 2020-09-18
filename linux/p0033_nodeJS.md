# Instalando o Node.JS e o Node Version Manager (NVM) no Linux (Ubuntu e derivados)

Antes de começarmos a instalação, precisamos atualizar o sistema.

> [saiba como atualizar seu Linux aqui.](p0005_update.md)

Em seguida, vamos instalar as bibliotecas de desenvolvimento, com o comando:

```
$ sudo apt install build-essential libssl-dev
```

- **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- **sudo** serve para pedir permissões de administrador temporariamente.

- **apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

- **install** é o comando de instalar, indicando ao apt o que fazer.

- **build-essential** é uma biblioteca que reúne diversas aplicações para compilar e instalar outros programas, que inclui, por exemplo, o make, automake, etc.

- **libssl-dev** é uma biblioteca com arquivos para desenvolvimento.

Agora faremos a instalação do **NVM** que permitirá a instalação de várias versões do Node e nos permitirá alternar entre elas, caso necessário:

```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

- **curl** é uma ferramenta em linha de comando para transferência de dados com sintaxe URL.

- O parâmetro **-o-** indica que a saída do arquivo terá seu nome mantido (sem modificações).

- **https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh** é o endereço de onde está o script que queremos baixar.

- **|**, conhecido como **pipe** (tubo), que faz o encadeamento de processos. Ele permite conectar a saída padrão de um comando à entrada padrão de outro.

- **bash** é um interpretador de comandos. É ele quem vai rodar o script que baixamos.

> O número da versão pode mudar com o tempo. Acesse a página do [projeto no GitHub (clique aqui)](https://github.com/creationix/nvm) e procure pela versão mais recente, caso seja necessário.

Após a instalação do script acima, feche o terminal e abra um novo.

Execute o comando

```
$ nvm ls-remote
```

Ele vai exibir várias versões do Node e assim sabermos se o **NVM** está funcionando corretamente.

Escolha uma versão para instalar. Por exemplo:

```
$ nvm install v14.11.0
```

Caso você instale mais de uma versão e no futuro tenha necessidade de alternar entre elas utilize o comando:

```
$ nvm use <número da versão>
```

Verifique a versão do Node que foi instalada com o comando:

```
$ node -v
```

tags: nvm, node, javascript
