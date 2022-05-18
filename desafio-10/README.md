#  Desafio 10

Bancos de dados são uma parte fundamental de um sistema distribuído. Eles podem ser SQL ou NoSQL. Neste desafio, vamos trabalhar com um banco relacional (SQL) e criar alguns níveis de permissionamento.

## Atividade 1

Criar um código utilizando Ansible e Terraform ou CloudFormation para instalar uma base de dados e criar seus usuários.

## Critérios de aceite / sucesso

* Instalar um banco MySQL (escolher a distribuição que achar melhor para o SO que utilizar)
* Criar uma base de dados chamada `aplicacao` e outra chamada `logs`

* Criar no banco os usuários abaixo com seus respectivos níveis de acesso:

| usuario | acesso |
|:---------:|:--------:|
| app | leitura em todas as tabelas |
| api | Criação em todoas as tabelas |
| convidado | leitura nas tabelas da aplicacao |

* Documentação do que foi realizado e justificativa das escolhas

## Referências

MySQL: https://www.mysql.com/

