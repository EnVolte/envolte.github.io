---
layout: post
title:  "Curso de HTML & CSS (Parte 3)"
date:   2018-06-27 07:00:00
categories: Curso
---

Agora, que já iniciamos o desenvolvimento da nossa página e aprendemos mais algumas tags em HTML, não podemos parar por aqui. Até o fim deste post, você deve aprender a **criar menus** (ainda simples) e dividiremos melhor o layout de nosso site com a separação por ``divs``. Por enquanto, iremos fazer o site de forma habitual, e só utilizaremos as tags **HTML5** nas próximas aulas, quando aprenderemos um pouco mais sobre elas.

Se você fez o exercício da aula anterior, deve ter percebido que nossa página ainda está sem identidade alguma. Isso, porque não inciamos a parte de **CSS** ainda. Ela também está bem crua, de modo que parece mais um texto, do que um site. Agora, vamos aprender sobre mais alguns itens antes de incluí-los no layout. Leia com atenção!

### Atributos HTML

Atributos proveem informações adicionais sobre um elemento ou tag, enquanto também modificam eles. Os atributos tem um valor; o valor modifica os atributos.

    <p align="center">
      Este texto está alinhado no centro.
     </p>
   
Neste exemplo, o valor **center** indica que o conteúdo dentro do elemento *p* deve ser alinhado no centro. Os atributos sempre são especificados na tag de abertura, e sua estrutura geralmente é ``nome="valor"``.

#### Atributo de tamanho

Nós também podemos mudar o tamanho de uma ``div`` ou outra tag HTML (não todas) incluindo o atributo **width**.

    <hr width="100px">
    <!-- width = largura -->
   
Neste exemplo, mudamos a largura da linha horizontal criado pela tag **hr**. Você também pode usar valores com porcentagens.

    <hr width="100%">
   
Isso irá fazer que a linha se estenda pela tamanho total da parte onde ela foi colocada.

#### Atributo ``align``

Como vimos mais acima, o atributo **align** é usado para especificar onde o texto é alinhado. Mais pra frente, veremos que ele também funciona com imagens. Seus valores são **left**, à esquerda, **center**, no centro, e **right**, à direita.

E se colocarmos atributos contrários no mesmo elemento?

    <p align="center">
      Isso é um texto
        <hr width="100px" align="left">
    </p>
    
Consegue imaginar este resultado? Teste em seu projeto e me conte o que aconteceu!

#### A tag ``<img>``

Se você for esperto, deve ter pecebido que esta tag é usada para inserir imagens. Ela contém apenas atributos, e não tem tag de fechamento. A URL (endereço) da imagem é definida utilizando o atributo **src**. A sintaxe é:

    <img src="imagem.jpg" />
    
No caso de sua imagem não ser mostrada, seja por um erro de carregamento ou endereço errado, o atributo **alt*, que significa "texto alterativo", descreve a sua imagem em palavras.

    <img src="imagem.jpg" alt="Aqui fica a descrição" />
    
##### Tamanho da imagem

Para definir o tamanho de uma imagem, use os atributos **width** e **height**, largura e altura, respectivamente. O valor pode ser especificado em *pixels* ou *porcentagem*.

    <img src="imagem.jpg" width="50%" height="50%" alt="" />
    <!-- ou -->
    <img src="imagem.jpg" width="50px" height="50px" alt="" />
    
**Dica**: Se sua imagem não for quadrada, é recomendado que você use apenas o atributo *width*, para não deformá-la.

Carregar imagens leva tempo. Usar imagens pesadas pode fazer sua página demorar para carregar, então use-as com cautela.

##### Bordas em imagens

Por padrão, as imagens não têm borda. Use o atributo **border** para criar uma borda ao redor da imagem.

    <img src="imagem.jgp" width="50px" border="1px" alt="" />
    
#### A tag ``<a>``

Links são uma parte importante do conteúdo na internet. Você pode adicionar links aos textos ou imagens, que redirecionarão os usuários que clicarem para outro arquivo ou site. No HTML, os links são definidos pela tag ``<a>``.

    <a href="">Nome do link</a>
    
##### O atributo ``target``

O atributo ´´target´´ permite especificar onde abrir o link. Se colocarmos o valor **_blank**, o link abrirá em uma nova janela ou guia.

    <a href="" target="_blank">Nome do link</a>
    
### Listas ordenadas

Uma lista ordenada inicia com ``<ol>``, e cada elemento listado é definido pela tag ``<li>``.
    
    <ol>
        <li>Primeiro</li>
        <li>Segundo</li>
        <li>Terceiro</li>
    </ol>

Este código resultará em uma lista com itens ordenados automaticamente por números (1, 2, 3).

