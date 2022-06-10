# Curso de Docker

### Comandos

- Criar uma imagem ubuntu interativo e executar comandos

  - docker run -it ubuntu

- Remover o container após finalizar

  - docker run -it --rm ubuntu

- Removendo container

  - docker rm id/nome do container

- Fazer a ponte entre porta do docker

  - docker run -d -p 8080:80

- Iniciar um container

  - docker start id/nome

- Para o container

  - docker stop id/nome

- Dar nome ao container

  - docker run --name xptop

- Entrar no container

  - docker exec -t id/nome bash

- Criar um volume (bind mounts)

  - docker run -d -v /home/thomas/:/usr/share/nginx/html nginx

- Criar um volume mount

  - $(pwd) pega o local da pasta
  - docker run -d --name nginx -p 8080:80 --mount type=bind,souce="$(pwd)"/html,target=/usr/share/nging/html

- Verificar os volumes existentes

  - docker volume ls

- Removendo uma lista de container

  - docker rm $(docker ps -a -q) -f

### Comandos Imagem

- Criar uma imagem
  - docker build -t nome/nginx-com-vim:latest . (pasta que esta)

### Dockerfile

- Comando CMD

  - CMD ["echo","Hello world"]
  - docker run nginx echo "oi"

- Comando fixo e variavel

  - ENTRYPOINT ["echo","Hello"]

  ### Adendo

  - Comando no arquivo para poder aceitar o que adicionar após
    - exec "$@"
