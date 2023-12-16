---
layout: post
comments: true
title: "entrevistas de system design e agora?"
date: 2023-02-27 02:24:55
image: '/assets/img/'
description:
main-class:
color:
tags:
categories:
twitter_text:
introduction:
---

## Entrevistas de system design e agora?

- deixar a entrevista divertida e colaborativa
- afunilar o escopo e descobrir cada ponto
- entendimento dos componentes de infraestrutura
- disponibilidade
- consistencia
- reduzir o scopo do problema

- pensando em custo, isso seria uma preocupacao?

client server model
    internet
        http
        tcp
client server model
protocolos de redes
latencia
cache
proxy
load balances
replication
rate limit
publish subscribe


- system design
    - features
        - é mobile?
        - é web?
        - quais features sao mais importantes?
        - o que é mais importante?
            - consistencia?
            - disponibilidade?

    - tradeoffs
        - pensando em escalabilidade e volume de trafego, 
            - quantos usuarios vao usar a aplicacao por dia?
            - DAU - Daily active users
            - 10kk dau
            
        - pensando em elasticidade
            - quais os nossos picos?
                - qual a frequencia que esses usuarios tendem a acessar?
                - existe uma hora que o sistema tende a ter mais acessos?
                - quantos usuarios simultaneos é esperado no pior caso?
                - quantos usuarios simultaneos é esperado no melhor caso?

    - usuarios?
        - quais os tipos de usuarios que temos?
        - quais as regras para cada tipo?
        - de onde eles podem acessar?
        - temos alguma projecao de crescimento?
        - tem alguma media de duracao do acesso?
        
    - modelo de dados
        - quais as querys mais comuns?
        - qual a frequencia que iremos adicionar dados?
        - multi tanance ou single tanance?
        - relacional
            - os dados precisam estar normalizados?
                - qual o designer das tabelas?
                - como indexar os nossos campos?
                - quais seriam os campos que poderiam ser idexados?
        - no sql
            - key value store, graph, blob

        - preciso me preocupar com a disponibilizacao desses dados?
            - como isso será disponibilizado pela empresa?
            - existe um etl pipeline pronto ou mapeamos ele aqui tbm?
    
    - geografia e latencia
        - preciso ter servidores em diferentes regios do mundo?
        - existe um rtt (round trip time) ideal?
        - como tratamos latencia?
        - apontar diferentes usuarios para ips diferentes baseados de onde vem regioes diferentes
        - preciso de uma cdn para atender pessoas de regioes diferentes?

    - apis e seguranca
        - rest atende?
        - qual o rate limit?
        - como tratar ataques como DoS, DDos?
        - autenticacao e autorizacao, podemos considerar jwt?
        - em caso de nao relacional e muitos micro servicos internos, grpc pode ser uma boa
        - se for mobile, pq nao reduzir o payload de dados com graphql
        - quais as preocupacoes que precisamos ter relacionadas a seguranca?
        - precisamos dar suporte a alguma api externa?
        - https, ssl, certificado
        - vamos precisar nos preocupar com paginacao em algum momento?
    
    - disponibilidade
        - o que podemos utilizar para observar esses microservicos?
            - logs
            - metricas
            - alertas
        - como orquestraremos nossos containers?
        - como escalamos a nossa aplicacao?
            - vertical
                - scale up
            - horizontal?
                - scale out
    
    - mensageria
        - precisamos pensar em mensageria?
        - qual tipo de fila podemos utilizar?

    - high level
        - separar os elementos principais
            - clients
                - web
                - mobile
                - etc...
            - dns
            - load balancers
                - servers
                    - fun out