## Overview

Recentemente estive inserido em um projeto para o desenvolvimento de um ambiente em 3D web, de início pareceu um grande desafio, visto que estou familiarizado com o desenvolvimento de páginas "tradicionais" em html/css/js, além ser um desenvolvedor mais focado em backend, porém logo me despertou uma grande curiosidade de entender um pouco mais como desenvolver um ambiente 3D para web e que seja performático e de fácil utilização, este artigo é o primeiro de uma série em que tento sintetizar um pouco dos conhecimentos adquiridos durante minha jornada. Nesta primeira postagem irei contextualizar um pouco do mercado 3D web, além de compartilhar as principais tecnologias para iniciar neste mundo.

## Por que 3D na web ?

Você pode estar se perguntando "Mas por que utilizar 3d na web ? Isso não é coisa de games e aplicativos?". E aqui te trago 2 bons motivos para investir em 3D na web: Marketing e Metaverso ! Vou falar um pouco mais sobre esses dois itens, porém há diversas outras aplicações, como por exemplo o uso em games para a web.

#### Marketing
Não é segredo para ninguém que o marketing é uma parte muito importante de todo negócio, e no mundo corporativo um grande desafio sempre foi como se destacar e atrair os clientes para seu produto, por isso por várias vezes você encontra sites em que utiliza estratégias de 3D como uma forma de engajamento de seus clientes, podemos ver um exemplo como nas páginas de anúncios da Apple, onde seu produto é demonstrado em 3D, ou então em alguns sites de carros onde você consegue navegar pelo carro e até escolher sua cor e seus opcionais e visualizar o resultado em tempo real

Um bom exemplo é o site da [lamborghini](https://www.lamborghini.com/en-en/3d)


#### Metaverso
Apesar de ser um conceito relativamente novo isso não impede de grandes empresas estarem investindo pesado em suas tecnologias, dessa forma a tendência é que aos poucos os sites começam a fornecer um maior suporte para óculos de realidade virtual tornando a experiência do usuário final ainda mais imersiva, como podemos ver o exemplo do [mozilla hubs](https://hubs.mozilla.com/) onde fornece um ambiente web para interações entre participantes, sendo possível realizar meets de forma mais imersiva 


## Tecnologias

Hoje uma das grandes ferramentas utilizadas pela maior parte das empresas é uma biblioteca chamada [ThreeJs](https://threejs.org/) sendo uma implementação em cima do WebGl, o qual basicamente é uma api do HTML5 onde permite a renderização de gráficos 2D e 3D em elemento canvas do HTML

Hoje muitos devs utilizam o React como base para seus desenvolvimentos, pensando nisso foi desenvolvido uma abstração do ThreeJs para o react, esta é a biblioteca [React Three Fiber](https://github.com/pmndrs/react-three-fiber), vale lembrar que esta não é a única biblioteca disponível para o desenvolvimento de 3D utilizando o React, porém é a que identifiquei com uma boa documentação e fácil utilização.


## Elementos básicos

* __Scene:__ No ThreeJs tudo se inicia com uma "scene" ou uma cena onde estará distribuído todos os elementos que estarão disponíveis no ambiente 3D(visíveis ou não).

* __Câmera:__ A câmera é outro elemento básico no ThreeJs, como o próprio nome diz, a câmera será por onde o usuário terá a visão do ambiente 3d, ou seja, delimita dentro do cenário 3d quais serão os elementos exibidos em tela ou não.


* __Renderer:__ O Renderer dentro da nossa página HTML será o ambiente de renderização do 3D, sendo basicamente o elemento canvas na árvore HTML.

