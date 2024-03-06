# Configuração do Ambiente de Desenvolvimento e Emulador
# Chocolatey

O Chocolatey ou Choco é um gerenciador de pacotes do Windows ao qual permite o usuário da maquina instalar ferramentas, aplicações, gerancimanto e atualizações diretamente pelo `terminal`.

Verifique suas permissões com o comando:

`Get-ExecutionPolicy`

Se aparecer a mensagem "Restricted" (Restrito), execute o comando abaixo, caso contrário, pule para o próximo comando:

`Set-ExecutionPolicy AllSigned`

Instalaremos o chocolatey com o seguinte comando:

`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

Teste se a instalação foi bem sucedida com o comando:

`choco`

Agora, feche e abra o seu powershell. Para instalar o Node.JS e o SDK 11 ou o recomendado para sua maquina conforme as atualizações por parte do Node.js, faremos no terminal:

`choco install -y nodejs-lts openjdk11 `

Novamente, reinicie o terminal, fechando e abrindo ele. Rode os comandos abaixo para conferir a instalação:

`node -v` para verificar a versão, caso esteja desatualizado, baixar a versão mais nova no site.

[Clique aqui para acessar o site do Node.js ](https://nodejs.org/en)

# Instalação do Node.js e npm

`npm install -g npm@VERSÃOMAISNOVA!!` para BAIXAR

## Instalando pacotes com NPM

O NPM é o gerenciador de pacotes do Node que vem junto em sua instalação. Para verificar a versão do NPM instalada, você pode executar o seguinte comando:

`npm --version`

Para dar início a nossa primeira aplicação, vamos abrir um novo terminal e executar os seguintes comandos:

`mkdir nodeapp` + `cd nodeapp` + `npm init`

Todas as vezes em que inicia um projeto utilizando o VITE ou baixando um arquivo em ZIP ou RAR, é necessário utilizar o comando: 

`npm install` para baixar o NODE_MODULES


# Emuladores

### Snack Expo

Para visualização em React Native Criada pela Expo para incorporar e executar projetos React Native e compartilhar como eles são renderizados em plataformas como Android e iOS

### Expo Go

O aplicativo Expo Go é uma ótima ferramenta para começar – ele existe para ajudar os desenvolvedores a lançar projetos rapidamente, experimentar ideias (como no Snack).

### Android Studio
Depois de baixarmos o Android Studio, vamos ver passo a passo como executar nosso emulador Android ou IOS. O desenvolvedor pode utilizar também seu smartphone para visualizar a produção de sua interface, basta abrir o aplicativo apontar a camêra do smartphone para o qrcode que é gerado para leitura.

### Passos Android Studio no Computador

Execute o Android Studio e, na parte inferior direita do aplicativo, `selecione “Configure” e depois clique em “AVD Manager”`. Será mostrada uma tela com os emuladores instalados. Talvez já apareça um emulador configurado, se na hora da instalação você tiver selecionado `“Android Virtual Device” ` - nessa situação, aperte no ícone de play (em formato de triângulo) para rodar o emulador. Caso não apareça um emulador, vamos configurar um agora mesmo!

`Clique em “Create Virtual Device”.`

Escolha o dispositivo que deseja ter como emulador e clique em “Next” (Próximo).

Agora, você precisa escolher a imagem do dispositivo. É bom escolher e baixar a versão recomendada pelo Android Studio, ou uma versão de API mais recente (28 ou superior) que são x86. Depois de baixar, o que pode levar um tempo, selecione a imagem baixada e clique em “Next” (Próximo).

Será exibida uma tela de configurações do seu emulador. No campo AVD Name, coloque um nome que preferir para seu emulador.

Clique em “Finish” (Finalizar).

Seu emulador deve estar sendo exibido na lista. Basta clicar no ícone de play para executá-lo. Lembramos que esse processo pode demorar pela primeira vez.

**Terminal 1**

`npm start`

**Terminal 2**

`npx react-native run-android`

### Passos Android Studio no Celular

Conecte seu dispositivo via USB no computador.
Ele precisa estar com o modo Depuração USB habilitado.
Caso ainda não esteja, vamos habilitar a opção de Desenvolvedor.
  1. Entre nas configurações do aparelho.
  2. Vá para Sistema ou Sobre o telefone.
  3. Caso sua tela anterior tenha sido Sistema, clique na opção Sobre. Agora, se sua tela anterior já era o Sobre, siga para o próximo passo.
  4. Clique em Informações do software.
  5. Nessa tela aberta, clique repetidamente na opção Número da versão ou em Número de compilação até ele te tornar um desenvolvedor.
  6. Pronto, agora você tem a opção desenvolvedor ativada.
Pronto! Com a opção Depuração USB ativada, podemos usar o dispositivo físico!

Agora, **com o seu aparelho conectado no cabo USB no computador**, abra o terminal e digite:

` adb devices `

Agora, para executar o aplicativo no seu celular, **é necessário que você já tenha criado um projeto React Native**. Se não tiver criado ainda, basta executar essa linha de comando no terminal (antes, navegue até a pasta do seu computador que deseje salvar o projeto):

` npx react-native init nomedoapp `

Agora, serão necessários dois terminais abertos dentro da pasta do projeto criado. No terminal 1, digite:

` npm start `

No terminal 2, digite:

`npx react-native run-android`

Será carregado o aplicativo para o seu celular e você poderá testá-lo enquanto programa.
