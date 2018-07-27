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
echo $nome[1]; // Retorna "Enio"
```

