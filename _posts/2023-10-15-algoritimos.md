
---
layout: post
comments: true
title: "Algorítimos"
date: 2023-10-15 03:06:56
image: '/assets/img/'
description:
main-class:
color:
tags:
categories:
twitter_text:
introduction:
---

## Entendendo a proposta

Ao longo dos proximos dias, estarei escrevendo uma série de posts que acredito que podem ajudar no aprendizado do basico para futuros desenvolvedores. Através de exemplos e exercícios, mostrarei como é possivel conectar as ideias de forma a resolvermos problemas mais complexos com o computador.


## Afinal, o que são algorítimos?

Muto se fala sobre algorítimos, mas na prática, nem sempre esse termo é explicado e é claro. O termo algoritmo refere-se a uma sequência de instruções bem definidas para chegarmos a um objetivo. Como uma “sequência bem definida de instruções”, devemos entender instruções claras que podem ser facilmente entendidas por quem vai executá-las e em uma ordem bem estabelecida. Apesar do termo algoritmo ser muito utilizado na matemática e computação, ele está presente em muitas atividades do nosso dia a dia. Toda vez que executamos algum processo que pode ser repetido através de um conjunto de instruções como trocar o pneu de um carro, dar o nó em uma gravata, cozinhar um prato utilizando uma receita, tocar uma música utilizando uma partitura ou cifras, estamos executando um algoritmo.

Quando nos referimos aos computadores, vale ressaltar que apesar de possuirem uma grande capacidade em processar e calcular grandes volumes de informação de forma muito rápida, para realizar qualquer tarefa, por mais simples que seja, é preciso que sejam atribuídos a eles um conjunto de operações que eles consigam compreender. Cabe, portanto, à capacidade de raciocínio humana indicar ao computador quais instruções devem ser efetuadas, e em qual ordem, para que ele processe as informações disponíveis de forma útil e adequada, ou seja, devemos informar qual algoritmo o computador deve executar para atingir o que desejamos. O que chamamos de programa é, portanto, um algoritmo escrito em uma linguagem que o computador consiga entender.

A palavra lógica se origina da palavra grega logos, que significa conhecimento, pensamento. Podemos traduzir lógica como a arte de pensar de forma correta e bem estruturada. Quando nos referimos à lógica de programação, estamos falando da estruturação de nossas ideias com o objetivo de resolver um problema utilizando o computador como ferramenta.

Quando pretendemos fazer isto, devemos entender o problema que queremos resolver, dividi-lo em problemas menores até chegarmos a problemas que sabemos e conseguimos resolver, ou melhor, em problemas que sabemos mostrar ao computador como ele deve resolver. Por fim, devemos unir as soluções destes pequenos problemas (sempre que possível utilizando o computador para isto) para finalmente chegarmos à solução do problema original.

### O que é um programa?

Um programa é um conjunto de instruções, também podemos chama-los de algoritmos, que pode ser entendido e executado por um computador/dispositivo móvel. Para que isto ocorra, o algoritmo deve ser escrito por intermédio do que chamamos de linguagem de programação.

A maioria das linguagens de programação foram construídas de forma que sejam facilmente compreendidas por seres humanos e também lida e executada por um computador.

Existem inúmeras linguagens de programação para os mais diversos fins (e gostos). Como exemplos, podemos citar: C, C++, Go, Ruby, Python, JavaScript, PHP, Swift, Java, C#, entre uma infinidade de outras.

Programar é criar um conjunto de instruções para um dispositivo executar, sempre de forma objetiva e ordenada, com o intuito do programa ser compreendido e bem processado. Vamos a um exemplo:

Ao longo dos próximos posts irei apresentar conceitos de Lógica de Programação e Orientação a Objetos, a linguagem que iremos utilizar será Go, assim, já nos familiarizaremos e aprenderemos a sintaxe da linguagem junto aos conceitos e operações básicas.

Ao montar uma pizza temos a seguinte lista de ingredientes:

![Lista de Ingredientes](/assets/img/1._Conceitos_Iniciais_-_01.png)

Quais seriam as opções de instruções?

Se sugerirmos:

1 – AdicionarQueijo()

Teremos um problema, pois colocaríamos o queijo onde? As instruções, que também são conhecidas como comandos, precisam ser objetivas, mas também necessitam estar ordenadas. Vamos iniciar novamente:

1 – PegarMassa
2 – AdicionarQueijo
3 – AdicionarCalabresa
4 – AdicionarTomate
5 – AdicionarCheiroVerde
6 – AdicionarCebola
7 – AdicionarAzeitonas

Será esse o nosso melhor conjunto de instruções? Vamos ver o resultado?

![Pizza V1](/assets/img/1._Conceitos_Iniciais_-_02.png)

Esquecemos de alguma coisa? Precisamos fatiar os ingredientes! Nova receita:

1 – FatiarQueijo
2 – FatiarCalabresa
3 – FatiarTomate
4 – FatiarCebola
5 – PegarMassa
6 – AdicionarQueijo
7 – AdicionarCalabresa
8 – AdicionarTomate
9 – AdicionarCebola
10 – AdicionarCheiroVerde
11 – AdicionarAzeitonas

Será!?

![Pizza V2](/assets/img/1._Conceitos_Iniciais_-_03.png)

Agora sim!  Montamos nossa pizza e conseguimos entender o quanto comandos imprecisos ou a falta deles podem nos levar a resultados inesperados!

