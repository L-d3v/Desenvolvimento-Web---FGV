# DESENVOLVIMENTO WEB

- Desenvolvimento Web trata-se do processo de criação de uma página web/site ou aplicativos;

- Ao se tratar de Desenvolvimento Web, estamos nos referindo a um conjunto de tecnologias e linguagens que trabalham em conjunto para criar e tornar as páginas interativas e funcionais;

- Para a criação "perfeita" de uma página web, existe 3 pilares fundamentais, são eles:

  - **HTML(HyperText Markup Language):** Assim como propriamente dito, HTML é uma linguagem de marcação. Ela é responsável por determinar e estruturar o conteúdo a ser apresentado no navegador, quando acessado.

  - **CSS(Cascading Style Sheets):** O CSS pode ser dito como uma linguagem de estilização, ou seja, ela irá definir a aparência visual da página, aplicando cores, espaçamentos, layouts , alterando fontes, entre outros.

  - **JavaScript:** Diferentemente do HTML e CSS que são tecnologias para a criação de uma página web, o JavaScript é uma linguagem de programação e através do seu uso, é possível criar funcionalidades, interatividade e manipular elementos dentro de uma página Web.

# INTRODUÇÃO AO HTML

- HTML é basicamente um arquivo de texto que o navegador irá utilizar renderizar coisas na página, sendo assim, tudo que é apresentado na web se inciar e termina com HTML;

- Para que ocorra renderização de elementos em uma página web, o HTML faz uso de TAGS que são responsáveis por marcar elementos e definir a estrutura da página

- Uma TAG é formada através da abertura e fechamento de colchetes angulares "<tag>", onde em seu meio, estará a TAG q deseja utilizar. Porém, para o fechamento, é utilizado  uma barra no incio "</tag>";

- Existe casos em que algumas TAGS são autofechadas, sendo assim, não possuem a TAG de fechamento ("</tag>")

- Uma TAG também pode conter atributos, que são formas de identifica-las;

## Estruturação Básica:

- Todo documento escrito em HTML segue uma estrutura básica e padrão, sua estrutura é formada por um conjunto de __tags__, são elas:

    ```
  <!DOCTYPE html>
  <html lang="pt-BR">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
    </head>
    <body>
      <!--Conteúdo-->
    </body>
  </html>
  ```



  * `<!DOCTYPE html>`:
    Responsável por determinar que o arquivo em questão, se trata de um documento do HTML5;

  * `<html lang= "pt-BR">`:
    Tag raiz de um arquivo HTML, ela é seguida do atributo "lang", que é responsável por especificar em que idioma o site estará sendo contruido;

* `<head>`:
    Contém os metadados/metainformações sobre o documento, especificando algumas "características" do HTML. Os metadatos padrão são:

  * `<meta charset = "UTF-8"> `:
    Serve para especificar a codificação de caracteres que estará sendo utilizado;

  * `<meta name = "viewport" content = "width, initial-scale = 1.0">`:
    Basicamente, esse metadata irá configurar o _viewport_ do site, tornando-o minimamente responsivo para demais dispositivos;

  * `<title> Document </head>`:
    Apresenta o nome que será escrito na aba do navegador.

* `<body>`:
  Por último, temos a _Tag_ body, que é responsável por apresentar o conteúdo dentro da página Web, dentro dele pode conter _tags_ de titulo (`<h1>`), parágrafos (`<p>`), entre outros tipo de tags.


## Tags Comuns:

  ### Títulos e Parágrafos:

  - As tags de títulos e parágrafos servem para estruturar o texto da página, fornecendo uma maneira de organizar e formatar o conteúdo, tonando mais legível e acessível;

  - Para os títulos, usamos a leta "h", seguida de um número, que é responsável por determinar o nível/grau de importância. Os níveis vai de 1 a 6 e sua estrutura fica da seguinte forma:
    <h1> Título Nível 1</h1>
    <h2> Título Nível 2</h2>
    <h3> Título Nível 3</h3>
    <h4> Título Nível 4</h4>
    <h5> Título Nível 5</h5>
    <h6> Título Nível 6</h6>
