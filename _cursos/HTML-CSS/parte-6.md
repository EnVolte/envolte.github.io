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
&#60;figcaption&#62;	|	Define uma legenda para um elemento <figure>
&#60;figure&#62;		  | Define um conteúdo como ilustrações, diagramas, fotos, códigos, listagens, etc
&#60;main&#62;		    | Define o conteúdo principal de uma página
&#60;mark&#62;		    | Define um texto marcado ou realçado
&#60;menuitem&#62;		| Define um commando/menu que pode ser usado para invocar um menu popup
&#60;meter&#62;		    | Define uma medida escalar dentro de uma faixa conhecida
&#60;progress&#62;		| Define o progresso de uma tarefa
&#60;rp&#62;		      | Define o que exibir em navegadores que não exibem anotações<br>ruby (anotações ruby são para mostrar a pronúncia de caracteres do Leste Asiático.)
&#60;rt&#62;		      | Define a pronúncia de um caractere (para tipografias do Leste Asiático)
&#60;ruby&#62;		    | Define uma anotação ruby (para tipografia do Leste Asiático)
&#60;summary&#62;		  | Define um título visível para um elemento <details>
&#60;time&#62;		    | Define uma data/hora
&#60;wbr&#62;		      | Define uma possível quebra de linha
&#60;datalist&#62;		| Lista opções predefinidas para controles inputs
&#60;keygen&#62;		  | Define um campo de gerador de par de chaves (para formulários)
&#60;output&#62;		  | Define o resultado de um cálculo
&#60;canvas&#62;		  | Define um desenho gráfico usando JavaScript
&#60;svg&#62;		      | Define um desenho gráfico usando SVG
&#60;audio&#62;		    | Define um conteúdo de som ou música
&#60;embed&#62;		    | Define um contêiner para aplicações externas (como plug-ins)
&#60;source&#62;		  | Define fonte para &#60;video&#62 e &#60;audio&#62;
&#60;track&#62;		    | Define faixas para &#60;video&#62; e &#60;audio&#62;
&#60;video&#62;		    | Define um conteúdo de vídeo
  
### O que mais mudou?

Quando escrevemos documentos em HTML5, uma das primeiras novidades é a declaração *doc type*, que foi simplificada para ```<!DOCTYPE HTML>```. Lembre-se de que esta declaração é necessária para informar ao navegador que estamos trabalhando com HTML.

#### Formulários

Os formulários em HTML5 agora são mais completos para a experiência do usuário. Foram adicionados seletores de cores, datas e controles numéricos, por exemplo. Os inputs agora incluem também os tipos de e-mail, pesquisa, url, range, número etc.

Para entender a importância desses novos tipos de inputs, você deve lembrar que os formulários que não os possuíam não faziam a verificação de dados. Isso significa, basicamente, que o HTML em si não verificava os dados ineridos, como, por exemplo, se os endereços de e-mail estavam sendo inseridos corretamente.
