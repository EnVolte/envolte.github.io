---
layout: curso
title:  "Curso de HTML & CSS (Parte 4)"
subtitulo: "Formulários, tipos de inputs e métodos de envio."
date:   2018-06-28 12:00:00
categories: HTML e CSS
---

Na [última aula](https://envolte.github.io/curso/2018/06/27/curso-html-css-parte-3.html), aprendemos algumas tags em HTML e estruturamos o código de uma página simples toda em HTML. O execício que eu deixei foi que você construísse a página à sua maneira, fizesse seu próprio menu e dividisse o conteúdo como quisesse. Você conseguiu? Conte aí nos comentários!

Nesta 4ª parte, vamos aprender sobre os **formulários**. Não pense que eles se limitam aos de contato. Sempre que você vir uma caixa de texto, barra de busca ou uma página de login, ele estará lá. Também são usados para preencher informações sobre os usuários, como em um formulário de cadastro, por exemplo. Os usos são diversos, mas uma coisa é certa: os formulários são de suma importância para o mundo da programação. Se você está acompanhando o [**Curso de PHP**](https://envolte.github.io/Curso-PHP.html), verá que eles aparecerão ao longo do curso para dinamizar as páginas.

### O elemento ``<form>``

Os formulários são definidos usando a tag ``<form>``, que possui abertura ``<>`` e fechamento ``</>``.

    <body>
      <form></form>
    </body>
    
O atributo **action** serve para indicar a página que receberá os dados após o usuário enviar o formulário.

    <form action="/recebedados.php">
    </form>
    
#### Os atributos ``method`` e ``name``

Estes atributos especificam o método HTTP (**GET** ou **POST**) que serão usados quando o formulário é enviado. Quando usamos **GET**, os dados do formulário serão passados pela URL, ou seja, ficarão visíveis. Use **POST** se os dados enviados incluem informações sensíveis, como senhas. Este tipo de envio oferece mais segurança porque os dados não ficam visíveis no endereço da página.

O atributo **name** especifica o nome do formulário. Para pegar as informações, como em PHP, por exemplo, é preciso que o nome corresponda com os elementos do *input*.

O elemento ``<input>`` tem muitas variações dependendo do atributo. Pode ser um *campo de texto*, *senha*, *radio* (escolha), *URL*, *submit* (enviar) etc.

    <form action="#" method="POST">
      <input type="text" name="usuario" />
      <input type="password" name="senha" />
    </form>
    
Se o método ficar em branco, ou usarmos uma ``#``, a ação acontecerá na mesma página do formulário.
    
#### Elementos de formulário

Se usarmos um *input* de tipo **radio** (não confunda com rádio), poderemos criar um formulário do tipo de escolha, onde  é possível escolher apenas um ítem. Veja:

    <input type="radio" name="genero" value="masculino" /> Masculino
    <input type="radio" name="genero" value="feminino" /> Feminino
    
Repare que os dois inputs possuem o mesmo valor em *name*. Isso porque é preciso saber qual foi o ítem marcado na hora de pegarmos a informação passada pelo nome "genero".

O tipo "checkbox" permite que o usuário escolha mais de uma opção.

    <input type="checkbox" name="comidas" value="doces" /> Doces
    <input type="checkbox" name="comidas" value="salgados" /> Salgados
    
O botão de envio manda um formulário para o endereço ou página informados no atributo *action*. Esse tipo de input é obrigatório para que seu formulário funcione corretamente, afinal, sem ele não há como mandar os dados, não é?

    <input type="submit" value="Enviar" />
    
### Exercício

Sua tarefa agora é criar um formulário de contato completo em HTML. Crie um arquivo chamado *formulario.html* e adicione os campos *nome*, *e-mail*, *mensagem* e o input *submit*. Você pode acrescentar mais inputs se quiser. Não se esqueça de que o formulário deve ficar dentro da tag *body*, e que deve ser feita uma página com todas tags básicas (*html*, *head* e *body*).
