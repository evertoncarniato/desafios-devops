#  Desafio 9

Nesse desafio, vamos utilizar um LAMBDA que será executado a partir de um tópico SNS, para sabermos todos os IPS adicionados pela amazon em um período de tempo

## Atividade 1

Criar um código lambda em python ou node.js para ler os dados de uma url que vira na mensagem do SNS, e extrair quantos ips foram alterados para cada serviço da AWS em uma região


## Critérios de aceite / sucesso
* Aplicação lambda deve ser executada sempre que algo for publicado no topico SNS `arn:aws:sns:us-east-1:806199016981:AmazonIpSpaceChanged` 
* A Lambda deve ser provisonada utilizando terraform, ansible, serverless, SAM ou Cloudformation para toda a configuração
* Um readme com a documentação do que foi realizado e justificativa das escolhas.


## Test event 
Para validar a invocação da lambda utilizando o SNS usem o evento de teste abaixo:
``` JSON
{
    "Records": [
        {
            "EventVersion": "1.0",
            "EventSubscriptionArn": "arn:aws:sns:EXAMPLE",
            "EventSource": "aws:sns",
            "Sns": {
                "SignatureVersion": "1",
                "Timestamp": "1970-01-01T00:00:00.000Z",
                "Signature": "EXAMPLE",
                "SigningCertUrl": "EXAMPLE",
                "MessageId": "95df01b4-ee98-5cb9-9903-4c221d41eb5e",
                "Message": "{\"create-time\": \"yyyy-mm-ddThh:mm:ss+00:00\", \"synctoken\": \"0123456789\", \"md5\": \"532fd4e00d3c51e8459490f49274be8c\", \"url\": \"https://ip-ranges.amazonaws.com/ip-ranges.json\"}",
                "Type": "Notification",
                "UnsubscribeUrl": "EXAMPLE",
                "TopicArn": "arn:aws:sns:EXAMPLE",
                "Subject": "TestInvoke"
                }
            }
        ]
     }
```

## Referências
Serverless:  https://www.serverless.com/framework/docs/providers/aws/guide/deploying/

AWS SAM: https://medium.com/@devops_83824/developing-serverless-applications-on-aws-using-aws-serverless-application-model-sam-cdcf3bda59bd

SNS: https://docs.aws.amazon.com/pt_br/sns/?id=docs_gateway

LAMBDA: https://docs.aws.amazon.com/pt_br/lambda/?id=docs_gateway

