# Bem vindo ao desafio 3

Agora já temos um CMDB, com toda a configuração do nosso webserver, vamos automatizar a criação do ambiente como um todo.

## Atividade

Vamos criar uma AMI nossa com todas as configurações do nosso webserver já aplicadas nela e subir esse ambiente de forma automatizada.


## Critérios de aceite / sucesso

Criação de uma AMI, utilizando packer que utilize o playbook do desafio 2 como base

Criação de um script terraform para o provisionamento dos itens abaixo:

1. Criar a instância
2. configurar os dns
3. Ajustar o security group
4. As aplicações do webserver devem estar acessíveis depois da execução do terraform
5. O terraform precisa utilizar a AMI criada por você com o packer

## Referências

Packer: https://www.packer.io/

Terraform: https://www.terraform.io/ 

IAAS WEEK packer: https://youtu.be/WGKjdlcShaM

IAAS WEEK terraform:  https://youtu.be/8mRZJcCgoS0
