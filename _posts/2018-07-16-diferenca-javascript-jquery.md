---
layout: post
title:  "Diferença entre Javascript e JQuery"
capa: "https://envolte.github.io/arquivos/fotos/jsquery.png"
capaindex: "https://envolte.github.io/arquivos/fotos/index/jsquery.png"
date:   2018-07-16 16:20:00
categories: Javascript Jquery
---

Você já deve ter visto por aí alguém falar de **Javascript** e **JQuery** em muitos tutoriais e vídeoaulas. Se você tem um conhecimento básico em desenvolvimento web, deve saber que Javascript é uma linguagem muito popular, e que está presente na maioria dos sites. Mas você sabe a diferença entre esses dois? Foi pensando nisso, e no intuito de sanar essas dúvidas, que resolvi fazer este post para esclarecer de vez as diferenças entre cada um.

Para começar, vamos falar um pouco de Javascript. Esta linguagem surgiu em 1995 e hoje é uma das mais usadas em todo o mundo, ocupando o 8º lugar na lista de linguagens de programação mais populares de Julho de 2018, segundo o **[Tiobe](https://www.tiobe.com/tiobe-index/javascript/)**. Ao contrário de outras, como PHP, Java, Ruby etc, o javascript é uma linguagem *client-side*, que funciona do lado do cliente. E não, Javascript não tem nada a ver com a linguagem *Java*.

### Mas como assim funciona do lado do cliente?

Se você está fazendo nosso [Curso de PHP](https://envolte.github.io/cursos/PHP/), deve saber a diferença entre as linguagens *client-side* e *server-side*. Mas se não, não se preocupe, vou explicar. A linguagem client-side funciona junto ao cliente, aquele que visita o site. Este tipo de linguagem não precisa de nenhum interpretador, como o *PHP*, por exemplo, que funciona ao lado do servidor (linguagem server-side). Todo código em linguagens client-side é lido pelo navegador.

### Para que serve o Javascript?

Seu principal uso consiste em controlar elementos *HTML* e *CSS* para manipular páginas. Também é muito comum na criação de funções, como botões de voltar e avançar, menus com submenus, redirecionamento de páginas, janelas pop-up, alertas etc. Estes são apenas alguns dos muitos exemplos que poderia destacar aqui.

### Existe alguma limitação?

Como Javascript é uma linguagem que funciona do lado do cliente, ela não faz nenhuma conexão direta com um banco de dados, como é possível nas linguagens server-side, e para determinados tipos de projetos, pode não ser muito seguro os processos funcionarem todos ao lado do cliente. É realmente muito poderosa, e mesmo que não desempenhe as mesmas funções que linguagens mais complexas, é essencial no desenvolvimento web. 

Apesar de suas limitações, uma de suas principais qualidades é, justamente, a facilidade de integração com outras linguagens. Até mesmo sites estáticos - construídos no código puro - podem fazer o uso de Javascript.

### Javascript em ação

Para entender melhor como usar Javascript, vamos a um exemplo básico.

    <script type="text/javascript">
    alert('Olá, mundo!');
    </script>
    
Repare que nós fizemos uso de uma tag para indicar ao navegador que estamos usando um *script* em *javascript*. A função ```alert``` retornará um *aviso* com "Olá, mundo!".

Agora que já entendemos bem o que é Javascript, vamos falar sobre o JQuery. Como você já deve saber, para que possamos utilizá-lo, devemos implementar uma chamada de sua biblioteca em nossa página, geralmente dentro da tag ```head```.

    <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    
Se não a fizermos, nenhum código em JQuery será executado corretamente, e isso pode nos causar muita dor de cabeça. Mas afinal, o que é esse **JQuery**? Ele tem algo a ver com Javascript?

A resposta é simples: sim. O **JQuery** é uma biblioteca de códigos, um *framework*, leve e cheio de recursos em Javascript. Trata-se de um projeto de código aberto, e muito útil, que foi criado em 2006. A sua proposta é mudar a forma de escrita dos códigos em Javascript, "descomplicando" o processo. O JQuery também permite que criemos *plugins* de alta complexidade sem o esforço que teríamos se usassemos o Javascript.

Seu slogan "*Write less, do more*" (Escreva menos, faça mais) é a tradução perfeita do que essa biblioteca significa para o desenvolvimento web.

### O que JQuery pode fazer?

- Seleção e manipulação de elementos em HTML e CSS
- Efeitos e animações
- Navegação pelo DOM (Document Object Model, ou *Modelo de Objeto de Documento*)
- Ajax
- Eventos (events)

A sintaxe do JQuery tem algumas diferenças do Javascript. Porém, assim como nele, começamos informando ao navegador que estamos utilizando um script.

    <script>
    $('seletoremHTML').acao(); // Em seletoremHTML, você coloca o elemento que o JQuery manipulará. ".acao()" é a ação que será desempenhada.
    ... // Aqui ficam os eventos.
    </script>
    
### Resumo

**Javascript** é uma linguagem de programação *client-side*. **JQuery** é um *framework* desenvolvido em Javascript que tem o objetivo de simplificar o desenvolvimento nesta linguagem. Escrevendo em JQuery, você gastará menos tempo e terá menos dores de cabeça, porém terá de implementar a biblioteca dentro de sua página para que funcione. Enquanto isso, o Javascript é suportado em todos os navegadores.

Qual é o melhor? O que atender a suas necessidades. Atualmente, no site oficial do [JQuery](https://jquery.com), você encontra diversos exemplos de funções que ele pode desempenhar. Você também encontrará a documentação oficial.
