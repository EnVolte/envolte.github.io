---
layout: curso
title:  "Curso de HTML & CSS (Parte 6)"
subtitulo: "Introdução ao HTML5."
date:   2018-08-24 02:30:00
categories: HTMLCSS
---

Nesta 6ª parte do curso, iremos finalmente entrar em **HTML5**. Durante as últimas aulas, falei sobre a estrutura básica de uma página em HTML, como formatar textos, separar conteúdos, criar tabelas, formulários etc. Se você está aqui, deve ter feito as nossas atividades propostas ao longo dos posts e já deve estar familiarizado com os códigos. Caso você queira saber um pouco mais sobre a história do *HTML* e suas versões anter de iniciarmos o HTML5, [clique aqui](https://pt.wikipedia.org/wiki/HTML#Hist%C3%B3ria).

### O que é HTML5?

O HTML5 é a mais recente atualização da evolução da linguagem de marcação criada por *Tim Berners-Lee*, também conhecido por desenvolver o protocolo **HTTP**, e se encontra, atualmente, na versão **5.2**. São destaques os novos *elementos*, *atributos*, *comportamentos* e um conjunto maior de tecnologias que permitem o desenvolvimento de aplicações e sites mais diversos e poderosos. Mas o que mudou?

#### Semântica

Agora é possível descrever mais precisamente o seu conteúdo com a adição de novas tags de *seções* e *conteúdo*. A proposta desta quinta versão do HTML é oferecer mais **organização** e **acessibilidade**. Nós vamos ver mais sobre isso a seguir.

##### Seções e estruturas

Resumidamente, as novas tags mais populares são ```<section>```, ```<article>```, ```<nav>```, ```<header>```, ```<footer>``` e ```<aside>```. Elas definem seções, artigos, menus, cabeçalhos, rodapés e partes do conteúdo de uma página. Para que você possa compreender melhor, veja a tabela a seguir:

Elemento    |    Definição
------------|-----------------------------------------
<article>	  | Define um artigo em uma página
<header>	  | Define um cabeçalho da página ou seção
<footer>	  | Define o rodapé da página ou seção
<section>	  | Define uma seção na página
<nav>	      | Define links de navegação na página
<aside>	    | Define um conteúdo, uma parte, do conteúdo da página
<bdi>       | Define um texto que pode ser formatado em diferentes direções
<details>	  | Define detalhes adicionais que o usuário pode ver ou ocultar
<dialog>	  | Define uma caixa de diálogo ou janela
<figcaption>|	Define uma legenda para um elemento <figure>
<figure>	  | Define um conteúdo como ilustrações, diagramas, fotos, códigos, listagens, etc
<main>	    | Define o conteúdo principal de uma página
<mark>	    | Define um texto marcado ou realçado
<menuitem>	| Define um commando/menu que pode ser usado para invocar um menu popup
<meter>	    | Define uma medida escalar dentro de uma faixa conhecida
<progress>	| Define o progresso de uma tarefa
<rp>	      | Define o que exibir em navegadores que não exibem anotações ruby (anotações ruby são para mostrar a pronúncia de caracteres do Leste Asiático.)
<rt>	      | Define a pronúncia de um caractere (para tipografias do Leste Asiático)
<ruby>	    | Define uma anotação ruby (para tipografia do Leste Asiático)
<summary>	  | Define um título visível para um elemento <details>
<time>	    | Define uma data/hora
<wbr>	      | Define uma possível quebra de linha
<datalist>	| Lista opções predefinidas para controles inputs
<keygen>	  | Define um campo de gerador de par de chaves (para formulários)
<output>	  | Define o resultado de um cálculo
<canvas>	  | Define um desenho gráfico usando JavaScript
<svg>	      | Define um desenho gráfico usando SVG
<audio>	    | Define um conteúdo de som ou música
<embed>	    | Define um contêiner para aplicações externas (como plug-ins)
<source>	  | Define fonte para <video> e <audio>
<track>	    | Define faixas para <video> e <audio>
<video>	    | Define um conteúdo de vídeo
  
### O que mais mudou?

Quando escrevemos documentos em HTML5, uma das primeiras novidades é a declaração *doc type*, que foi simplificada para ```<!DOCTYPE HTML>```. Lembre-se de que esta declaração é necessária para informar ao navegador que estamos trabalhando com HTML.

#### Formulários

Os formulários em HTML5 agora são mais completos para a experiência do usuário. Foram adicionados seletores de cores, datas e controles numéricos, por exemplo. Os inputs agora incluem também os tipos de e-mail, pesquisa, url, range, número etc.

Para entender a importância desses novos tipos de inputs, você deve lembrar que os formulários que não os possuíam não faziam a verificação de dados. Isso significa, basicamente, que o HTML em si não verificava os dados ineridos, como, por exemplo, se os endereços de e-mail estavam sendo inseridos corretamente.