### Listas não-ordenadas

Uma lista não-ordenada começa com a tag ``<ul>``. Os itens desta lista serão marcados por bolinhas.

    <ul>
        <li>Azul</li>
        <li>Verde</li>
        <li>Amarelo</li>
    </ul>
    
### Criando uma tabela

As tabelas servem para organizar conteúdo em uma página. São definidas pela tag ``<table>``. As tabelas são dividas em linhas com a tag ``<tr>``, que significa "table row", ou *fileira da tabela*. As linhas são divididas em colunas com a tag ``td``, "table data", ou *dados da tabela*.
    
    <table>
        <tr><!-- Inicia uma linha -->
            <td></td><!-- Uma coluna -->
        </tr><!-- Fecha uma linha -->
    </table>
    
#### Bordas e o atributo Colspan
 
 Uma borda pode ser adicionada utilizando o atributo ``border``.
 
        <table border="2">
        
##### Colspan
 
Se você testar o código da nossa tabela, perceberá que ela é bem divida. Porém, se você colocar, por exemplo, uma fileira com apenas uma divisão, enquanto as outras têm 2 ou mais, ela ocupará apenas o seu tamanho, e isso pode ser um incomodo.

O atributo ``colspan``, "col" de *coluna*, e "span", de ocupação, pode fazer a célula da sua coluna ocupar dois ou mais espaços.

        <table border="2">
            <tr>
                <td>Azul</td>
                <td>Verde</td>
                <td>Amarelo</td>
            </tr>
            <tr>
                <td>Cor 1</td>
                <td colspan="2"></td><!-- Indicamos que ela deve usar o tamanho de duas colunas -->
            </tr>
            
Para fazer uma fileira se adaptar a mais de uma coluna, utilizamos o atributo ``rowspan`` na tag **<tr>**. Isso significa, basicamente, que uma fileira vai se adaptar ao número de colunas. O número de colunas deve ser o valor do atributo.

#### Os atributos ``align`` e ``bgcolor``

Para mudar a posição de nossa tabela, use o atributo ``align`` dentro da tag. Os valores são os mesmos ensinados acima. Já se você quer especificar a cor de fundo de uma coluna, por exemplo, use o atributo ``bgcolor``.

### Tipos de elementos

Em HTML, a maioria dos elementos é definida como "elementos em blocos" ou "elementos em linha". Os elementos em blocos iniciam em uma nova linha.

> **Por exemplo**: ``<h1>``, ``<form>``, ``<ul>``, ``<li>``, ``<ol>``, ``<p>``, ``<table>``, ``<div>`` etc.

Os elementos em linha são normalmente exibidos na mesma linha.

> **Por exemplo**: ``<b>``, ``<a>``, ``<strong>``, ``<img>``, ``<span>`` etc.

O elemento ``<div>`` é um elemento de bloco que quase sempre é usado como container para outros elementos em HTML. Quando usamos com um pouco de CSS, que veremos mais adiante, este elemento pode ser usado como bloco de estilo para o conteúdo.

        <html>
        <body>
        <h1>Cabeçalho</h1>
        <div style="color: white; background-color: blue; padding: 15px;"><!-- Inicia div -->
        <p>Isto é uma frase.</p>
        </div>
        </body>
        </html>
        
Neste caso, todo o conteúdo dentro da ``div`` possuirá fundo azul, cor de texto branca e espaçamento de 15 pixels.

Parecido, o elemento ``<span>`` é um *elemento em linha* que é muito utilizado como container para um texto. Quando usamos junto com CSS, podemos estilizar parte de um texto.

        <html>
        <body>
        <h2>Aprendendo sobre span</h1>
        <p>Preservem nossa <span style="color: green;">Amazônia</span></p>
        <p>Isto é uma frase.</p>
        </body>
        </html>
        
Teste este código e você verá que a palavra **Amazônia** ficou da cor verde.

> ### Resumo
>
> O elemento **div** define uma *seção em nível de blocos*.
>
> O elemento **span** define uma *seção em linha*.

### Tipos de elementos

Outros elementos podem ser usados como *elementos em bloco*. Isso inclui os seguintes:

* **APPLET**: Miniaplicativo Java embutido.
* **IFRAME**: Uma frame (quadro) de alguma coisa.
* **INS**: Texto inserido.
* **MAP**: Mapeamento de imagem.
* **OBJECT**: Um objeto embutido.
* **SCRIPT**: Um script dentro do HTML.

Agora que já aprendemos mais um pouco, vamos iniciar o desenvolvimento da nossa página. Lembra que no começo do post eu prometi ensinar a fazer **menus simples** e **dividir** o conteúdo? Vamos colocar isso em prática!
