---
layout: curso
title:  "Curso de HTML & CSS (Parte 2)"
subtitulo: "Principais tags, headings, formatação de texto, comentários e estrutura básica de página."
date:   2018-06-26 10:00:00
categories: HTMLCSS
---

Na [primeira parte](https://envolte.github.io/curso/2018/06/26/curso-html-css-parte-1.html) do nosso curso, aprendemos um pouco sobre as tags básicas, como ``<html>``, ``<head>`` e ``<body>``. Agora, com intuito de praticar, vamos começar a montar uma página inteira em HTML. Por enquanto, ainda sem nenhuma estilização.

Todo esse processo que iremos iniciar agora é extremamente necessário para que você possa ir se acostumando com essas tags, pois, se você esquecer de fechar qualquer uma delas, um problema enorme pode surgir no seu código. Na verdade, esse tipo de problema é realmente bem comum, mas a página fica tão bagunçada, que faz parecer que se trata de algo maior. Mas não se desespere, abra seu *editor de códigos* e vamos colocar a *mão na massa*!

<section id="quadro">
<label>Índice</label> <button class="openclose">Abrir/Fechar</button>
<div class="linha"></div>
<section id="indice">
<ol><!-- indice -->

<li><a href="#01">HTML em prática</a></li>
<li><a href="#02">Extensões do HTML</a></li>
<li><a href="#03">Tag 'title'</a></li>
<li><a href="#04">Tag 'style'</a></li>
<li><a href="#05">Tags de cabeçalho</a></li>
<li><a href="#06">Tag 'p'</a></li>
<li><a href="#07">Quebra de linha 'br'</a></li>
<li><a href="#08">Formatando elementos com HTML</a></li>
<li><a href="#09">Linha horizontal</a></li>
<li><a href="#10">Comentários</a></li>
<li><a href="#11">Exercício</a></li>

</ol>
</section>
</section><br>

<span id="01"></span>
Comece criando um arquivo chamado *index.html*. Salve-o em uma pasta de fácil acesso. Este arquivo poderá ser aberto no seu navegador sem problemas, e sem que você precise instalar um programa adicional. Adicione o código a seguir:

    <html>
    <head></head>
 
    <body>
    ...
    </body>
    </html>
    
Recomendo que você digite o código ao invés de **copiar** e **colar**. Salve o arquivo e abra. Veja que o código retornou uma página em branco. Agora vamos adicionar mais algumas tags, mas antes, vou explicar um pouco sobre elas.

<span id="02"></span>
> Documentos HTML podem ser salvos tanto com nomes terminados em **.html**, como **.htm**.

<span id="03"></span>
#### Tag ``<title>``

Como o nome já diz, esta tag faz referência ao título da página. Ela é inserida dentro da tag **head**, e sua ausência faz com que a página fique sem indentificação no navegador. Também é usada pelas ferramentas de busca, como o Google, para indexar o seu site.

<span id="04"></span>
#### Tag ``<style>``

A tag **style** indica que todo conteúdo que estiver dentro dela será em CSS. Neste primeiro momento, não iremos criar uma folha de estilos.

<span id="05"></span>
#### Tags ``<h1>``, ``<h2>``, ``<h3>``, ``<h4>``, ``<h5>`` e ``<h6>``

**h1** é uma *heading tag*, um recurso utilizado para destacar títulos e subtitulos de uma página. H1 é uma abreviação para "Header 1", ou "Cabeçalho 1". Ele é precedido por **h2**, **h3**, **h4**, **h5** e **h6**. Assim como suas posições, essas tags também possuem tamanhos diferente, sendo **h1** a maior. Não é recomendado o uso dessas tags apenas para aumentar o texto, visto que os motores de busca utilizam esses cabeçalhos para indexar o conteúdo de uma página.

<span id="06"></span>
#### Tag ``<p>``

Para parágrafos em HTML, nós usamos a tag **p** para abertura e fechamento. Os navegadores adicionam uma linha em branco antes e depois de um parágrafo.

<span id="07"></span>
#### Quebra de linha ``<br>``

Usa-se **br** para fazer uma quebra de linha sem iniciar um novo parágrafo. Isso significa que após adicionar esta tag, o conteúdo seguinte inciará em uma nova linha.

<span id="08"></span>
### Formatando elementos

Em HTML, há uma lista de elementos que especificam o estilo de um texto. Vejamos alguns:

##### ``<b>`` e ``<strong>``

Essas duas tags são responsáveis por colocar os textos em **negrito**. Os navegadores mostram **strong** como **b**. Mas há uma diferença entre os dois: enquanto **b** apenas deixa em negrito, **strong** indica que o texto é importante.

##### ``<i>`` e ``<em>``

Essas duas tags transformam em *itálico*, outro elemento importante quando estamos destacando um texto. Os navegadores mostram *em* como *i*. A diferença é a mesma do item acima: *em* indica que o texto é importante.

<span id="09"></span>
##### Linha horizontal

Para criar uma linha horizontal, use a tag **<hr>**.

<span id="10"></span>
#### Comentários

Os navegadores não mostram comentários dentro das páginas, mas eles ficam no HTML. Você pode adicionar comentários, descrições, instruções e notas para que você não se perca no código. É uma ótima dica para iniciantes!

        <!-- Este é um comentário -->
        
O ponto de exclamação (**!**) deve ir logo após "**<**" na tag de abertura, mas não é necessário na tag de fechamento.

<span id="11"></span>
### Exercício

Agora que conhecemos um pouco sobre as tags do HTML, vamos colocá-las em prática fazendo nossa primeira página. Lembra do nosso arquivo *index.html*? Vamos editá-lo agora. Por enquanto, não iremos colocar nenhum código para download, já que estamos apenas fazendo exercícios simples.

    <html>
    <head>
    <title>Meu site</title>
    
    <style>
    /* Por enquanto, ficará vazio */
    </style>
    </head>
 
    <body>
    <h1>Meu site</h1>
    
    <h2>Titulo de uma postagem</h2>
    <p>Aqui escreveremos o conteúdo.</p>
    </body>
    </html>

O código acima é apenas um exemplo. Monte sua página com título e texto que quiser. Utilize as **tags de formatação** e o máximo de elementos ensinados que conseguir. Na próxima parte do curso, iremos colocar mais alguns itens dentro da página, incluiremos um **menu**, e aprenderemos a separar o conteúdo em ``divs``.

