# snake-game-js
Clássico jogo da cobrinha (bem simples) em JavaScript.
<img src="sprite-snake.jpg" alt="drawing" width="50"/>


<!-- ## Rodando localmente 1 (apenas para alunos usando o computador)
Você pode rodar o jogo abrindo o arquivo [_views/pages/jogo.html_](views/pages/jogo.html) com o seu navegador.

```sh
$ git clone https://github.com/ifal-riolargo/snake-game-js.git # clone a aplicação para sua máquina local (ou faça antes um fork e clone do seu próprio repositório)
$ cd snake-game-js
$ firefox views/pages/jogo.html # ou use outro navegador ex. google-chrome 
```

---- -->

## Rodando localmente 
O jogo usa a infraestrutura do Node.js para publicação no Heroku. Por este motivo, você pode rodar um servidor localmente e executar o jogo.

Antes, você precisa ter o [Node.js](http://nodejs.org/) e o [NPM](https://www.npmjs.com/) instalados.
<br><br>
Para quem for usar o Termux, instale com o comando abaixo.
```sh 
$ pkg install nodejs
```

Para quem usa Ubuntu, use os comandos abaixo.
```sh 
$ sudo apt update
$ sudo apt install nodejs
$ sudo apt install npm
```
<br>
Agora execute.

```sh
$ node --version # verificar versão do node
$ npm --version # verificar versão do NPM
$ git --version # verificar versão do GIT
$ git clone https://github.com/<SEU USUARIO DO GITHUB>/snake-game-js.git 
$ cd snake-game-js
$ npm install
$ npm start
```

Pronto. Sua aplicação deve executar em [localhost:5000](http://localhost:5000/).
Para finalizar o servidor web, no terminal, aperte CTRL+C.

----

## Deploying no Heroku (opção 1)


Agora você pode fazer deploy da suaplicação no Heroku.
Após fazer o cadastro no site [https://www.heroku.com/](https://www.heroku.com/), você deve acessar o gerenciador de aplicações da sua conta no Heroku através do endereço (https://dashboard.heroku.com/apps)[https://dashboard.heroku.com/apps]. 
Clique no botão _Create new app_. 
No campo App name coloque _snake-game-js_ (caso o nome não esteja disponível, coloque -01 no final do nome), em região deixe a opção United States e depois clique no botão Create app.

Na próxima página, na opção _Deploy/Deployment Method_, clique em Github Connect To Github.
Agora clique no botão que apareceu _Connect to Github_, digite seu login e sua senha do Github e autorize acesso ao seu perfil.
Clique no botão _Search_ para localizar os repositórios do seu perfil e selecione _snake-game-js_. Para finalizar clique em _Connect_. 
Uma nova opção vai abrir na tela (_Automatic Deploys_). 
Clique no botão _Enable Automatic Deploys_.
Isso permite que o Heroku atualize para uma nova versão sempre que você fizer um novo _git push_ no seu repositório no Github.
Para finalizar clique no botão _Deploy Branch_

Se tudo ocorreu corretamente, suba a página para o início e clique no botão _Open app_ (no canto superior direito). Pronto! Sua aplicação está em produção, executando em um servidor na nuvem. Agora você pode copiar o endereço da sua aplicação e compartilhar com seus amigos.



## Deploying no Heroku (opção 2 - apenas para quem está no WSL/Ubuntu)
Uma segunda forma de fazer deploy no Heroku é usando o Heroku CLI. 
O Heroku CLI que vai ajudar a gerenciar e dimensionar seus aplicativos, provisionar complementos, visualizar seus logs de aplicativo e executar seu aplicativo localmente. 
Instale o Heroku CLI com o comando abaixo (você precisa ter o snap instalado na sua máquina)

```sh
$ sudo snap install heroku --classic 
```

```sh
$ heroku login # isso deve abrir o navegador e pedir para você entrar com seu login e senha no Heroku
$ heroku create #cria um repo remoto em heroku.com e aponta o seu repo local para lá 
$ git push heroku main #envia sua aplicação para o heroku
$ heroku open #abre o navegador na sua aplicação, executando em um servidor na nuvem
```

Pronto. Você verá sua aplicação executando em um servidor na nuvem. Basta copiar o link do navegador e você poderá mostrar sua aplicação para seus amigos.

<!-- or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy) -->

----

## Importante

Para mais informações sobre como usar Node.js no Heroku, veja a documentação oficial (em inglês):

- [Getting Started on Heroku with Node.js](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Best Practices for Node.js Development](https://devcenter.heroku.com/articles/node-best-practices)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)
