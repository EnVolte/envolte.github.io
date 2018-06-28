---
layout: post
title:  "Curso de PHP (Parte 3)"
date:   2018-06-28 10:00:00
categories: Curso
---

Agora, que já aprendemos um pouco sobre como escrever *variáveis*, vamos dar prosseguimento ao curso. Espero que você tenha feito os exercícios práticos que sugeri na aula passada, pois eles são de grande ajuda para o aprendizado, já que as variáveis estão presentes em todo o código PHP, como você verá nos próximos posts.

Nesta 3 parte do nosso curso, vamos aprender sobre os **Operadores aritiméticos**, **Operadores de atribuição**, **Operadores de comparação** e **Operadores lógicos**. Estes operadores são de grande ajuda quando estamos desenvolvendo um projeto, pois são responsáveis por *somar*, *juntar*, *comparar*, *atribuir resultados* etc.

Gostaria de lembrar que este é um *curso básico* para quem tem interesse iniciar no mundo da programação. O **PHP** é uma linguagem realmente muito *poderosa*, e você vai se surpreender em como é fácil aprender. Se você ainda não fez a sua inscrição, [cadastre-se aqui](https://envolte.github.io/Curso-PHP.html). Por mais que não haja necessidade de estar inscrito para ver o conteúdo, isso me dá uma base do alcance do meu curso. Nesta página, você também pode dar a sua sugestão, crítica e contribuir para que o aprendizado possa se tornar muito mais proveitoso.

### Operadores arítiméticos

Como o próprio nome já diz, estes são operadores que realizam operações matemáticas. Os **operadores aritiméticos** funcionam com valores numéricos para realizar operações comuns. Veja:

  Operador   |   Nome   |   Exemplo
:----------: | :------: | :---------:
+            |Adição    |   $x + $y
-            |Subtração |   $x - $y
*            |Multiplicação| $x * $y
/            |Divisão   |   $x / $y
%            |Módulo    |   $x % $y

Abra seu programa, ligue o **Apache** e crie um arquivo chamado *operacoes.php*. Digite o seguinte código:

    <?php
      $num1 = 10;
      $num2 = 8;
      
      // Adição
      echo $num1 + $num2; // 18
      
      // Subtração
      echo $num1 - $num2; // 2
      
      // Multiplicação
      echo $num1 * $num2; // 80
      
      // Divisão
      echo $num1 / $num2; // 1,25
    ?>
      
Como eu disse acima, as *variáveis* estão presentes no código a todo instante, por isso é importante se familiarizar com elas. Não se esqueça de sempre fechar com ``;`` para não causar nenhum erro. 

Quando usamos o comando ``echo``, normalmente ele é acompanhado de aspas simples ``'`` ou aspas duplas ``"``. Porém, se estivermos trabalhando com variáveis, não precisamos colocar.

#### Módulo

O operador de **módulo**, representado pelo sinal **%**, retorna o valor restante da divisão entre dois números. 

Caso não tenha entendido bem o que é *módulo*, vou tentar explicar melhor. Se dividirmos o número **14** por **3**, por exemplo, o resultado será **4,6666**... Transformando este número em um número *inteiro*, ficaríamos com **4**. **3 x 4 = 12**. O que resta? Isso mesmo, **2**, que é o nosso módulo. Veja em prática:

    <?php
      $x = 14;
      $y = 3;
      echo $x % $y; // 2
    ?>
    
> Se você usar números com pontos (float) com o operador de módulo, eles serão convertidos em **inteiros** antes da operação.

#### Incremento & Decremento

O operador de **incremento** é usado para incrementar o valor de um variável. O operador de **decremento** é usado para decrementar (diminuir) o valor de uma variável.

    $x++; // Equivale a $x = $x+1;
    $x--; // Equivale a $x = $x-1;
    
Estes operadores podem anteceder ou suceder uma variável.

    $x++; // Pós-incremento
    $x--; // Pós-decremento
    ++$x; // Pré-incremento
    --$x; // Pré-decremento
    
A diferença é que o **pós-incremento** retorna o valor original *antes* de mudar a variável, enquanto o **pré-decremento** muda a variável primeiro, depois retorna o valor.

    $i = 2; $f = $i++; // $i = 3, $f = 2
    $i = 2; $f = ++$a; // $i = 3, $f = 3
    
Por enquanto, será um pouco confuso, mas logo você entenderá como funciona. Não esqueça que a melhor forma de aprender é na prática, então teste todos os códigos aqui no seu editor.

#### Operadores de atribuição

Os **operadores de atribuição** são usados para escrever valores para as variáveis.

    $num1 = 2;
    $num2 = $num;
    
No exemplo acima, foi atribuído o valor **2** à variável **$num1**, e **$num2** recebeu o valor de **$num1**.

Também podem ser usados em conjunto com os operadores aritiméticos, facilitando o código. Veja:

Exemplo | Mesmo que... | Tipo
:------:|:------------:|:-----:
x += y  | x = x + y    |Adição
x -= y  | x = x - y    |Subtração
x &#42;= y  | x = x * y    |Multiplicação
x /= y  | x = x / y    |Divisão
x %= y  | x = x % y    |Módulo

#### Operadores de comparação

Esse tipo de operador compara dois valores (números ou string). Geralmente, são usados para fazer declarações condicionais, que vão avaliar entre **TRUE** e **FALSE**, ou verdadeiro e falso.

Operador  |   Nome   |   Exemplo   | Resultado
:--------:|:--------:|:-----------:|--------------------
==        | Igual    | $x == $y    |Retorna *true* se **$x** for <br>igual a **$y**
===       | Idêntico | $x === $y   |Retorna *true* se **$x** for <br>igual a **$y** e do mesmo tipo
!=        | Diferente| $x =! $y    |Retorna *true* se **$x** for <br>diferente de **$y**
<>        | Diferente| $x <> $y    |Retorna *true* se **$x** for <br>diferente de **$y**
!==       | Não idêntico | $x !== $y |Retorna *true* se **$x** e **$y** <br>forem diferentes e não do mesmo tipo
>         | Maior que| $x > $y     |Retorna *true* se **$x** for <br>maior que **$y**
<         | Menor que| $x < $y     |Retorna *true* se **$x** for <br>menor que **$y**
>=        | Maior ou igual| $x >= $y|Retorna *true* se **$x** for <br>maior ou igual a **$y**
<=        | Menor ou igual| $x <= $y|Retorna *true* se **$x** for <br>menor ou igual a **$y**

#### Operadores lógicos


