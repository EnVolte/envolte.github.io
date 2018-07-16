---
layout: post
title:  "Diferença entre Javascript e JQuery"
capa: "https://envolte.github.io/arquivos/fotos/javascript.png"
capaindex: "https://envolte.github.io/arquivos/fotos/index/javascript.png"
date:   2018-07-00 16:20:00
categories: Javascript Jquery
---

Você já deve ter visto por aí alguém falar de **Javascript** e **JQuery** em muitos tutoriais e vídeoaulas. Se você tem um conhecimento básico em desenvolvimento web, deve saber que Javascript é uma linguagem muito popular, e que está presente na maioria dos sites. Mas você sabe a diferença entre esses dois? Foi pensando nisso, e no intuito de sanar essas dúvidas, que resolvi fazer este post para esclarecer de vez as diferenças entre cada um.

Para começar, vamos falar um pouco de Javascript. Esta linguagem surgiu em 1995 e hoje é uma das mais usadas em todo o mundo, ocupando o 8º lugar na lista de linguagens de programação mais populares de Julho de 2018, segundo o **(Tiobe)[https://www.tiobe.com/tiobe-index/javascript/]**. Ao contrário de outras, como PHP, Java, Ruby etc, o javascript é uma linguagem *client-side*, que funciona do lado do cliente. E não, Javascript não tem nada a ver com a linguagem *Java*.

###Mas como assim funciona do lado do cliente?

Se você está fazendo nosso (Curso de PHP)[https://envolte.github.io/cursos/PHP/], deve saber a diferença entre as linguagens *client-side* e *server-side*. Mas se não, não se preocupe, vou explicar. A linguagem client-side funciona junto ao cliente, aquele que visita o site. Este tipo de linguagem não precisa de nenhum interpretador, como o *PHP*, por exemplo, que funciona ao lado do servidor (linguagem server-side). Todo código em linguagens client-side é lido pelo navegador.

###Para que serve o Javascript?

Seu principal uso consiste em controlar elementos *HTML* e *CSS* para manipular páginas. Também é muito comum na criação de funções, como botões de voltar e avançar, redirecionamento de páginas, janelas pop-up, alertas etc. Estes são apenas alguns dos muitos exemplos que poderia destacar aqui.

###Existe alguma limitação?

Como Javascript é uma linguagem que funciona do lado do cliente, ela não faz nenhuma conexão direta com um banco de dados, como é possível nas linguagens server-side, e para determinados tipos de projetos, pode não ser muito seguro os processos funcionarem todos ao lado do cliente. Ela é realmente muito poderosa, e mesmo que não desempenhe as mesmas funções que linguagens mais completas, é essencial no desenvolvimento web. 

Apesar de suas limitações, uma de suas principais qualidades é, justamente, a facilidade de integração com outras linguagens. Até mesmo sites estáticos - construídos no código puro - podem fazer o uso de Javascript.

###Javascript em ação

Para entender melhor como usar Javascript, vamos a um exemplo básico.

    <script type="text/javascript">
    alert('Olá, mundo!');
    </script>
    
Repare que nós fizemos uso de uma tag para indicar ao navegador que estamos usando um *script* em *javascript*. A função ```alert``` retornará um *aviso* com "Olá, mundo!".
