---
layout: curso
title:  "Curso de HTML & CSS (Parte 5)"
subtitulo: "Cores em HTML."
date:   2018-07-28 12:00:00
categories: HTMLCSS
---

Na [última parte do curso](https://envolte.github.io/curso/HTML-CSS/parte-4/), falei sobre os f*ormulários*, *tipos de inputs* e *métodos de envio*. Agora, que entramos em uma parte essencial para o desenvolvimento, precisamos saber como manipular e enviar informações, bem como construir a estrutura de uma página completa. Foi explicado o que são *divs*, como *separar o conteúdo*, e você já deve saber como funciona a estrutura básica de uma página. Tudo isso é essencial para que qualquer site possa ir ao ar, e que não tenhamos nenhum problema com algo tão básico, mas necessário, como o **HTML**.

Agora, iremos entrar um pouco na parte de *estilização*. Mas calma, ainda não vamos focar em **CSS**. Nesta 5 parte, vou ensinar a usar as cores em HTML. Este recurso funciona da mesma forma em CSS, mas como ainda estamos focados em HTML, começaremos por aqui.

<section id="quadro">
<label>Índice</label> <button class="openclose">Abrir/Fechar</button>
<div class="linha"></div>
<section id="indice">
<ol><!-- indice -->

<li><a href="#01">As cores</a></li>
<li><a href="#02">Cores em RGB</a></li>
<li><a href="#03">Infográfico</a></li>
<li><a href="#04">Atributos 'bgcolor' e 'color'</a></li>
<li><a href="#05">Exercícios</a></li>

</ol>
</section>
</section><br>

<span id="01"></span>
As cores são essenciais nos websites, assim como são essenciais na vida. Sem cores, uma página ficaria sem vida e difícil de ler. Por padrão, os navedores interpretam os textos sem formatação com a cor **preta**. Você deve ter pecebido isso enquanto fazia alguma de nossas atividades. Elas também podem estar presentes em imagens, bordas, menus, links, blocos de conteúdo e, até mesmo, no plano de fundo de um site.

<span id="02"></span>
### Cores em RGB

Os valores *hexadecimais* (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F) representam a formação de todas as cores. São **16** valores, porém, nenhum acima de **F**, que representa o maior valor. As cores são mostradas em uma combinação de **red** (vermelho), **green** (verde) e **blue** (azul), o famoso **RGB**. São escritas usando uma cerquilha (**#**), seguida por três ou seis caracteres. Juntos, esses valores podem alcançar mais de 16 milhões de combinações. É muita coisa, não?

<span id="03"></span>
<figure><img src="https://envolte.github.io/arquivos/fotos/cores.png" width="auto" />
  <figcaption>Entenda melhor com este infográfico.</figcaption>
</figure>

No infográfico acima, referenciei as principais cores em RGB (vermelho, verde e azul), assim como as mais básicas, que são o **preto** e o **branco**. Mas, como descrito acima, nós podemos fazer misturas e variações de cores para atingir um resultado que mais nos agrade. As possibilidades são quase infinitas, mas não se preocupe em gravar o número de todas as cores.

<span id="04"></span>
### Atributos ``bgcolor`` e ``color``

Nós sabemos que é possível estilizar qualquer elemento em HTML através de uma *folha de estilos*. Porém, como ainda não entramos na parte do CSS, e não iremos fazer o uso do atributo ```style```, existe uma maneira mais prática de mudar a cor de um plano de fundo ou de uma fonte com o ```bgcolor``` e ```color```.

```
<html>
  <head>
  <title>Exemplo</title>
  </head>
    <body bgcolor="#000000">
      <h1><font color="#FFFFFF">Cabeçalho na cor branca</font></h1>
    </body>
</html>
```

Se você testar o código acima, verá que criamos um documento com o fundo **preto** e o cabeçalho **branco**.

<span id="05"></span>
### Exercício

Nas próximas partes falaremos mais sobre as cores, e outras formas de incluí-las, quando entrarmos em **CSS**. Por enquanto, você pode treinar com o exercício a seguir. 

O exercício proposto é você **criar uma página de contato com um formulário** (com quantos campos você quiser), titulo (**h1**), um texto de instruções sobre como preencher e mudar o plano de fundo com alguma cor. Aproveite bem o que foi ensinado nestas duas últimas partes!

Para que você não se confunda, basta seguir a lista:

- Crie uma página com todos os elementos em HTML essenciais.
- Separe o conteúdo dentro do ```body``` com *divs*.
- Crie um titulo com ```h1``` para a sua página (acima do texto) com uma cor de destaque.
- Faça um texto com a tag ```p``` (uma para cada parágrafo) e destaque as palavras importantes com outra cor. Você pode pesquisar cores hexadecimais na internet e escolher uma.
- Crie um formulário em HTML com os campos que quiser, e não se esqueça do botão de envio.

Se você ficar com alguma dúvida, ou tiver algum problema com o exercício, deixe seu comentário abaixo.
