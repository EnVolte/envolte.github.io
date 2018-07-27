---
layout: curso
title:  "Curso de PHP (Parte 4)"
subtitulo: "Arrays (vetores), arrays numéricos, associativos e multimensionais."
date: 2018-07-05 15:00:00
categories: PHP
---

Na [3ª parte do Curso de PHP](https://envolte.github.io/cursos/PHP/parte-3), ensinei sobre os *Operadores aritiméticos*, *Operadores de atribuição*, *Operadores de comparação* e *Operadores lógicos*. Agora, as coisas vão começar a complicar um pouco com a chegada dos **vetores**, mais conhecidos como *arrays*. Apesar de o curso ser básico, e com objetivo de introduzir ao desenvolvimento de sites dinâmicos com PHP, todo este conteúdo que estamos vendo é de suma importância para o aprendizado *intermediário* e *avançado*. PHP não é uma linguagem de programação difícil de ser aprendida, mas exige que prestemos atenção. As linguagens de programação são como os idiomas; quanto mais praticamos, mais rápido estaremos "fluentes".

### O que são vetores?

Os **vetores**, ou *arrays*, são variáveis especiais que podem conter mais de um valor ao mesmo tempo. Na verdade, pode ser descrito como um mapa ordenado. Um mapa é um tipo que relaciona valores a chaves. Pode ser tratado como um array, uma lista (vetor), hashtable (que é uma implementação de mapa), dicionário, coleção, pilha, fila etc.

Por exemplo, se nós tivéssemos uma lista (como uma de chamada), os ítens em variáveis únicas ficariam assim:

```
$nome1 = "Bianca";
$nome2 = "Enio";
$nome3 = "Luciana";
$nome4 = "Marina";
```

Até aí, tudo bem. Mas e se estivermos trabalhando com mais de 50, 100 valores? Não dá para criar uma variável para cada um, já que isso se tornaria algo cansativo. A solução: crie um *array*! Para fazer isso, use a função **array()** do PHP. Mas antes, vamos conhecer um pouco mais sobre cada tipo.

#### Array numérico

Arrays numéricos, ou arrays indexados, associam um índex numérico para cada valor. O seu índex pode ser definido automaticamente (sempre iniciam a partir de **0**). Vamos a um exemplo:

```
$nomes = array("Bianca", "Enio", "Luciana", "Marina"); // Repare que todos os valores ficam separados por aspas e vírgula.
```

Como alternativa, você pode definir os valores manualmente.

```
$nome[0] = "Bianca";
$nome[1] = "Enio";

// Nós definimos um array chamado '$nome', que contém 2 valores.
```

Para acessá-los, é fácil. Podemos fazer isso através de seus índices.

```
print_r ($nome[1]); // Retorna "Enio"
```

Note que fiz o uso da função ```print_r``` ao invés de ```echo```. Isso, porque o PHP não faz a conversão de arrays para strings através dessa função. Com o *print_r*, podemos ver a estrutura do vetor e seus índices. Você verá mais a seguir.

> **Não se esqueça**: os índices começam a partir de **0**, não de *1*!

A partir deste momento, acredito que você esteja com seu servidor PHP ligado e testando todas as funções que estou ensinando. Não se esqueça de que a prática ajuda a fixar o conteúdo.

> Se você está usando o **EasyPHP**, tem uma ferramenta muito legal que pode descomplicar os testes em códigos PHP. Ao ligar seu servidor local, procure por *code tester*. Aqui no meu computador fica em [http://127.0.0.1:1111/codetester.php](http://127.0.0.1:1111/codetester.php).

<figure>
  <img src="https://envolte.github.io/arquivos/fotos/php01.png" width="auto" />
  <figcaption>Todo o código em PHP é interpretado ao clicar no botão 'interpret'. Note que a estrutura do array foi mostrada com o uso da função print_r, citada acima.</figcaption>
  </figure>
  
Você pode ter números inteiros, strings e outros tipos de dados juntos em um array.

```
<?php
  $array[0] = "Fernando";
  $array[1] = "<em>ensinou</em>";
  $array[2] = "21 + 30"; // Dentro das aspas, o valor passa a ser uma string
  $array[3] = 21 + 30; // Fora das aspas, o valor é interpretado como inteiro
  
  echo $array[0]. " me " .$array[1]. " que a soma de " .$array[2]. " é " .$array[3];
?>
```

Resultará em:

"Fernando me *ensinou* que a soma de 21 + 30 é 51"

Neste exemplo, repare que fiz o uso de ```echo```. Isso foi possível porque pegamos cada valor de nosso vetor individualmente, como  strings. Para exibir o resultado, também usei o operador de concatenação "**.**", ligando as strings às variáveis. Se você ficou com dúvida aqui, volte um pouco o curso que eu explico mais sobre esse operador.
