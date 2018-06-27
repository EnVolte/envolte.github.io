---
layout: post
title:  "Curso de HTML & CSS (Parte 2)"
date:   2018-06-26 10:00:00
categories: Curso
---

Na [primeira parte](https://envolte.github.io/curso/2018/06/26/curso-html-css-parte-1.html) do nosso curso, aprendemos um pouco sobre as tags básicas, como ``<html>``, ``<head>`` e ``<body>``. Agora, com intuito de praticar, vamos começar a montar uma página inteira em HTML. Por enquanto, ainda sem nenhuma estilização.

Todo esse processo que iremos iniciar agora é extremamente necessário para que você possa ir se acostumando com essas tags, pois, se você esquecer de fechar qualquer uma delas, um problema enorme pode surgir no seu código. Na verdade, esse tipo de problema é realmente bem comum, mas a página fica tão bagunçada, que faz parecer que se trata de algo maior. Mas não se desespere, abra seu *editor de códigos* e vamos colocar a *mão na massa*!

Comece criando um arquivo chamado *index.html*. Salve-o em uma pasta de fácil acesso. Este arquivo poderá ser aberto no seu navegador sem problemas, e sem que você precise instalar um programa adicional. Adicione o código a seguir:

    <html>
    <head></head>
 
    <body>
    ...
    </body>
    </html>
    
Recomendo que você digite o código ao invés de **copiar** e **colar**. Salve o arquivo e abra. Veja que o código retornou uma página em branco. Agora vamos adicionar mais algumas tags, mas antes, vou explicar um pouco sobre elas.

> Documentos HTML podem ser salvos tanto com nomes terminados em **.html**, como **.htm**.

#### Tag ``<title>``

Como o nome já diz, esta tag faz referência ao título da página. Ela é inserida dentro da tag **head**, e sua ausência faz com que a página fique sem indentificação no navegador. Também é usada pelas ferramentas de busca, como o Google, para indexar o seu site.

#### Tag ``<style>``

A tag **style** indica que todo conteúdo que estiver dentro dela será em CSS. Neste primeiro momento, não iremos criar uma folha de estilos.

#### Tag ``<h1>``

**h1** é uma *heading tag*, um recurso utilizado para destacar títulos e subtitulos de uma página. H1 é uma abreviação para "Header 1", ou "Cabeçalho 1". Ele é precedido por **h2**, **h3**, **h4**, **h5** e **h6**. Assim como suas posições, essas tags também possuem tamanhos diferente, sendo a *h1* a maior.

#### Tag ``<p>``

Para iniciar parágrafos em HTML, nos usamos a tag **p** para abertura e fechamento. Os navegadores adicionam uma linha em branco antes e depois de um parágrafo.

#### Quebra de linha

Usa-se **<br>** para fazer uma quebra de linha sem iniciar um novo parágrafo. Isso significa que após adicionar esta tag, o conteúdo seguinte inciará em uma nova linha.
