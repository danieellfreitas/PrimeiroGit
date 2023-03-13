Como instalar o Git em seu computador
Para instalar o Git no Windows você pode entrar no site oficial e fazer o download do arquivo de instalação. Verifique se o seu sistema operacional é 32 ou 64 bit e baixe a versão correspondente. A instalação é bem simples basta seguir o passo a passo do instalador.

Para você que usa Linux ou Mac, recomendo fazer direto do terminal que é bem mais fácil e rápido, basta digitar os seguintes comandos e aguardar.

Linux:


sudo apt update && sudo apt install git
Mac:


brew install git
Como configurar o Git
Para configurar o Git é necessário abrir o terminal e se você estiver no Windows pode procurar pelo Git Bash na barra de pesquisa do sistema.

Com o terminal aberto, basicamente existem duas coisa que você precisa configurar que é o seu nome de usuário e o e-mail. Então digite os seguintes comandos no terminal:

Para configurar o nome de usuário no Git:


git config --global user.name "Seu nome aqui"
Para configurar o e-mail de usuário no Git:


git config --global user.email seuemail@email.com
Pronto! Só isso e o seu Git já está configurado e pronto para usar. Fácil não é mesmo?

Como abrir o Git dentro do VSCode
Usar o Git dentro do VSCode facilita muito no dia-a-dia de desenvolvimento e para configurar isso siga o passo a passo:

Abra o VSCode e entre no menu Arquivos -> preferencias -> Configurações ou no atalho (CTRL + ,).

No canto superior direto do VSCode clique no o ícone Abrir configurações (JSON) e cole o código abaixo:


"terminal.integrated.defaultProfile.windows": "Git Bash",

"terminal.integrated.tabs.enabled": true,
Para que funcione corretamente não esqueça das vírgulas!

Agora basta usar os atalhos (CTRL + SHIFT + ') ou (CTRL + J) para abrir o terminal.




Usando o Git


Primeiro, entre no seu Terminal e navegue até o diretório do seu projeto e inicie o GIT com o comando git init.

Terminal
git init
Se tudo der certo, será retornado algo como:
Initialized empty Git repository in /diretorio/.git/

Configurando seu usuário
Agora temos que configurar nosso usuário colocando nome e e-mail com os comandos abaixo:

Terminal
git config --global user.name "João Rodrigues"
git config --global user.email joao@ajudadoprogramador.com.br
Lembre de mudar seu nome e e-mail antes de executar os comandos acima.

Essa configuração precisa ser feita apenas uma vez já que foi passado a opção --global Caso queira usar um nome e e-mail diferente em um projeto, faça o processo sem a opção --global.

Terminal
git config user.name "João Rodrigues"
git config user.email joao@ajudadoprogramador.com.br
Configurando seu editor
Sempre que é preciso utilizar um editor, o GIT usará o padrão do sistema Geralmente este editor é o Vi, Vim ou Nano, dependendo do seu OS. Para mudar o editor padrão, basta executar o seguinte:

Terminal
git config --global core.editor nomedoeditor
Configurando ferramenta de Diff
Caso queira mudar a ferramenta padrão para resolver os conflitos, basta executar o seguinte:

Terminal
git config --global merge.tool nomedaferramenta
Por padrão, o git aceita as ferramentas kdiff3, tkdiff, meld, xxdiff, emerge, vimdiff, gvimdiff, ecmerge e opendiff.

Lista de configurações
Para listar as suas configurações, execute o seguinte:

Terminal
git config --list
Pronto pequeno Padawan! Seu git está configurado e pronto para você errar milhares de vezes antes de aprender a usá-lo ele de forma correta. ;)

Quer aprender tudo sobre o GIT? Clique aqui e veja todos os artigos.