# PROJETO INICIATIVA DEVOPS
> Nesse projeto é criado uma imagem Docker e publicado no dockerhub.

Passos:
1) Montar o Dockerfile com as especificações desejadas;
2) Construir a imagem a partir do Dockerfile:
`docker build -t thalesteo/conversao-temperatura:v1 .`
3) Subindo a aplicação no localhost:
`docker container run -d -p 8080:8080 thalesteo/conversao-temperatura:v1` 
4) Listando as minhas imagens: `docker image ls`
5) Autenticar no dockerhub: `docker login`
6) Enviar a imagem para o dockerhub: `docker push thalesteo/conversao-temperatura:v1`
7) Subindo a versão latest: `docker tag thalesteo/conversao-temperatura:v1 thalesteo/conversao-temperatura:latest`
8) Enviando a imagem versão latest: `docker push thalesteo/conversao-temperatura:latest`