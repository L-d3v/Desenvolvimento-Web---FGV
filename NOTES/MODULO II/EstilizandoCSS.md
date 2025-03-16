# Revisão:

Como dito no módulo anterior, o HTML é responsável por fornecer a estrutura de uma página web, enquanto o CSS é responsável por fornecer o estilo/aparência da página. Com o uso do CSS, podemos transformar uma estrutura simples numa “interface” atraente e responsiva.

## Introdução ao CSS:

- Cascadin Style Sheets (CSS) permite adicionarmos cores, fontes, espaçamentos entre outras demais formatações em elementos criados pelo HTML;


- Existem 3 formas de aplicar estilização em elementos aplicados no HTML, são eles:

  1. **Estilo Embutido:** 
     Caso onde a estilização é adicionada diretamente ao elemento desejado no HTML, através do uso do atributo `style:`;
        ``` 
        <h1 style="color: blue; font-size: 24px;">Este é um cabeçalho h1</h1>
        ```
 
  2. **Estilo Interno:**
     Semelhante ao primeiro caso, porém o estilo interno é aplicado na seção `<head>` do HTML, criando a tag `<style>`
      ```
         <!DOCTYPE html>
         <html>
         <head>
            <title>Minha Página</title>
               
         <style>
             h1 {
                 color: blue;
                 font-size: 24px;
             }
         </style>
         </head>
    
         <body>
             <h1>Este é um cabeçalho h1</h1>
             <p>Este é um parágrafo de texto.</p>
         </body>
         </html>
        ```

  3. **Estilo Externo (Padrão de uso):**
      Nesse caso, o documento CSS é criado separadamente e depois é vinculado ao documento HTML através da tag `<link>` na seção `<head>`
     ```
     <!DOCTYPE html>
      <html>
      <head>
      <title>Minha Página</title>
  
      <link rel="stylesheet" href="styles.css">
        
      </head>

      <body>
         <h1>Este é um cabeçalho h1</h1>
         <p>Este é um parágrafo de texto.</p>
      </body>
      </html>
       ```


- Para aplicarmos as estilizações desejadas, devemos seguir sintaxe do CSS, onde dentro do CSS, cada regra de estilo é formada por um seletor e seu bloco de declaração;


- Um seletor é responsável por apontar/determinar o elemento no HTML que será estilizado, o bloco de declaração é onde irá conter as estilizações a serem aplicadas separas por ponto e virgula (";");
    Ex. 
    ```
    h1{
        color: blue;
        font-size: 24px;
    }
    ```
  
    Nesse contexto, podemos notar o seguinte:
  
    - `h1` é o seletor que irá aplicar as alterações para todos os elementos `<h1>` em HTML;
    - Os colchetes `{ }` são responsáveis por determinar o bloco de declaração
    - `color:blue;` e `font-size: 24px;` são duas declarações de estilo que define a cor do texto e o tamanho da fonte;

## Tamanhos em CSS:

