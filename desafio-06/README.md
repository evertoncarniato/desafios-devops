# Desafio 06

Agora é hora de automatizarmos o deploy da nossa aplicação. Para isso, vamos utilizar uma pipeline.

## Atividade

Criar uma pipeline utilizando qualquer ferramenta de CI/CD e fazer o deploy da sua aplicação no kubernetes.

## Critérios de aceite / sucesso

* assim que um commit for realizado na sua branch master, o pipeline deve ser automaticamente iniciado
* build e publicação da imagem do contêiner
* deploy no Kubernetes da sua aplicação (utilizando os yamls do desafio 5)
* teste da sua aplicação
* Em caso de falha no teste, efetuar o rollback da aplicação
* Readme com a expliação de por que escolheu essa ferramenta de CI/CD e como configurá-la

## Referências

Pipeline: https://gomex.me/2020/05/28/qual-software-de-pipeline-ci/cd-voc%C3%AA-deve-usar/

