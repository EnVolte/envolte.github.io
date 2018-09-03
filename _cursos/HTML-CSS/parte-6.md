---
layout: curso
title:  "Curso de HTML & CSS (Parte 6)"
subtitulo: "Introdução ao HTML5."
date:   2018-08-24 02:30:00
categories: HTMLCSS
---

Nesta 6ª parte do curso, iremos finalmente entrar em **HTML5**. Durante as últimas aulas, falei sobre a estrutura básica de uma página em HTML, como formatar textos, separar conteúdos, criar tabelas, formulários etc. Se você está aqui, deve ter feito as nossas atividades propostas ao longo dos posts e já deve estar familiarizado com os códigos. Caso você queira saber um pouco mais sobre a história do *HTML* e suas versões antes de iniciarmos o HTML5, [clique aqui](https://pt.wikipedia.org/wiki/HTML#Hist%C3%B3ria).

<section id="quadro">
<label>Índice</label> <button class="openclose">Abrir/Fechar</button>
<div class="linha"></div>
<section id="indice">
<ol><!-- indice -->
<li><a href="#01">O que é HTML5?</a></li>
<li><a href="#02">Semântica</a></li>
<li><a href="#03">Seções e estruturas</a></li>
<li><a href="#04">O que mais mudou?</a></li>
<li><a href="#05">Formulários</a></li>
<li><a href="#06">Modelos de conteúdo</a></li>
<li><a href="#07">Infográfico</a></li>
</ol>
</section>
</section>
<br>

<span id="01"></span>
### O que é HTML5?

O HTML5 é a mais recente atualização da evolução da linguagem de marcação criada por *Tim Berners-Lee*, também conhecido por desenvolver o protocolo **HTTP**. Atualmente, se encontra na versão **5.2**. São destaques os novos *elementos*, *atributos*, *comportamentos* e um conjunto maior de tecnologias que permitem o desenvolvimento de aplicações e sites mais diversos e poderosos. Mas antes de aprendermos a desenvolver utilizando HTML5, vamos ver o que mudou.

<span id="02"></span>
#### Semântica

Agora é possível descrever mais precisamente o seu conteúdo com a adição de novas tags de *seções* e *conteúdo*. A proposta desta quinta versão do HTML é oferecer mais **organização** e **acessibilidade**. Nós vamos ver mais sobre isso a seguir.

<span id="03"></span>
#### Seções e estruturas

Antes do HTML5, todo o conteúdo era divido em divs, que é a forma como muitos aprenderam a criar páginas inteiras para a web. Se você procurar na internet, ou em livros mais antigos, muitos tutoriais ainda te ensinarão a fazer isso. Não é que seja errado, mas não é a melhor forma de desenvolver sites atualmente.

As novas tags vieram para te ajudar, desenvolvedor, assim como as pessoas que consomem seu conteúdo. Os mecanismos de busca, por exemplo, vão buscar pela parte do conteúdo que contém a informação mais importante. Se você desenvolver páginas sem a nova estrutura, que proporciona uma organização melhor e facilita a **acessibilidade**, é possível que o conteúdo indexado não faça sentido, ou perca posições nas pesquisas. Para resumir, desenvolver seu site estruturado em HTML5 proporciona melhores resultados de SEO e garante o bom funcionamento dos métodos de acessibilidade.

A seguir, você verá uma tabela com as novas tags e as definições de cada uma. As mais básicas são ```<section>```, ```<article>```, ```<nav>```, ```<header>```, ```<footer>``` e ```<aside>```. Elas definem *seções*, *artigos*, *menus*, *cabeçalhos*, *rodapés* e *partes do conteúdo* de uma página.

Elemento              |    Definição
----------------------|-----------------------------------------
&#60;article&#62;	    | Define um artigo em uma página
&#60;header&#62;	    | Define um cabeçalho da página ou seção
&#60;footer&#62;		  | Define o rodapé da página ou seção
&#60;section&#62;		  | Define uma seção na página
&#60;nav&#62;	        | Define links de navegação na página
&#60;aside&#62;		    | Define um conteúdo, uma parte, do conteúdo da página
&#60;bdi&#62;	        | Define um texto que pode ser formatado em diferentes direções
&#60;details&#62;		  | Define detalhes adicionais que o usuário pode ver ou ocultar
&#60;dialog&#62;		  | Define uma caixa de diálogo ou janela
&#60;figcaption&#62;	|	Define uma legenda para um elemento &#60;figure&#62;
&#60;figure&#62;		  | Define um conteúdo como ilustrações, diagramas, fotos, códigos, listagens, etc
&#60;main&#62;		    | Define o conteúdo principal de uma página
&#60;mark&#62;		    | Define um texto marcado ou realçado
&#60;menuitem&#62;		| Define um commando/menu que pode ser usado para invocar um menu popup
&#60;meter&#62;		    | Define uma medida escalar dentro de uma faixa conhecida
&#60;progress&#62;		| Define o progresso de uma tarefa
&#60;rp&#62;		      | Define o que exibir em navegadores que não exibem anotações<br>ruby (anotações ruby são para mostrar a pronúncia de caracteres do Leste Asiático.)
&#60;rt&#62;		      | Define a pronúncia de um caractere (para tipografias do Leste Asiático)
&#60;ruby&#62;		    | Define uma anotação ruby (para tipografia do Leste Asiático)
&#60;summary&#62;		  | Define um título visível para um elemento &#60;details&#62;
&#60;time&#62;		    | Define uma data/hora
&#60;wbr&#62;		      | Define uma possível quebra de linha
&#60;datalist&#62;		| Lista opções predefinidas para controles inputs
&#60;keygen&#62;		  | Define um campo de gerador de par de chaves (para formulários)
&#60;output&#62;		  | Define o resultado de um cálculo
&#60;canvas&#62;		  | Define um desenho gráfico usando JavaScript
&#60;svg&#62;		      | Define um desenho gráfico usando SVG
&#60;audio&#62;		    | Define um conteúdo de som ou música
&#60;embed&#62;		    | Define um contêiner para aplicações externas (como plug-ins)
&#60;source&#62;		  | Define fonte para &#60;video&#62; e &#60;audio&#62;
&#60;track&#62;		    | Define faixas para &#60;video&#62; e &#60;audio&#62;
&#60;video&#62;		    | Define um conteúdo de vídeo

Não se preocupe em decorar todas essas tags e seus significados logo de primeira. Atente-se apenas às mais importantes, que foram citadas acima da tabela.

<span id="04"></span>
### O que mais mudou?

Uma das primeiras novidades em relação à escrita de documentos em **HTML5**, é a declaração *doc type*, que foi simplificada para ```<!DOCTYPE html>```. Lembre-se de que esta declaração é necessária para informar ao navegador que estamos trabalhando com um documento em HTML.

<span id="05"></span>
#### Formulários

Os formulários em HTML5 agora são mais completos. Quem trabalha com desenvolvimento de sites, sabe a importância do bom funcionamento de um formulário. E quem pensa que eles só são úteis na hora de criar páginas de contato ou barras de busca, se engana: eles estão presentes em várias formas, em praticamente qualquer site, e são muito úteis para inserir informações nos bancos de dados.

Foram adicionados seletores de cores (color picker), datas (data picker) e controles numéricos (ajustes de *maior* e *menor*), por exemplo. Os inputs agora incluem, também, os tipos *e-mail*, *pesquisa*, *url*, *range*, *número* etc. A importância de se ter um tipo específico para cada uso não está apenas na semântica, mas na forma como o navegador irá interpretar a informação e realizar a checagem dos dados, impedindo que os usuários enviem informações incompletas ou erradas. Já era possível fazer isso através de Javascript, PHP ou outra linguagem de programação, porém, o HTML5 veio para facilitar a forma como desenvolvemos para a web.

<span id="06"></span>
#### Modelos de conteúdo

Os elementos em HTML são tipicamente divididos entre elementos de bloco e elementos em linha. Com a chegada do HTML5, foram introduzidos 7 novos modelos de conteúdo.

- Metadata (Metadados)
- Embedded (Embutido)
- Interactive (Interativo)
- Heading (Título)
- Phrasing (Parágrafo)
- Flow (Fluxo)
- Sectioning (Seccionando)

Vamos ver melhor cada um desses novos modelos, com seus respectivos exemplos, a seguir.

##### Metadata

Conteúdo que configura a apresentação ou comportamento do resto do conteúdo. Estes elementos estão presentes no **cabeçalho** de um documento em HTML. São exemplos: ``<base>``, ``<link>``, ``<meta>``, ``<noscript>``, ``<script>``, ``<style>``, ``<title>``.

##### Embedded

Conteúdo importado de outras fontes para dentro do documento. São exemplos: ``<audio>``, ``<video>``, ``<canvas>``, ``<iframe>``, ``<img>``, ``<math>``, ``<object>``, ``<svg>``.

##### Interactive

Conteúdo projetado especificamente para a interação do usuário. São exemplos: ``<a>``, ``<audio>``, ``<video>``, ``<button>``, ``<details>``, ``<embed>``, ``<iframe>``, ``<img>``, ``<input>``, ``<label>``, ``<object>``, ``<select>``, ``<textarea>``.

##### Heading

Define o cabeçalho de uma seção. São exemplos: ``<h1>``, ``<h2>``, ``<h3>``, ``<h4>``, ``<h5>``, ``<h6>``.

##### Phrasing

Este modelo possui um número de elementos em linha em comum com o HTML4. Você reconhecerá alguns, veja: ``<span``, ``<img>``, ``<strong>``, ``<sub>``, ``<small>``, ``<label>`` e outros.

> O mesmo elemento pode pertencer a mais de um modelo de conteúdo.
> Repare que muitos desses elementos já foram citados anteriormente.

##### Flow

Contém a maioria dos elementos em HTML5 que devem ser incluídos no fluxo normal de uma página.

##### Sectioning

Define o escopo de cabeçalhos, conteúdo, navegação e rodapés. São exemplos: ``<article>``, ``<aside>``, ``<nav>``, ``<section>``.

> Os diversos modelos de conteúdo se sobrepõe em algumas áreas, dependendo de como eles estão sendo utilizados.

Para melhor entendimento, veja um exemplo da estrutura desses modelos no *infográfico* abaixo.

<span id="07"></span>
<figure style="max-width: 50%; margin: auto auto;"><img src="https://envolte.github.io/arquivos/fotos/modelosconteudo.png" width="auto" />
  <figcaption>Simplificando o esquema dos modelos de conteúdo.</figcaption>
</figure>

Na próxima parte do Curso de HTML & CSS, iremos aprender sobre a *estrutura básica* de uma página em **HTML5**.

Ficou com alguma dúvida, encontrou algum equivoco ou gostaria de contribuir com o conteúdo? Comente abaixo!
