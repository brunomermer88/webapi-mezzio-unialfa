# webapi-mezzio-unialfa

Projeto criado e desenvolvido na disciplina de API com PHP Unialfa

Dockerfile na raiz do projeto, para rodar o projeto, basta realizar os seguintes comandos:

Build:

docker build -t apibruno -f Dockerfile .

Subindo o container:

docker run -v ./:/var/www/ -p 8094:80 --rm --name testes2 apibruno

Para testes da api em Ubuntu:

Instalando o prism: curl -L https://raw.githack.com/stoplightio/prism/master/install | sh

Rodandando o prism: prism mock openapi.json / http get http://127.0.0.1:4010/acesso

Instalando as dependencias para o nmp, e redoc-cli:

sudo apt-get install -y libssl1.0-dev
sudo apt-get install -y nodejs-dev
sudo apt-get install -y node-gyp
sudo apt-get install -y npm
sudo npm install redoc-cli -g
