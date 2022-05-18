# Bem vindo ao desafio 01

Esse é o primeiro desafio então vamos começar aplicando conceitos de administração de sistemas no modelo mais clássico (raiz).

## Atividade

* Criar um webserver centos7 na AWS
* Configurar uma loja com Magento 
* Configurar um blog com WordPress
* Configurar o Tomcat
* Cria um site estático 
* Criar um domínio e ajustar as entradas de DNS
* criar certificado SSL wildcard

### Critérios de aceite / sucesso

* Ao menos um dos sites deve estar configurado com o certificado SSL
* Cada um dos ambientes precisa ter o seu próprio _virtual host_ no Nginx
* As configurações dos sites devem ficar no diretório `/var/www/html/NOME-DA-PASTA` ou `/usr/share/nginx/html/NOME-DA-PASTA`, com uma pasta para cada ambiente
* O Tomcat precisa apenas estar no ar e via Nginx entregar a página padrão
* O DNS do domínio deve ser criado e configurado no Route53
* entradas:
    - site.dominio < DNS do site estático
    - loja-blog.dominio < DNS do Magento
    - blog.dominio <  dns do WordPress
    - tomcat.dominio < dns do Tomcat
* o site deve apontar para um `index.php`
* o blog não pode abrir com `/wordpress` na frente
* documentação dos passos realizados para a criação desse ambiente no README.md



# Referências

Criar um dominio grátis: http://www.dot.tk/pt/index.html

Tomcat: https://tomcat.apache.org/download-90.cgi

Wordpress: https://br.wordpress.com/ 

Magento: https://magento.com/

Let's encrypt: https://letsencrypt.org/

**Boa Sorte!**
