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

    <p **align="center"**>
      Este texto está alinhado no centro.
     </p>
   
Neste exemplo, o valor **center** indica que o conteúdo dentro do elemento *p* deve ser alinhado no centro. Os atributos sempre são especificados na tag de abertura, e sua estrutura geralmente é ``**nome="valor"**``.

#### Atributo de tamanho

Nós também podemos mudar o tamanho de uma ```div`` ou outra tag HTML (não todas) incluindo o atributo **width**.

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

    <img src="imagem.jgp" width="50px" **border**="1px" alt="" />
    
#### A tag ``<a>``

Links são uma parte importante do conteúdo na internet. Você pode adicionar links aos textos ou imagens, que redirecionarão os usuários que clicarem para outro arquivo ou site. No HTML, os links são definidos pela tag ``<a>``.

    <a href="">Nome do link</a>
    
##### O atributo ``target``

O atributo ´´´target´´ permite especificar onde abrir o link. Se colocarmos o valor **_blank**, o link abrirá em uma nova janela ou guia.

    <a href="" target="_blank">Nome do link</a>
