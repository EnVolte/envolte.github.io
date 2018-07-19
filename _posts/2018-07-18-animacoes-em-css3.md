---
layout: post
title:  "Animações em CSS3"
capa: "https://envolte.github.io/arquivos/fotos/jsquery.png"
capaindex: "https://envolte.github.io/arquivos/fotos/index/jsjquery.png"
date:   2018-07-18 16:20:00
categories: CSS CSS3
---

Quando se está desenvolvendo um blog, site ou qualquer outra página na internet, sempre chega o momento de dar o estilo para aquilo que você criou. Geralmente, esta é a primeira parte, quando fazemos um planejamento de como o site será em programas como o Photoshop. Porém, sempre que estamos buscando inspiração para um projeto assim, acabamos nos deparando com algo não planejado que muda, ou atrapalha, todo aquele *rascunho*. Quem já está nesse mundo há um tempo, sabe que é possível fazer praticamente qualquer coisa hoje em dia, o que vale é a imaginação. Mas fica dificíl quando nós queremos algo, mas não sabemos fazê-lo.

Sempre achei que só era possível fazer animações com Javascript, que, como já sabemos, é uma popular linguagem de programação frequentemente utilizada para manipular elementos em HTML e CSS, fazer efeitos nas páginas etc. Nem sempre tenho a oportunidade de testar novas configurações e explorar a fundo todos os recursos que o CSS3 nos proporciona, mas acho que as *keyframes* fazem parte de uma lista de "comandos secretos" que deveria ser mais valorizada e conhecida pelos desenvolvedores e web designers.

### Mas por que eu deveria usar isso?

Hoje em dia, praticamente qualquer pessoa pode abrir um blog e ficar online, ganhar seguidores, reconhecimento, e até mesmo *dinheiro*. Sempre que fazemos uma busca no bom e velho **Google**, encontramos uma dúzia de resultados semelhantes. Nós sempre temos aquela dúvida de em qual link entrar, não é mesmo? Quase sempre avaliamos mais o visual, do que o conteúdo em si. Se um site nos é visualmente mais atraente, acaba ganhando mais respeito do que os outros, e isso acaba sendo uma estratégia de SEO. Investir em uma boa aparência é essencial para conquistar leitores. É claro que muitos preferem o conteúdo, do que apenas a aparência, mas quanto mais qualidades tiver, melhor. 

As animações são a parte interativa de uma página, junto aos efeitos de *mouseover*, *mouseout*, *efeito de foco* etc. Os pequenos detalhes chamam a atenção, e por isso é legal investir um pouco de tempo aprendendo isso. Mas também há outra vantagem: as animações em CSS3 são mais fáceis de serem criadas do que as em Javascript. É uma economia de tempo enorme, e estará bem ali, dentro da sua folha de estilos.

### Uma animação básica

Para criar nossa primeira animação, usaremos ```@keyframe exemplo```, onde "exemplo" é o nome que daremos. O código a seguir deve ser incluido na sua folha de estilos (.css)!

    @keyframes examplo {
    from {background-color: black;} // from = de
    to {background-color: white;} // to = para
    }

Neste exemplo básico, eu defini que a animação começaria com o fundo preto, indo para o branco. Repare que não usamos nenhuma configuração para o tempo ou a forma como ela será executada. Agora, para que possamos de fato usá-la, devemos incluir uma div que possa executar a *keyframe*.

    div {width: 100px; height: 100px; background-color: blue; animation-name: examplo; animation-duration: 5s;}
    
Veja um exemplo prático de como ficou:
