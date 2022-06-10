# Caddy

Usamos o Caddy para fazer os direcionamentos de nossos domínios para os serviços que eles representam.

Como nossos apps são todos em Docker, utilizamos o [Caddy Docker Proxy](https://github.com/lucaslorentz/caddy-docker-proxy),
que lê labels especiais no container para fazer o direcionamento.


## Exemplo

"Onde encontro o chat.semudando.com.br?"

Este serviço irá procurar em todos os serviços no cluster "Alguém é responsável pelo chat.semudando.com.br?" e fará o 
direcionamento corretamente.


## HTTPS

Uma das funções que vem de brinde só por usar o Caddy é o HTTPS _automágico_ em todas as URLs.
Ele lida com a terminação SSL