# CSS-colors
Registro dos conhecimentos adquiridos no curso FreeCodeCamp


### CSS

#### CONJUNTO DE MARCADORES COLORIDOS

---

**Meta Elementos**

- Você pode ter vários elementos meta em uma página da web. Cada elemento meta adiciona informações sobre a página que não podem ser expressas por outros elementos HTML.
  - Adicione outro elemento meta dentro do elemento head. Dê a ele o atributo name definido como "viewport" e o atributo content definido como "width=device-width, initial-scale=1.0" para que a página tenha a mesma aparência em todos os dispositivos.

---

**Centralizar Marcador**

- Seu marcador ficaria melhor se estivesse centralizado na página. Uma maneira fácil de fazer isso é com a propriedade abreviada margin.
  - No último projeto, você definiu a área de margem dos elementos separadamente com propriedades como margin-top e margin-left. A propriedade abreviada margin facilita a definição de várias áreas de margem ao mesmo tempo.
  - Para centralizar seu marcador na página, defina a sua propriedade margin como auto. Isso define margin-top, margin-right, margin-bottom e margin-left como auto.

---

**Adicionar Marcadores**

- Agora que você tem um marcador centralizado com cor, é hora de adicionar os outros marcadores.
  - No container div, adicione mais dois elementos div e dê a cada um deles uma classe de marcador.
  - Embora você tenha três elementos div de marcador separados, eles parecem um grande retângulo. Você deve adicionar algum espaço entre eles para facilitar a visualização de cada elemento.
  - Quando a propriedade abreviada margin tem dois valores, ela define margin-top e margin-bottom com o primeiro valor, e margin-left e margin-right com o segundo valor.

---

**Cores Diferentes para Marcadores**

- Para dar aos marcadores cores diferentes, você precisará adicionar uma classe única a cada um deles.
  - Várias classes podem ser adicionadas a um elemento listando-as no atributo class e separando-as com um espaço. Por exemplo, o seguinte adiciona as classes animal e dog a um elemento div.
  - Se você adicionar várias classes a um elemento HTML, os estilos das primeiras classes que você listar podem ser substituídos pelos das classes futuras.

---

**Regras CSS para Cores**

- Crie uma nova regra CSS que direciona a classe one e defina sua propriedade background-color para red.
  - Crie uma regra CSS que direciona a classe two e defina sua propriedade background-color para green.
  - Além disso, crie uma regra CSS separada para a classe three e defina sua propriedade background-color para blue.

---

**Modelos de Cor**

- Existem dois modelos de cores principais: o modelo aditivo RGB (vermelho, verde, azul) usado em dispositivos eletrônicos, e o modelo subtrativo CMYK (ciano, magenta, amarelo, preto) usado em impressão.
  - Neste projeto, você trabalhará com o modelo RGB. Isso significa que as cores começam como preto e mudam à medida que diferentes níveis de vermelho, verde e azul são introduzidos. Uma maneira fácil de ver isso é com a função CSS rgb.
  - Uma função é um pedaço de código que pode receber uma entrada e realizar uma ação específica. A função CSS rgb aceita valores, ou argumentos, para vermelho, verde e azul, e produz uma cor:
    - Cada valor de vermelho, verde e azul é um número de 0 a 255. 0 significa que há 0% dessa cor e é preto. 255 significa que há 100% dessa cor.
  - Na regra CSS .one, substitua a palavra-chave da cor red pela função rgb. Para a função rgb, defina o valor para red como 255, o valor para green como 0 e o valor para blue como 0.
  - Agora use a função rgb para definir as outras cores.
  - Na regra CSS .two, use a função rgb para definir a cor de fundo para o valor máximo para green, e 0 para os outros valores. E na regra CSS .three, use a função rgb para definir a cor de fundo para o valor máximo para blue, e 0 para os outros valores.

---

**Espaço Vertical Adicional**

- Embora os marcadores vermelho e azul pareçam iguais, o verde é muito mais claro do que era antes. Isso ocorre porque a palavra-chave da cor verde é na verdade um tom mais escuro, e está aproximadamente a meio caminho entre o preto e o valor máximo para verde.
  - Agora adicione um pouco mais de espaço vertical entre seus marcadores e a borda do elemento container em que eles estão.
  - Na regra CSS .container, use a propriedade abreviada padding para adicionar 10px de padding superior e inferior, e defina o padding esquerdo e direito para 0. Isso funciona de maneira semelhante à propriedade abreviada margin que você usou anteriormente.

---

**Cores Primárias no Modelo RGB**

