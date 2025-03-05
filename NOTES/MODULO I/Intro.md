# DESENVOLVIMENTO WEB

- Desenvolvimento Web trata-se do processo de criação de uma página web/site ou aplicativos;


- Ao se tratar de Desenvolvimento Web, estamos nos referindo a um conjunto de tecnologias e linguagens que trabalham em conjunto para criar e tornar as páginas interativas e funcionais;


- Para a criação "perfeita" de uma página web, existe 3 pilares fundamentais, são eles:


  - **HTML(HyperText Markup Language):** Assim como propriamente dito, HTML é uma linguagem de marcação. Ela é responsável por determinar e estruturar o conteúdo a ser apresentado no navegador, quando acessado.


  - **CSS(Cascading Style Sheets):** O CSS pode ser dito como uma linguagem de estilização, ou seja, ela irá definir a aparência visual da página, aplicando cor, espaçamentos, layouts, alterando fontes, entre outros.


  - **JavaScript:** Diferentemente do HTML e CSS são tecnologias para a criação de uma página web, o JavaScript é uma linguagem de programação e através do seu uso, é possível criar funcionalidades, interatividade e manipular elementos numa página Web.

# INTRODUÇÃO AO HTML

- HTML é basicamente um arquivo de texto que o navegador irá utilizar renderizar coisas na página, sendo assim, tudo apresentado na web se inicia e termina com HTML;


- Para ocorrer a renderização de elementos em uma página web, o HTML faz uso de TAGS responsáveis por marcar elementos e definir a estrutura da página


- Uma TAG é formada através da abertura e fechamento de colchetes angulares "<tag>", onde em seu meio, estará a TAG que deseja utilizar. Porém, para o fechamento, é utilizado uma barra no início "</tag>";


- Existem casos em que algumas TAGS são autofechadas, sendo assim, não possuem a TAG de fechamento ("</tag>")


- Uma TAG também pode conter atributos, que são formas de identificá-las;

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
    Tag raiz de um arquivo HTML, ela é seguida do atributo "lang", responsável por especificar em que idioma o site estará sendo construído;


* `<head>`:
    Contém os metadados/metainformações sobre o documento, especificando algumas "características" do HTML. Os metadata padrão são:

  * `<meta charset = "UTF-8"> `:
    Serve para especificar a codificação de caracteres que estará sendo utilizado;

  * `<meta name = "viewport" content = "width, initial-scale = 1.0">`:
    Basicamente, esse metadata irá configurar o _viewport_ do site, tornando-o minimamente responsivo para demais dispositivos;

  * `<title> Document </head>`:
    Apresenta o nome que será escrito na aba do navegador.


* `<body>`:
  Por último, temos a _Tag_ body, responsável por apresentar o conteúdo dentro da página Web, dentro dele pode conter _tags_ de título (`<h1>`), parágrafos (`<p>`), entre outros tipo de tags.


## Tags Comuns:

  ### Títulos e Parágrafos:

  - As tags de títulos e parágrafos servem para estruturar o texto da página, fornecendo uma maneira de organizar e formatar o conteúdo, tonando mais legível e acessível;


  - Para os títulos, usamos a leta "h", seguida de um número, responsável por determinar o nível/grau de importância. Os níveis vão de 1 a 6 e sua estrutura fica da seguinte forma:

    `<h1> Essa é a estrutura de uma Tag de Título</h1>`
        <h1> Título Nível 1</h1>
        <h2> Título Nível 2</h2>
        <h3> Título Nível 3</h3>
        <h4> Título Nível 4</h4>
        <h5> Título Nível 5</h5>
        <h6> Título Nível 6</h6>

  - Para os parágrafos, utilizamos a _tag_ `<p>`

  ### Listas:

-   As listas são uteis para agrupar itens semelhantes/relacionados;


- Além disso, as listas podem ser divididas em 2 tipos: Ordenadas e Não Ordenadas;

  - Para as listas ordenadas, utiliza-se a _tag_ `<ol>`, que significa Ordered list;

  - Para as listas não ordenadas, utilizamos a _tag_ `<ul>`, que significa Unordered list;


- Para adicionarmos mais itens em uma lista, fazemos o uso da _tag_ `<li>` (list item);

```
<ol>
  <li>Primeiro item</li>
  <li>Segundo item</li>
  <li>Terceiro item</li>
</ol>

<------------H------------>

<ul>
  <li>Item A</li>
  <li>Item B</li>
  <li>Item C</li>
</ul>
```

### Atributos:

- Os atributos servem como característica de uma _tag_, onde, para sua formação, é necessário o nome e o seu valor dentro da _tag_ de abertura;

```
<a href="https://www.example.com" target="_blank">Visite o Example</a>
<img src="imagem.jpg" alt="Descrição da imagem">
```

- No caso acima, é possível identificar os seguintes atributos:


1. **href:**
    Define o link de destino para o elemento `<a>`;


