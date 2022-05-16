# webapi-mezzio-unialfa

Projeto criado e desenvolvido na disciplina de API com PHP Unialfa

Dockerfile na raiz do projeto, para rodar o projeto, basta realizar os seguintes comandos:

Build:

docker build -t apibruno -f Dockerfile .

Subindo o container:

docker run -v ./:/var/www/ -p 8094:80 --rm --name testes2 apibruno