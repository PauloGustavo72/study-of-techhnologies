# Docker
## Prazo: 27/05/2023

Docker é um sistema criado primeiramente no linux e então adaptado para os demais S.O que visa facilitar a criação de containers. 

Containers são parecidos com uma máquina virtual, porém usando muito menos recurso da máquina física. 


### Instalação
Basta [seguir a documentação](https://docs.docker.com/desktop/install/windows-install/)


### Dockerfile
Dockerfile é o arquivo base para criar sua própria imagem.

Esse nome é também uma extensão de arquivo, então é possível criar mais de um arquivos dockerfile dentro da mesma pasta, algo como `arquivo1.Dockerfile` e `arquivo2.Dockerfile`


### Quais são os comandos usados no dockerfile

- [documentação da rockeatseat](https://blog.rocketseat.com.br/dockerfile-principais-comandos-para-criar-a-receita-da-imagem/)


### Qual comando usado para fazer o build do dockerfile
`docker build -t {image_name} -p {host_port}:{docker:port} -v host:docker {dockerfile_path}`



### Exemplo de dockerfile para spring
Here

### Como funciona a parte de login no dockerhub ? 
Para logar desde um terminar e ser possível baixar suas imagens privadas, ou mesmo atualizar alguma imagem privada, deve-se usar o seguiinte comando:

```docker login --username={user_name} --email={email}```

### Como fazer push, get e update de imagen para o dockerhub ?
Uma vez que esteja logado via terminal, para buscar uma imagen privada usar o comando:
`docker image pull {image_name}`

e caso queira criar uma nova versão da imagen, se usa os comandos:
* `docker build -t <your-docker-hub-id>/{image_name}:v1 .`
* `docker push <your-docker-hub-id>/{image_name}:v1`






## Comandos

* `docker ps` -> lista todos os containers ativos
* `docker ps -a` -> lista todos os containers existentes na máquina

* `docker images` -> lista todas as imagens da máquina