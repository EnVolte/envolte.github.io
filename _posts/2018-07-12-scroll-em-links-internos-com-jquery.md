---
layout: post
title:  "Scroll em links internos com JQuery"
capa: "https://envolte.github.io/arquivos/fotos/javascript.png"
capaindex: "https://envolte.github.io/arquivos/fotos/index/javascript.png"
date:   2018-07-14 16:20:00
categories: Javascript
---

Um dos componentes essenciais de qualquer site, são os *links*. Sejam estes para o menu, dentro de um post, em um anúncio, sempre temos um links dentro da página. Eles, normalmente, nos levam a uma outra página, dentro ou fora do endereço de nosso site. Nesta categoria, nós temos os *links internos*, que fazem a ligação de um ítem à uma determinada seção do site. Estes links são geralmente encontrados em um índice, como os das *páginas* de nossos cursos, ou para se fazer uma página carregar do menu com Javascript.

Apesar de ser uma função em HTML, nós podemos mudar um pouco o funcionamento dela. Como todos sabemos, o **Javascript** é uma linguagem *front-end*, *client-side*, que é vista frequentemente na criação de sites estáticos e dinâmicos. Ela tem o poder de criar funções, efeitos, carregar páginas, interagir com elemento e de fazer coisas inimagináveis - o que vale é a sua imaginação, aliada ao código.

Sabendo disso, iremos criar uma função em Javascript, aliada ao Jquery, que fará com que os links internos possam deslizar suavemente pela página. Para entender melhor, vamos a um exemplo básico de um link interno.

      <ul class="links">
      <li><a href="#link-1">Link 1</a></li> <!-- Funciona como um link comum, com a difereça da cerquilha (#) -->
      </ul>
      
      <!-- conteúdo -->
      
      <div id="link-1"> <!-- A div, que também pode ser um span, tem o mesmo id do link -->
      <p>O conteúdo vai aqui.</p>
      </div>
    
Faça um teste no seu navegador e você verá que este código faz com que, ao clicarmos no link, sejamos levados direto a *div* com a *id* correspondente. Este é o uso básico desta função, que pode atender diversas necessidades. Porém, nós queremos que, ao clicar, a página deslize até a div, ao invés de apenas fazer a mudança do conteúdo.

Para começar, vamos entender o código. Já que estamos trabalhando com links, devemos fazer com que o seletor pegue apenas os que pertencem à nossa lista, que está com a classe *links*.

    $('ul.links a[href^="#"]').on('click', function(e) {
     
Esta parte também só pegara os links que começarem com a cerquilha (#).

    e.preventDefault(); // faz com que a função atribuída não funcione de forma padrão
    var id = $(this).attr('href'),
    targetOffset = $(id).offset().top; // a segunda linha pega o valor do href (link), a terceira calcula a distância do topo dá página até seu elemento.
    
Agora, iremos para a ultima parte, onde criaremos um função que seleciona os elementos *html* e *body*, fazendo uma animação.
    
    $('html, body').animate({ 
    scrollTop: targetOffset - 30 // a div chamada pelo link ficará a 30px do topo
    }, 700); // 700 é a velocidade da animação que vai fazer os links deslizarem pela página (700 milissegundos).
    });
    
Você pode conferir o resultado, bem como a forma de implementar o código, logo abaixo.

<iframe class="codigo" width="100%" height="300" src="//jsfiddle.net/3mysa0b1/23/embedded/js,html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>


Não se esqueça de incluir a bibliote JQuery mais recente para que o código funcione!
