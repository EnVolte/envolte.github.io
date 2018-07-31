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

Até aí, tudo bem. Mas e se estivermos trabalhando com mais de 50, 100 valores? Não dá para criar uma variável para cada um, já que isso se tornaria cansativo. A solução: crie um *array*! Para fazer isso, use a função **array()** do PHP. Mas antes, vamos conhecer um pouco mais sobre cada tipo.

#### Array numérico

Arrays numéricos, ou arrays indexados, associam um índex numérico para cada valor. O seu índex pode ser definido automaticamente (sempre iniciam a partir de **0**). Vamos a um exemplo:

```
$nomes = array("Bianca", "Enio", "Luciana", "Marina"); // Repare que todos os valores ficam separados por aspas e vírgula.
```

Como alternativa, você pode definir os índices manualmente.

```
$nome[0] = "Bianca";
$nome[1] = "Enio";
// Nós definimos um array chamado '$nome', que contém 2 valores.
```

Para acessá-los, é fácil. Podemos fazer isso chamando o nome do *array* com o seu índice dentro de colchetes.

```
print_r ($nome[1]); // Retorna "Enio"
```

Note que fiz o uso da função ```print_r``` ao invés de ```echo```. Isso, porque o PHP não faz a conversão de *arrays* para *strings* através dessa função. Com o *print_r*, podemos ver a estrutura do vetor e seus índices. Note que, neste caso, era possível fazer uso de ```echo```, porém introduzi a esta função para futuros testes em que chamamos o array de forma habitual (sem o índex). Você verá mais sobre isso a seguir.

> **Não se esqueça**: os índices começam a partir de **0**, não de **1**!

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

**Resultado**:

"Fernando me *ensinou* que a soma de 21 + 30 é 51"

Neste exemplo, repare que fiz o uso de ```echo```. Isso foi possível porque pegamos cada valor de nosso vetor individualmente, como  strings. Para exibir o resultado, também usei o operador de concatenação "**.**", ligando as strings às variáveis. Se você ficou com dúvida aqui, volte um pouco o curso que eu explico mais sobre esse operador.

#### Arrays associativos

Arrays associativos são vetores que usam *nomes* como *chaves* que você associa aos valores. Existem duas maneiras de criar um:

```
<?php
  $animais = array("Cachorro" => "caninos", "Gato" => "felinos");
  // Ou
  $animais['Cachorro'] = "caninos";
  $animais['Gato'] = "felinos";
?>
```

> No primeiro exemplo, note o uso de **=>** para associar os valores às respectivas chaves.

Mas como eu faço para pegar o valor deste vetor? Simples, use suas chaves nominais, como nos *arrays númericos*.

```
echo "O cachorro faz parte dos " .$animais['Cachorro'];
// Retorna "O cachorro faz parte dos caninos"
```

E se usassemos ```echo $animais;```? Faça o teste e você verá que o PHP retornará um erro informando que não é possível fazer a conversão de arrays para strings, como mencionado anteriormente. Neste caso, use a função ```print_r```.

<figure>
  <img src="https://envolte.github.io/arquivos/fotos/php02.png" width="auto" />
  <figcaption>Arrays associativos sendo exibidos de duas formas: a primeira com o comando 'echo', e a segunda com 'print_r'.</figcaption>
  </figure>

#### Arrays multidimensionais

Um array multidimensional é um vetor que contém mais de um array, ou seja, um vetor dentro de outro. A dimensão de um array indica o número de índices que serão precisos para selecionar um elemento. Podemos construir uma estrututa com diversas dimensões, mas as que ultrapassam 3 níveis são mais difíceis de serem gerenciadas.

- Para um array de 2 dimensões (bidimensional), usa-se 2 índices para selecionar um elemento;
- Para um array de 3 dimensões (tridimensional), usa-se 3 índices para selecionar um elemento e assim por diante.

Para entender melhor como funciona, vamos a um exemplo prático de um array bidimensional.

```
$pessoas = array( // Array bidimensional
  'formados' => array('João', 'Maria'), // Primeiro array
  'cursando' => array('José', 'Alexandre'), // Segundo array
  'desistentes' => array('Mario', 'Paulo') // Terceiro array
);
```

Se você prestar bastante atenção, se questionará o por quê de termos **3** arrays dentro de um outro, se estamos trabalhando com arrays de **duas dimensões**. Isso pode ser um pouco confuso, mas é bem fácil de entender.

O primeiro array, na verdade, é a base do *array multidimensional*. Para trabalhar com esse tipo de vetores, é preciso entender que o seu tamanho não é contado por número de arrays, e sim por dimensões. Dentro do array *pessoas* temos três outros arrays, *formados*, *cursando* e *desistentes*. Este array é bidimensional porque trabalha com dois níveis, ou seja, nós temos três arrays *filhos* dentro de um array *pai*.

Para exibir seus ítens, podemos fazer de duas formas: com o ```print_r``` ou ```echo```.

```
print_r ($pessoas); // Retorna a estrutura do vetor multidimensional

echo $pessoas['formados'][0];
echo $pessoas['cursando'][0];
echo $pessoas['desistentes'][0]; 
// Retorna o primeiro valor (índice 0) do primeiro vetor de cada array
```

**Com a função** ```print_r```, **teremos**:

Array ( [formados] => Array ( [0] => **João** [1] => **Maria** ) [cursando] => Array ( [0] => **José** [1] => **Alexandre** ) [desistentes] => Array ( [0] => **Mario** [1] => **Paulo** ) )

Com ```echo $pessoas['formados'][0];```, nós teremos "João" como resultado. A função ```echo``` sempre funciona quando estamos exibindo um ítem de vetor por vez. Entre colchetes, especificamos o array "formados", e o índice, que é **0**. Para que você possa entender melhor, vou exemplificar em uma tabela.

Formados | Cursando | Desistentes
---------|----------|------------
João     |José      |Mario
Maria    |Alexandre |Paulo

As três colunas representam os três *arrays*. O array é bidimensinal porque os três vetores estão dentro do array principal, *$pessoas*. Também pode ser chamado de array de duas dimensões.

Os arrays tridimensionais são aqueles que possuem três níveis hierárquicos, ou seja, um array, dentro de dois outros arrays. A estrutura funciona de forma parecida com a dos arrays de duas dimensões, veja:

```
$supermercado = array( // Array tridimensional
  'produtos' => array( // Array bidimensional
    'ofertas' => array('frutas', 'legumes'), // Primeiro array
    'normal' => array('carne', 'verduras') // Segundo array
  ),
);
```

Criamos um array chamado ```supermercado```, e dentro dele temos outro array, chamado ```produtos```, que possui outros dois arrays no mesmo nível. Para acessar este vetor, ao invés de 2 índices, você precisará de 3. Esse valor deverá ser maior ou menor de acordo com o número de dimensões.

```
echo $supermercado['produtos']['ofertas'][1]; // Retornará "legumes"
```

Se você quiser saber mais sobre arrays, acesse o [Manual do PHP](https://secure.php.net/manual/pt_BR/language.types.array.php).

Encontrou algum erro ou gostaria de sugerir uma mudança? Comente abaixo!
