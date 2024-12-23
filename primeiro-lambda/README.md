Passo a passo para subir a sua primeira função lambda via cli.

Contextualizando;

- Estou partindo do fato que você já tem na aws.
- Tem um user de IAM criado nessa conta.
- Tem o AWS-cli instalado e devidamente configurado para esse user.
- Esse é o pré-rec minimo para que você consiga executar esse tutorial.

O que será feito ?

Com os comando a seguir nós iremos, criar uma função lambda, que toda vez que cair 1 arquivo em um
s3, ela irá fazer a copia para um outro s3 criptografando o arquivo.

Vamos começar criando o nosso bucker que vai receber os arquivos;

$ aws --profile bueno  s3api create-bucket --bucket sourcebucket --region us-west-2 --create-bucket-configuration LocationConstraint=us-west-2

OBS; Terminar de alocar os comando aqui.
