---
layout: post
title:  "Animações em CSS3"
capa: "https://envolte.github.io/arquivos/fotos/jsquery.png"
capaindex: "https://envolte.github.io/arquivos/fotos/index/jsjquery.png"
date:   2018-07-18 16:20:00
categories: CSS3
---

Quando se está desenvolvendo um blog, site ou qualquer outra página na internet, sempre chega o momento de dar o estilo para aquilo que você criou. Geralmente, esta é a primeira parte, quando fazemos um planejamento de como o site será em programas como o Photoshop. Porém, sempre que estamos buscando inspiração para um projeto assim, acabamos nos deparando com algo não planejado que muda, ou atrapalha, todo aquele *rascunho*. Quem já está nesse mundo há um tempo, sabe que é possível fazer praticamente qualquer coisa hoje em dia, o que vale é a imaginação. Mas fica dificíl quando nós queremos algo, mas não sabemos fazê-lo.

Sempre achei que só era possível fazer animações com Javascript, que, como já sabemos, é uma popular linguagem de programação frequentemente utilizada para manipular elementos em HTML e CSS, fazer efeitos nas páginas etc. Nem sempre tenho a oportunidade de testar novas configurações e explorar a fundo todos os recursos que o CSS3 nos proporciona, mas acho que as *keyframes* fazem parte de uma lista de "comandos secretos" que deveria ser mais valorizada e conhecida pelos desenvolvedores e web designers.

### Mas por que eu deveria usar isso?

Hoje em dia, praticamente qualquer pessoa pode abrir um blog e ficar online, ganhar seguidores, reconhecimento, e até mesmo *dinheiro*. Sempre que fazemos uma busca no bom e velho **Google**, encontramos uma dúzia de resultados semelhantes. Nós sempre temos aquela dúvida de em qual link entrar, não é mesmo? Quase sempre avaliamos mais o visual, do que o conteúdo em si. Se um site nos é visualmente mais atraente, acaba ganhando mais respeito do que os outros, e isso acaba sendo uma estratégia de SEO. Investir em uma boa aparência é essencial para conquistar leitores. É claro que muitos preferem o conteúdo, do que apenas a aparência, mas quanto mais qualidades tiver, melhor. 

As animações são a parte interativa de uma página, junto aos efeitos de *mouseover*, *mouseout*, *efeito de foco* etc. Os pequenos detalhes chamam a atenção, e por isso é legal investir um pouco de tempo aprendendo isso. Mas também há outra vantagem: as animações em CSS3 são mais fáceis de serem criadas do que as em Javascript. É uma economia de tempo enorme, e estará bem ali, dentro da sua folha de estilos.

### Uma animação básica

Para criar nossa primeira animação, usaremos ```@keyframe exemplo```, onde "exemplo" é o nome que daremos. O código a seguir deve ser incluido na sua folha de estilos (.css)!

    @keyframes exemplo {
    from {background-color: black;} // from = de
    to {background-color: blue;} // to = para
    }

Neste exemplo básico, eu defini que a animação começaria com o fundo preto, indo para o azul. Agora, para que possamos de fato usá-la, devemos incluir uma div que possa executar a *keyframe*.

    div {
    width: 100px;
    height: 100px;
    background-color: blue;
    animation-name: exemplo;
    animation-duration: 5s;}
    
Com o código acima, nós conseguimos o seguinte resultado:

<iframe class="exemplo" src="https://envolte.github.io/exemplos/css/animacao.html" width="100" height="100"></iframe>

Antes de prosseguir, vamos entender duas configurações, o ```animation-name: exemplo;``` e ```animation-duration: 5s;```. No primeiro valor, você deve especificar o **nome** da sua keyframe. Ele precisa ser exatamente igual ao que você deu ali em cima. No segundo, você define o **tempo** da sua animação.

E se eu quiser algo mais complexo? Como eu disse acima, aquele era apenas um exemplo básico. Nós podemos utilizar outras configurações para que nossa animação possa ser bem mais aproveitada.

    @keyframes exemplo {
    0% {background-color: white;}
    25% {background-color: yellow;}
    50% {background-color: red;}
    100% {background-color: black;}
    }
   
    div {
    width: 100px;
    height: 100px;
    background-color: red;
    animation-name: exemplo;
    animation-duration: 10s;
    }
    
Repare que em nosso código agora temos 4 valores (0, 25, 50 e 100), que representam a porcentagem de tempo da animação e o que deve ser executado em cada um deles. Esses valores podem mudar de acordo com suas necessidades.

<iframe class="exemplo" src="https://envolte.github.io/exemplos/css/animacao2.html" width="100" height="100"></iframe>

### O que mais posso fazer?

As *keyframes* não se limitam apenas a mudança de cores. Nós podemos fazer coisas mais legais também, como mudar o seu tamanho, colocar bordas e tudo mais que sua imaginação lhe permitir.

<iframe class="exemplo" src="https://envolte.github.io/exemplos/css/animacao3.html" width="250" height="100"></iframe>

```
div {
width: 100px; 
height: 100px;
background-color: red;
animation-name: exemplo;
animation-duration: 5s;
animation-iteration-count: infinite;
}

@keyframes exemplo {
0% {background-color: blue; width: 100px; border-radius: 0px;}
25% {background-color: orange; width: 150px; border-radius: 2px;}
50% {background-color: brown; width: 200px; border-radius: 5px;}
100% {background-color: black; width: 250px; border-radius: 10px;}
}
```
	
Nos três exemplos eu fiz o uso de ```animation-iteration-count: infinite;```, que repete a animação *infinitamente*. Você pode alterar seu valor para o número de repetições que você preferir.

A propriedade ``animation-direction``

Esta propriedade especifica se a animação deve ser executada *para frente*, *de trás para frente* ou em *ciclos alternados*.

- **normal**: animação é executada de forma padrão (para frente)
- **reverse**: animação é executada de forma reversa (de trás para frente)
- **alternate**: animação é executada de forma **padrão**, depois **reversa** (para frente, de trás para frente)
- **alternate-reverse**: animação é executada de forma **reversa**, depois **padrão** (de trás para frente, para frente)

<iframe class="exemplo" src="https://envolte.github.io/exemplos/css/animacao4.html" width="250" height="100"></iframe>

A propriedade ``animation-timing-function``

Esta propriedade especifica a forma como a animação será executada (velocidade).

- **ease**: começo lento, depois rápido e termina lento
- **linear**: mesma velocidade do começo ao final
- **ease-in**: começo lento
- **ease-out**: final lento
- **ease-in-out**: começo e fim lentos
- **cubic-bezier(n,n,n,n)**: permite que você especifique um valor na função da curva de Bézier

Função | valor
-------|---------
ease   | cubic-bezier(0.25,0.1,0.25,1)