- Dentro do CSS, os tamanhos podem ser definidos em seis tipos, sendo:
    1. **Pixels(px)**
    2. **Polegadas(in)**
    3. **Centimentros(cm)**
    4. **Rem**
    5. **Viewport(vw ou vh**

- As unidades como `rem`, `vw` e `vh` são unidades de valores relativos, sendo recomnedavél para criar layouts que se adaptaram para diferentes tamanhos de telas;

## Seletores, ID's e Classes:

- Assim como dito no inicio desse documento, os seletores são responsáveis por aplicar os estilos aos elementos no HTML. Porém, podemos usar 3 tipos de seletores:

    1. **Seletor de Elemento:**
        O seletor de elemento aplica os estilos aos elementos selecionados, ou seja, quando um `h1` é chamado no CSS, o estilo que for aplicado será aplicado aos demais `h1` existentes na página;
        ```
        h1{
            color:blue;
        }
        ```

    2. **Classes:**
       Para criar uma classe, é necessaŕio aplicar um atributo `class` ao elemento HTML. Quando chamado no CSS, deve-se inicar com o uso de um ponto (".") e o estilo aplicado será apenas para aquele(s) elemento(s) que possuir a mesma classe;
       ```
       .titulo{
           font-family: "Arial"
       }
       ```
       
    3. **ID:**
         Para os IDS, utiliza-se a mesma idéia das classes, porém agora o atibuto será um `id`. Ao chamar o ID no CSS, deve-se iniciar com uma hashtag ("#").
        ```
       #titulo-principal{
            font-weight: bold;
       }
        ```

- Vale ressaltar que os seletores do tipo `class` são reutilizavéis, podendo ser aplicado a mais de um elemento. Já o seletor do tipo `id`, ele é do tipo reservado e único, então só pode ser usado 1 unica vez;

## Propriedades de Texto e Layout Básico:

- Para melhorar a legibilidade e aparência de um site é possivel realizar adicionando alguns estilos de textos e layout;


- Dentro do CSS, podemos usar sua ampla variedade de propriedades e estilizar textos da forma que desejarmos;


- **Propriedades de textos:***

    - **font-size:**
        Define o tamanho da fonte;
  
    - **font-family:**
        Define a fonte do texto;
  
    - **font-weight:**
        Define o peso da fonte;
  
    - **text-align:**
        Alinha o texto;
  
    - **line-height:**
        Controla a altura entre as linhas do texto

- **Propriedades de cores:**
    
    - **color:** 
        Define a cor do texto;
  
    - **background-color:**
        Define a cor de fundo do site;

    - **boder-color:**
        Define a cor da borda;

### Margens, Bordas, Padding, Dimensões:

- Com o uso de algumas propriedades dentro do CSS, conseguimos controlar o espaço ao redor dos elementos;


- Essas propriedades podem ser ditas como a base do modelo de caixa(_box model_);

    - **Margin:** 
        Define um espaço fora do elemento;
  
    - **Border:** 
        Aplica um contorno em volta do elemento;
  
    - **Padding:**
        Define um espaço dentro do elemento, entre o conteúdo e a borda;

- Para as dimensões, podemos controlo-las usando as propriedades de `width`(largura) e `height`(altura);

## Flexbox:

- Para facilitar a sistribuição de espaços e no alinhamentos dos itens numa interface, podemos fazer o uso do _Flexbox_. Com ele, podemos criar layouts responsivos, alinhar itens em linha ou coluna, dentre outras opções que ele permite realizar;


- **Propriedades para Container Flexível:**
  
  - `display:flex;`: 
    Permite controlar a direção, o alinhamento e espaçamentos entre os elementos filhos;

  - `flex-direction`: 
        Define a direção dos itens dentro do container, o valores presentes são:
        
    - `row`(padrão): 
        OS itens são colocados em linha;
    
    - `row-reverse`: 
        Os itens são colocados em linha, mas do lado contrário/inversa;
  
    - `column`: 
        Os itens são colocados em forma de coluna (um abaixo do outro);
         
    - `column-reverse`: 
        Assim como o `column`, porém na ordem inversa;

- **Alinhamento dos Itens:**

  - Com o uso do `justify-content`, é possivel alinhar os itens de acordo com o eixo principal;

  - Assim como o `flex-direction`, o justify-content também possui valores a ser adicionados. São eles:
    
    - `flex-start`: 
      Define o alinhamento para "início";

    - `flex-end`:
      Define o alinhamento para o "final";

    - `center`:
      Define o alinhamento ao centro
    
    - `space-between`:
      Define o alinhamneto uniformemente entre os elementos dentro do container;
    
    - `space-around`:
      Define o alinhamento uniformemente ao redor dos elementos dentro do container;

- **Alinhamneto no Eixo Cruzado:**

- Usando a propriedade `align-items`, os elementos serão alinhados em relação ao eixo cruzado. Em caso de estar com a propriedade do flex-direction `row`, será alinhado na vertical;

- Valores que podem ser adicionados:

    - `stretch`:
      Os itens serão esticados para preencher o contâiner;
  
    - `flex-start`:
      Os itens são alinhados no ínicio do contâiner;
  
    - `flex-end`:
      Os itens são alinhados ao final do contâiner;
  
    - `center`:
      Os itens serão alinhados ao centro;
  
    - `baseline`:
      Os itens serão alinhados na linha da base

- **Ordem dos Itens:**

- Além de propriedades destinadas ao contâiner, o `display flex` também oferece propriedades destinadas aos itens;

    - `order`:
      Define a ordem dos itens dentro do contâiner. Seu valor inical é 0, mas pode ser alterado por vlaores positivos ou negativos;
  
    - `flex-grow`:
      Define a capacidade de crescimento do item para preencher o espaço vasio presente no contâiner. Inicialmente o valor é 0, desse forma o item não crescerá além do tamanho definido;
  
    - `flex-shrink`:
      Ao contrário do `flex-grow`, a propriedade flex-shrink define a capacidade de encolhimento do item, quando seu espaço é limitado. Inicialmente seu valor é 1, dessa forma o item pode encolher;
  
    - `flex-basis`:
      Define o tamanho inicial do item antes dele crescer ou encolher;

## CSS Grid: 

- Assim como o Flexbox, o CSS Grid é um sistema de layout, permitindo criar layouts com facilidade. Diferentemente do flexbox, o CSS Grid atua em formas de colunas e linhas, posicionando os itens de forma precisa;

- O CSS Grid trabalha com o `display: grid`, sendo preciso especificar as linhas e colunas através das propriedades `grid-template-rows` e `grid-template-columns`, onde:
  
    - `grid-template-columns`:
      Define o número e tamanho das colunas;
  
    - `grid-template-rows`:
      Define o número e tamanho das linhas;
  
    - `gap`:
      Define o espaçamento entre as célular da propriedade grid;

- **Posicionamento Elementos Grid:**

    - Com as propriedades de `grid-column` e `grid-row`, podemos posicionar os elementos dentro do Grid;

        - `grid-column`:
          Define quais colunas serão ocupadas pelo elemento grid.
            
            Ex.
            ```
            grid-column: 1 -> Ocupará a coluna 1
            grid-column: 4 -> O item terminará na linha 4
            grid-column: 1/3 -> O item ocupará as colunas 1 e 2, onde 3 será o começo da terceira coluna
            ```

        - `grid-row`:
          Define quais linhas serão ocupadas pelo elemento grid.
        
            Ex.
            ```
            grid-row: 1 -> Ocupará a linha 1
            grid-row: 4 -> Ocupará a linha 4
            grid-row 1/3 -> Ocupará até a segunda linha, onde 3 será o inicio da terceira linha
            ```

## Técnicas de Posicionamento e Layout Responsivo:

- Criar um site com um layout responsivo e que se adapte aos tamanhos de telas diversificados é ideal para tornar a experiência mais agradavél;

- O posicionamento preciso dos elementos podem ser feitos através de técnicas como `position`, `z-index`, `float` e `clear`, onde:
    

- **Position:** 

  - Com a propriedade `position`, podemos definir a forma em que o elemento será posicionnado na página. Essa propriedade oferece os seguintes valores:
      
      - `static`: 
        Os elementos serão posicionados conforme o fluxo da página;
    
      - `relative`:
        Os elementos são posicionados em relação a sua posição original;
    
      - `absolute`:
        Os elementos será relativo ao container, dessa forma, posicionando mais próximo;
    
      - `fixed`:
        O elemnto é posicionado em releação ao bloco de contenção, ou seja, em relação ao viewport;
    
      - `stick`:
        O elemento é posicionado com base na posição de rolagem do usuário;

- **Z-index:**

    - A propriedade `z-index`, conseguimos controlar a sobreposição dos elementos, onde um elemento com a propriedade maiorUso do Z-Index que a de outro elemento, será apresentado "acima".
  
        Ex.
        ```
      .box1 {
        position: absolute;
        z-index: 1;
        }

      .box2 {
        position: absolute;
          z-index: 2;
        }
        ```

- **Unidades Relativas:**

- Viewport é a área visivel de uma página web e uma unidade relativa;


- Com as unidades relativas, podemos criar uma página que se adapta dinamicamente ao tamanho da tela;


- Algumas unidades relativas são:
    
    - **Porcentagem(%):** 
      Se baseia ao tamanho do elemento pai;
  
    - **Viewport Width(vw):**
      1 vw é igual será igual a 1% da largura da viewport;
  
    - **Viewport Height(vh):**
      Assim como o `vw`, 1vh será igual a 1% da altura do viewport;

## Adaptação para Diferentes Telas:

- Media Queries é uma técnica de desing responsivo, quando usado, é possivel fazer com que o site funcione em diferentes dispositivos com diferentes tamanhos;

- Com o uso da Media Querie, podemos aplicar determinados estilos em diferentes dispositivos;