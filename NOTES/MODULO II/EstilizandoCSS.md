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


- **Propiredades de textos:***

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

- **Propriedades dde cores:**
    
    - **color:** 
        Define a cor do texto;
  
    - **background-color:**
        Define a cor de fundo do site;

    - **boder-color:**
        Define a cor da borda;