# Protocolo HTTP (Hyper Text Transfer Protocol)

1. **Hyper Text** é um texto que tem links associados,
2. Começou com transferência de textos linkados,

## Características

1. Faz parte da Camada de Aplicação
2. Ele é sem estado, ou seja, **Stateless**. Quando uma máquina faz uma requisição HTTP para um servidor, é como se essa comunicação fosse feita pela primeira vez.
3. Baseado no coneceito de requisição e resposta, **Cliente-Servidor**. Faço uma requisição para o servidor e posso receber, por exemplo, uma resposta como JSON.
4. O **Protocolo HTTP** roda em cima da Stack TCP/IP
5. Via de regra, o protocolo retorna conteúdos para formar uma página web.

## Fluxo Básico de uma Conexão HTTP
1. Usuário informa a URL no browser
2. O browser gera a requisição na raiz, por exemplo:
*GET / HTTP /1.1
Host: www.google.com.br* 
3. O servidor gera uma resposta, por exemplo, esta de sucesso:
*HTTP/1.1 OK
content-Type: text/html; charset=UTF-8
date: Mon, 30 Abril 2018 17:00:02 GMT
connection: close
content-Length: 438*
4. Browser exibe a página (se atente que são feitas várias requisições)

## Métodos do HTTP
1. **GET**: URL + parâmetros da requisição. 
2. **POST**: Parâmetros no corpo da requisição e não na URL. Não quer dizer que isso seja mais seguro. Para isso, é necessário que a requisição seja executada em cima de uma requisição https.
3. PUT
4. DELETE
5. TRACE
6. OPTIONS
7. CONNECT
8. HEAD


