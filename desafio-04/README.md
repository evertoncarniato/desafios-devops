# Bem vindo ao desafio 4

Agora que já sabemos como criar um ambiente do zero utilizando automação, vamos treinar um pouco de programação e do uso de contêiners.

## Atividade 

Vamos criar uma imagem docker com uma API em python  utiliando o framework flask ou javascript utiliando o framework node.js

### Critérios de aceite / sucesso
* Seu contêiner deve estar publicado no [dockerhub](hub.docker.com)
* Sua API deve ter uma rota de healthchek testando os componentes:
1. versão da API
2. banco SQL
3. nanco NoSQL
4. uma fila (SQS, Redis, etc.)
5. e seu status
* retorno esperado do healthcheck:

```
{"API": {
     "api": "1.0",
     "dep": {
     "db-sql": "OK",
     "db-nosql": "OK",
      "fila": OK,
      "status": 200
    },
  }
}

```

# Referências
Docker: https://docs.docker.com/

Play with Docker: https://labs.play-with-docker.com/

Flask: https://flask-ptbr.readthedocs.io/en/latest/

Node.js: https://nodejs.org/pt-br/docs/
