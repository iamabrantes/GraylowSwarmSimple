# Criação de cluster swarm para utilização do graylog
O cluster consiste em 4 containers, sendo:

1-MongoDB
2-Elasticsearch
3-grayloggeral(tratador dos logs)
4-graylogmaster(Interface web)

Pata utilizar o mesmo altere o nome das variáveis em example.env de acordo com:

GRAYLOG_PASSWORD_SECRET=testando4linux123 #SenhaDoUsuarioAdmin
GRAYLOG_ROOT_PASSWORD_SHA2=8b06a9887ea5058d703e17d895432c8e7a078a29591240afe6275fe4dd098a5c #SenhaDoUsuarioAdminEmSha2

Para gerar o sha2 da senha usar o comando em um terminal:

echo -n (senha) | shasum -a 256

Alterar também a linha 64 apontando o endereço do seu cluster swarm