- No modelo de cores aditivas RGB, as cores primárias são cores que, quando combinadas, criam branco puro. Mas para que isso aconteça, cada cor precisa estar em sua intensidade máxima.
  - Observe que as cores vermelha e ciano são muito brilhantes quando estão próximas uma da outra. Esse contraste pode ser distraente se for usado em excesso em um site, e pode tornar o texto difícil de ler se estiver colocado em um fundo com uma cor complementar.
  - É uma prática melhor escolher uma cor como a cor dominante e usar sua cor complementar como destaque para chamar a atenção para certos conteúdos na página.

**Exemplos:**
- `rgb(red, green, blue)`
- `rgb(255, 0, 0) → Vermelho puro`
- `rgb(0, 255, 0) → Verde puro`
- `rgb(0, 0, 255) → Azul puro`
- `rgb(255, 255, 255) → Branco`
- `rgb(0, 0, 0) → Preto`

---

**Detalhes Adicionais para Marcadores**

- Agora é hora de adicionar outros detalhes aos marcadores, começando pelo primeiro.
  - No primeiro elemento do marcador div, altere a classe one para red.

```html
<div class="marker one">
</div>
```

Para:

```html
<div class="marker red">
</div>
```

- Atualize a regra CSS .one para direcionar a nova classe red.
  - Uma maneira muito comum de aplicar cor a um elemento com CSS é com valores hexadecimais ou hex. Embora os valores hexadecimais pareçam complicados, eles são realmente apenas outra forma de valores RGB.
  - Os valores de cor hexadecimais começam com um caractere # e aceitam seis caracteres de 0-9 e A-F. O primeiro par de caracteres representa o vermelho, o segundo par representa o verde e o terceiro par representa o azul. Por exemplo, #4B5320.
  - Você pode já estar familiarizado com valores decimais, ou valores de base 10, que vão de 0 a 9. Valores hexadecimais, ou valores de base 16, vão de 0 a 9, depois A a F:
  - Com cores hexadecimais, 00 é 0% dessa cor e FF é 100%. Então, #00FF00 traduz 0% vermelho, 100% verde e 0% azul, sendo igual a rgb(0, 255, 0).

---

**Modelo de Cores HSL**

- O modelo de cores HSL, ou matiz, saturação e luminosidade, é outra forma de representar cores.
  - A função CSS hsl aceita 3 valores: um número de 0 a 360 para o matiz, uma porcentagem de 0 a 100 para a saturação e uma porcentagem de 0 a 100 para a luz.
  - Se você imaginar um círculo cromático, a cor vermelha fica a 0 graus, o verde é a 120 graus e o azul está a 240 graus.
  - A saturação é a intensidade de uma cor de 0%, ou cinza, até 100% para cor pura. Você deve adicionar o sinal % de percentual aos valores de saturação e luz.
  - A luz é o nível de brilho no qual uma cor aparece, de 0%, ou preto completo, até 100%, branco total, com 50% de neutralidade.

Ex: `hsl(hue, saturation, lightness)`

---

**Gradiente de Cor**

- Você aprendeu algumas maneiras de definir cores planas em CSS, mas também pode usar uma transição de cor, ou gradiente, em um elemento.
  - Um gradiente é quando uma cor transita para outra. A função CSS linear-gradient permite controlar a direção da transição ao longo de uma linha e quais cores são usadas.
  - Uma coisa a lembrar é que a função linear-gradient na verdade cria um elemento de imagem, e geralmente é emparelhada com a propriedade background que pode aceitar uma imagem como valor.
 
---
### CSS

#### CONJUNTO DE MARCADORES COLORIDOS

---

**Função Linear-Gradient**

- A função linear-gradient é muito flexível -- aqui está a sintaxe básica que você usará neste tutorial:

```css
linear-gradient(gradientDirection, color1, color2, ...);
```

---

**Função RGB no Gradiente**

- Você usará a função rgb para as cores deste gradiente.
  - Na mesma função linear-gradient, use a função rgb para definir o segundo argumento de cores como vermelho puro.
  - Você não verá o gradiente ainda porque a função linear-gradient precisa de pelo menos dois argumentos de cor para funcionar.
  - Na mesma função linear-gradient, use a função rgb para definir o segundo argumento de cores como verde puro.
  - Como você pode ver, a função linear-gradient produziu um gradiente suave de vermelho para verde. Embora a função linear-gradient precise de um mínimo de dois argumentos de cor para funcionar, ela pode aceitar muitos argumentos de cor.

---

**Paradas de Cor (Color-Stops)**

- As paradas de cor permitem ajustar onde as cores são colocadas ao longo da linha de gradiente. Elas são uma unidade de comprimento como px ou porcentagens que seguem uma cor na função linear-gradient.
  - Por exemplo, neste gradiente vermelho preto, a transição do vermelho para o preto ocorre no ponto 90% ao longo da linha de gradiente. Então, o vermelho ocupa a maior parte do espaço disponível:

