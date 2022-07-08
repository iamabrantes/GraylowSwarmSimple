# Criação de cluster swarm para utilização do graylog
Pata utilizar o mesmo altere o nome das variáveis em example.env de acordo com:

GRAYLOG_PASSWORD_SECRET=testando4linux123 #SenhaDoUsuarioAdmin
GRAYLOG_ROOT_PASSWORD_SHA2=8b06a9887ea5058d703e17d895432c8e7a078a29591240afe6275fe4dd098a5c #SenhaDoUsuarioAdminEmSha2

Para gerar o sha2 da senha usar o comando em um terminal:

echo -n (senha) | shasum -a 256
