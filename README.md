# docker-mongodb
Comando para criação de um container com banco de dados MYSQL com o uso do docker

docker container run --name desafio03 -d -p 27017:27017  -e MONGO_INITDB_ROOT_USERNAME=mongo_usr -e MONGO_INITDB_ROOT_PASSWORD=mongo_pwd -e MONGO_INITDB_DATABASE=mongodb mongo

docker container run <-- é usado para criação de um container em cima de uma imagem 
--name NOME <-- é usado para escolher o nome do container o nome dele ser colocado logo em seguida 
-d <-- mostra para o Deamon que o container é um teste e deve ser continuo 
-p 5000:5400 <-- é para escolher a porta de saido do container 5000: é a porta e 5400 é a subporta (Modificado somente para o exemplo) 
-e <-- é usado para podermos adicionar as variaveis da imagem e devem sempre estar antes da variavel 
mongo <-- e o nome da imagem e sempre deve estar no final. 
-e MONGO_INITDB_DATABASE=NOMEDOBANCO 
-e MONGO_INITDB_ROOT_USERNAME=NOMEDOUSUARIO 
-e MONGO_INITDB_ROOT_PASSWORD=SENHADOBANCO