```css
linear-gradient(90deg, red 90%, black);
```

---

**Gradiente para o Marcador Verde**

- O marcador vermelho está parecendo muito mais realista. Agora você fará o mesmo para o marcador verde, usando uma combinação da função linear-gradient e cores hexadecimais.
  - Na regra do CSS .green, altere a propriedade background-color para background.

---

**Direção do Gradiente Padrão**

- Se nenhum argumento gradientDirection for fornecido à função linear-gradient, ela organiza as cores de cima para baixo, ou ao longo de uma linha de 180 graus, por padrão.

---

**Gradiente para o Marcador Azul**

- Agora você aplicará um gradiente ao marcador azul, desta vez usando a função hsl como argumentos de cor.
  - Na regra CSS .blue, altere a propriedade background-color para background.

---

**Propriedade Opacity**

- Com a propriedade do CSS opacity, você pode controlar como um elemento é opaco ou transparente. Com o valor 0, ou 0%, o elemento será completamente transparente e 1.0, ou 100%, o elemento será completamente opaco, como é por padrão.

---

**Canal Alfa**

- Outra maneira de definir a opacidade de um elemento é com o canal alfa. Semelhante à propriedade opacity, o canal alfa controla quão transparente ou opaca uma cor é.
  - Você já está familiarizado com o uso da função rgb para definir cores. Para adicionar um canal alfa a uma cor rgb, use a função rgba em vez disso.
  - A função rgba age como a função rgb, mas recebe mais um número de 0 a 1.0 para o canal alfa:

---

**Problema com Display Block**

- Parece que sua manga desapareceu, mas não se preocupe -- ela ainda está lá. O que aconteceu é que seu novo div cap está ocupando toda a largura do marcador, e está empurrando a manga para a linha seguinte.
  - Isso ocorre porque a propriedade padrão display para elementos div é o block. Então, quando dois elementos block estão próximos um do outro, eles empilham como blocos de verdade. Por exemplo, os elementos do marcador estão todos empilhados em cima um do outro.
  - Para posicionar dois elementos div na mesma linha, defina suas propriedades display para inline-block.

---

**Bordas em Elementos HTML**

- Todos os elementos HTML têm bordas, embora geralmente estejam definidas como none por padrão. Com o CSS, você pode controlar todos os aspectos da borda de um elemento e definir a borda de todos os lados, ou apenas um lado de cada vez. Para uma borda estar visível, você precisa definir sua largura e estilo.
  - As bordas têm vários estilos para escolher. Você pode fazer sua borda uma linha sólida, mas também pode usar uma linha tracejada ou pontilhada, se preferir. Linhas de borda sólida são provavelmente as mais comuns.
  - Sua borda deve estar visível agora. Se nenhuma cor for definida, preto é usado por padrão. Porém, para tornar seu código mais legível, é melhor definir a cor da borda explicitamente.
  - A propriedade abreviada border-left permite definir a largura, o estilo e a cor da borda esquerda ao mesmo tempo.
  - Na regra do CSS .sleeve, substitua as propriedades border-left-width, border-left-style, e border-left-color pela propriedade abreviada border-left. Os valores para a largura, estilo e cor da borda esquerda devem ser os mesmos.

---

**Propriedade Box-Shadow**

- A propriedade box-shadow aplica uma ou mais sombras a um elemento. Aqui está a sintaxe básica:

```css
box-shadow: offsetX offsetY color;
```

  - Veja como os valores de offsetX e offsetY funcionam:
    - Ambos offsetX e offsetY aceitam valores numéricos em px e outras unidades CSS.
    - Um valor positivo de offsetX move a sombra para a direita e um valor negativo a move para a esquerda.
    - Um valor positivo de offsetY move a sombra para baixo e um valor negativo a move para cima.
    - Se você quiser um valor de zero (0) para offsetX, offsetY ou para os dois, você não precisa adicionar uma unidade. Todos os navegadores entendem que zero significa que não há alterações.

---

**Sombra Simples**

- Como você pode ver, você adicionou uma sombra vermelha simples ao redor do seu marcador que está 5 pixels à direita e 5 pixels para baixo.
  - Mas e se você quisesse posicionar essa sombra no lado oposto? Você pode fazer isso usando valores negativos para offsetX e offsetY.

---

**Arestas da Sombra**

- Note que as bordas da sombra são nítidas. Isso ocorre porque há um valor opcional blurRadius para a propriedade box-shadow:
  - Se um valor para blurRadius não estiver incluído, o padrão é 0 e produz arestas com pontas. Quanto maior o valor de blurRadius, maior será o efeito de desfoque.

---

**Valor SpreadRadius**

- E se você quiser expandir ainda mais a sombra? Você pode fazer isso com o valor opcional spreadRadius:

---