2. **target:**
   Define em como o link será aberto, sendo possível aplicar 4 valores:
    - **"_blank":** Abre o documento em uma nova aba;
    - **"_self":** Abre o documento no mesmo frame;
    - **"_parent":** Abre o documento no frame do elemento pai;
    - **"_top":** Abre o documento no corpo inteiro da janela. 
   

3. **src:** Define o caminho do arquivo a ser exibido na tela;


4. **alt:** Aplicada por questões de Acessibilidade, o atributo "alt" serve para adicionar uma descrição alternativa;

### Imagens:

- Dentro do HTML é possível incorporar não só imagens, mas também, áudios e vídeos, porém são "menos" utilizadas;


- Para aplicar uma imagem em uma Página Web, utilizamos a _tag_ `<img>` sem alguma "restrição" do formato da imagem. Os mais comuns são:
  
    1. **JPEG:** Normalmente para fotografias, onde a imagem possui muitas cores;
    
    2. **PNG:** Suporta transparência (fundo transparente);

    3. **GIF:** Curta animação com limitação de 256 cores;

    4. **SVG:** Ideal para ícones e logotipos, pois não retira a qualidade;

    5. **WEBp:** Formato destinado ao desenvolvimento Web, onde busca reduzir o tamanho dos arquivos para um melhor carregamento.


- O caminho de uma imagem pode ser Relativo ou Absoluto, onde:

    - Caminho Relativo especifica a localização da imagem em relação ao documento;
  
    - Caminho Absoluto especifica a localização completa da imagem (pode incluir o domínio).

### Links e Ancoras:

- Para a criação de um link, é utilizado a _tag_ `<a>`, onde o tipo desse link pode ser divido em dois:

    - **Links Internos:** Apontam para outro arquivo dentro do mesmo documento/site;
    - **Links Externos:** Apontam para outros Sites Web.
  

- O caso das âncoras serve para criar uma conexão de uma seção presente na mesma página (Ex. Uma Landing-page);


- Para criar essa conexão, definimos/aplicamos um `id` que servirá como identificador da seção. 

    ```
    <h2> id = "secao1"> Seção 1 <h2>
    <a href = "#secao1"> Voltar para a Seção 1 </a> 
    ```

### Tabelas e Formulários: 

- Tabelas e formulários são essenciais para realizar a coleta de dados/informações dos usuários;


- O caso das tabelas, são normalmente utilizadas como meio de organização;


- Para criarmos uma tabela usamos _tags_ como `<tr>` que indicará a linha, `<th>` que indica uma cédula e por último `th` que indico o cabeçalho da tabela;


- Outras tags presentes são:   
    
    * `<table>`: Define uma tabela;
    * `<thead>`: Define o cabeçalho;
    * `<tbody>`: Define o corpo da tabela;

    Ex.
        
    ```
    <table>
        <thead>
            <tr>
                <th>Nome</th>
                <th>Idade</th>
                <th>Cidade</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Ana</td>
                <td>28</td>
                <td>São Paulo</td>
            </tr>
            <tr>
                <td>João</td>
                <td>35</td>
                <td>Rio de Janeiro</td>
            </tr>
        </tbody>
    </table>
    ```

- Em uma tabela, é possível mesclar cédulas utilizando atributos como `rowspan` ou `colspan`;


- A `rowspan` mescla a célula com a célula de baixo, enquanto `colspan` mescla a célula com duas células à direita;


- Agora, os formulários permitem a coleta de dados. Para a sua construção, utilizamos a _tag_ `<form>`;


- Um formulário pode conter diversos elementos, tais como: campo de entrada, caixa de seleção, botões, entre outros;


- A estrutura básica de um formulário é feito da seguinte forma:

    ```
    <form action="/submit" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">

    <label for="email">Email:</label>
    <input type="email" id="email" name="email">

    <input type="submit" value="Enviar">
    </form>
    ```
- Onde: 
    * **action:** Trata-se de um atributo que definirá a URL para onde os dados serão enviados;

    * **method:** Define o método de envio dos dados (_get_ ou _post_);
 
    * **label:** Define um rótulo para um elemento do formulário;
  
    * **input:** Define um campo de entrada;


- Os campos de entrada de um `input` mais comuns são:
    * **Texto:** Aplicando o atributo `type = "text"`;
  
    * **E-mail:** Aplicando o atributo `type="email"`;
  
    * **Número:** Aplicando o atributo `type="number"`;
  
    * **Senha:** Aplicando o atributo `type="password"`;
  
    * **Data:** Aplicando o atributo `type="date"`;
  
    * **Caixa de Seleção:** Aplicando o atributo `type="checkbox"`;
  
    * **Botão de Rádio:** Aplicando o atributo   `type="radio"`;
  
    * **Botão de Envio:** Aplicando o atributo `type="submit"`.

- É possível adicionar meios de validação para melhorar a experiência do usuário, são eles:
    * **required:** Indica que o campo é obrigatório para ser preenchido;

    * **min** e **max:** Define um valor mínimo/máximo para um campo numérico;

    * **pattern:** Define um padrão de expressão regular onde o valor/resposta deve corresponder;