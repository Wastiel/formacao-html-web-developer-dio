# HTML II: Ampliando Conhecimento

## On boarding

- Vamos aprender pontos mais avançados do HTML
    - HTML Semãntico
    - Melhorias nas versões do HTML
    - Acessibilidade
    - WebScraping
    - Tags
        - main, header, footer
        - nav, section, aside
        - article, blockqoute, q
        - figure, figcaption, picture
    - Resenha: o que é SEO?

A ideia deste módulo é criar um site do jeito que tem que ser. 

### HTML Semântica

O que é semântica? Disciplina da linguística que se ocupa da significação das palvras e expressões linguísticas bem como das relações de sentido que estas estabelecem entre si. 

Significa dentro do HTMl, se o mesmo está fazendo o que se propos a fazer.    

Antigamente utilizavamos DIVs, no html 5,veio algumas tag's que trouxeram mais siginficiados para algumas coisas. 

A classe da uma acessbilidade que as vezes não é interessante termos, pois tira o padrão e organização relacionado ao HTM.

O HTML não é somente lido por humanos, também é lido por humanos. 

Organizar por tag,s, auxilia os robos a ler o html e essa organização se chama webscraping., existem leitores de telas.

Mudanças no html, vem para mudar a estrutura e organizar a semantica. 

HTML 5 são mudanças de conceitos e fundamentos. O HTML deixou de ter o objetivo de formatação e sim de organização. 

### Mudança do HTML 5

- Mudanças do html 4 para o HTML 5.
    - Novas tags
    - Novos Atributos
    - alguns atributos obsoletos
    - HTML deixando de ser um padrão de formatação
        - Deixando tudo para o CSS
        - Parceria entre CSS e htmL aumentando mais
    - Novas Tag's criadas:
        - main, header, footer, nav, section, aside, article, video
    - Tag's depreciadas:
        - basefront, big, center, font, strike, tt, frame, frameset

[Exemplo de site simples para exemplificação](./index.html)

Tag's em vermelho significam que estão ficando depreciadas. 

Principais mudanças não formatação é estrutura. 

### Acessibilidade

- Navegabilidade definida principlamente pelo html
- Foco em uma web mais democrática
- Aula mais conceitual sobre acessibilidade

- Acessibilidade é algo super importante nos dias de hoje. 
    - Acessebilidade é essencial para desenvolvedores e organizações que desejam criar sites e ferramentas da Web de alta qualidade e não excluir as pessoas de usar seus produtos e serviços. 
    - A missão da iniciativa de Acessibilidade da WEB é levar a web a todo seu potencial para ser acessivel, permitindo que pessoas com deficiencia p participem igualmente na rede.

- Arvore de acessiblidade. Leitores de tela leem a arvore de acessibilidade. 

- WAI-ARIA: Acessible Rich Internet Applications
- Pelo console Web conseguimos ler a arvore de acessibilidade.
- Tags e atributos direcionados para a acessibilidade;

### Web Scraping

Rastreador: Crawler, as vezes também chamado de robo ou indexador é um termo genérico para qualquer programa usado para descobrir e examinar sites automaticamente seguindo links entre páginas web.

Exemplo Google Bot: Ferramenta do google que faz varredura no seu site e indexa o mesmo para ser vizivel na web. 

Técnica especifica para otmiziação do HTml para fazer as pesquisas no google.

Web Scraping: ação de uma aplicação entrar no site, extrair informações e gravar. 
Crwoling: enrtar em sites pré dfiniidos e depois usar estes dados para algum fim. 

Ileggal extrair sites? Em teoria se esta na internet é publico. É crime extrair estes dados? Hoje ele não é ilegal, mas se deve utilizar ele de forma ética. 

### Main, Header e Footer, aside, section, nav

````html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tags HTML 5 - Estrutural</title>
    <style>
        nav ul {
            display: flex;
            list-style: none;
            margin: 0;
        }
        nav ul li a {
            padding: 10px 15px;
            color: blue;
            text-decoration: none;
            border-radius: 15px 0;
        }
        nav ul li a:hover {
            color: white;
            background-color: blue;
            
        }
    </style>
</head>
<body>
    <header>Header
        <nav>
            <ul>
                <li><a href="#">Item 1</a></li>
                <li><a href="#">Item 2</a></li>
                <li><a href="tel: 55519999999">Telefone</a></li>
            </ul>
        </nav>
    </header>
    <!--
    main é uma tag principal que não pode ser filha de nem uma outra tag
    Existe somente um por página
    As demais tag's podem ser filhas de main.
    Define o conteudo principal dentro da página
    Main é uma tag estrutural. 
    
    section: Como se fosse uma div, porém a div é genérica. Section entra nos assuntos princiapis

    aside: Quando não é o assunto principal. 

    nav: HTML de navegação
    -->
    <main>
        <section></section>
        <section></section>
        <section></section>
        <aside></aside>
        <article><!-- colocar o artigo dentro. Um pode estar dentro de outro --></article>
        <time><!-- Dia especifico , ajuda nos motores de busca--></time>
        <blockquote><!--Citação, também da para apontar para a materia especifica. --></blockquote>
        <q><!-- citação pequena. Também da para colocar a fonte da citação --></q>
        <figure> <!--Conteiner de imagem. com uma descrição -->></figure>
        <figcaption></figcaption>
        <picture><!--Foncciona também em função da imagem --->></picture>
    </main>
    <footer>
        <address>R: Das Flores, numero e tals</address>
    </footer>
    <section>
        <header>Header 2</header>
        <footer>Footer 2</footer>
    </section>
</body>
</html>
````

### O que é SEO?

O que é SEO? Search Engine Optimization, otimização para mesanismos de busca. Melhorar o desempenho para mecanismos de busaca.

São um conjunto de técnicas para melhorar e colocar o site no topo de buscas. 

Google Search Console. busca metricas, mostra metricas com isto conseguimos ajustar o nosso site para melhorar a colocação. 

SEO é uma técnica. 

### Questionamentos:


1/10
Qual o significado da palavra "semântica"?
Estudo de deixa o HTML mais fácil de acessar na internet.
É HTML mais bem escrito.
É HTML com javascript.
É HTML mais bem estruturado.
A semântica é a área da linguística voltada para entender o significado das palavras.

Para que serve a tag ````<picture>````?
Para carregar imagens com resolução maior do que o normal.
Legenda aplicada em uma imagem.
Melhor a acessibilidade para textos e gráficos.
Para carregar imagens diferentes de acordo com a resolução da tela do dispositivo.
Carregar vídeos de outras extensões.

Qual das opções é que correto dizer sobre a tag ````<main>````?
Deve ser obrigatoriamente inserida dentro da tag ````<section>````
É usada para colocar somente em volta da tag ````<nav>````, mostrando que é a navegação principal.
Deve ser obrigatoriamente inserida dentro da tag ````<article>````
Deve ser obrigatoriamente inserida dentro da tag ````<header>````
Só pode ser usada uma por página HTML.

Qual o consórcio que regulamenta as regras definidas no HTML 5?
ARIA
WAI
Mozilla
Microsoft
W3C

GoogleBot, é um exemplo de quê?
Resultado das buscas do Google.
Links do resultado da busca do Google.
Relevância do seu site perante outros.
Sistema de renderização do Google Maps.
Crawler, usado para Web Scraping.

São exemplos de tags Estruturais do HTML 5
````<section>, <img>, <video>````
````<p>, <b>, <aside>````
````<video>, <audio>, <track>````
````<main>, <header>, <footer>````
````<section>, <aside>, <figcaption>````

São exemplos de tags de Mídia do HTML 5
````<section>, <img>, <video>````
````<main>, <header>, <footer>````
````<p>, <b>, <aside>````
````<video>, <audio>, <track>````
````<section>, <aside>, <figcaption>````

Para que serve o atributo cite, nas tags ````<blockquote> e <q>````?
Gera um link clicável para a fonte daquela citação.
Server para deixar o texto em negrito e com mais ênfase.
Coloca aspas duplas automaticamente no conteúdo.
É o atributo onde você insere o link da página que originou aquela citação.
Serve para deixar o texto mais claro e levemente itálico.

Para acessibilidade, para que serve o atributo alt de uma tag ````<img>```` ?
Utilizado para aumentar a resolução das imagens.
Serve para aumentar a quantidade de pixels de uma imagem.
Serve para navegadores indexarem melhor nas buscas.
O mesmo que a tag ````<td>````.
Serve para leitores de tela, conseguirem ler o descritivo de uma imagem.

Qual a sigla da iniciativa voltada para acessibilidade no HTML?
Mozilla Foundation.
W3C - World Wide Web Consortium.
Microsoft Azure.
WAI - Web Accessibility Initiative.
HTML - Hypertext Markup Language.

## HTMl recursos especiais

- O que vai ser abordado:
    - datalist
    - cod, kbd, pre
    - details, summary
    - mark, com java script
    - meter
    - canvas
    - Atributos uteis no html 5

### Datalist

datalist: Alternativa ao select

````html
    <input type="search" name="search" />
    <datalist id="browsers">
        <option value=>Selecione um navegador</option>
        <option value="chrome"></option>
        <option value="firfox"></option>
        <option value="Edge"></option>
        <option value="Safari"></option>
        <option value="Opera"></option>
    </datalist>
````

### code, kbd e pre

````html
    <p>Para copiar esta informação, <kbd>CTRL</kbd> + <kbd>C</kbd></p>
    <p> para trocar o fundo de um elemento, utilize o comando<code>Background-color</code>
    <pre>Gera um texto formatado</pre>
````

### Details e summary

````html
    <details>
        <details>
            <summary>como troco o fundo de um elemento.</summary>
            <p>para executar esta ação, utilize o comando background collor</p>
        </details>
    </details>
````

### Mter e progress

````html
<meter><!--Metter vai aumentando em dirção a 100%, tipo temperadturas-->></meter>
<progress><!--progress, começo, meio e fim.--></progress>
````

### Mark e JavaScript

````html
<input type="text" name="" id="busca"><br>
<p id="descricao">
    Os nossos cursos e programas de formação são criados por empresas mais inovadoras do mercado aplicando uma metodologia.
    Domine as tecnologias utilizadas no mercado e também mergulhe nas atuais tecnologias que impactarão o futuro dos negócios digitais.
</p>

<script>
    // Seleciona o campo de entrada e o parágrafo de descrição
    var searchField = document.getElementById('busca');
    var descriptionElement = document.getElementById('descricao');
    var originalText = descriptionElement.innerHTML;

    // Função para marcar a palavra encontrada
    function highlightText() {
        var searchText = searchField.value;
        
        // Reseta o texto original para buscar novamente
        descriptionElement.innerHTML = originalText;
        
        if (searchText.trim() !== "") {
            var regex = new RegExp(`(${searchText})`, 'gi');
            // Substitui o texto encontrado pela versão com <mark> para destacar
            descriptionElement.innerHTML = originalText.replace(regex, '<mark>$1</mark>');
        }
    }
    // Adiciona um evento de input para ativar a função ao digitar
    searchField.addEventListener('input', highlightText);
````

### Canvas Parte 1

Teg relacionada com a tag canvas. Podemos manipular graficos dentro do navegador. Cirar animações ou coisas do tipo. 

- Conte de conhecimento: codepen exemplos canvas
- Bastante utilizados em gráficos 

### Novos atributos do HTML 5

[Diferenças do HTMl 4  para o HTML 5](https://www.w3.org/TR/html5-diff/)
- autofocos, carregando a página ele ja cai direto dentro do campo
- placeholder, exemplo de campo como legenda no campo
- required, obrigatoriedade do atributo.
- disabled dentro do fieldset. 
- maxlength, delimite a quantidade de caracteres do texto. 
- minlength, minimo de caracteres
- atributo form, colocar dentro do campo o form, relacionado ao astributo. 
- content editable, pode alterar o atributo no html.

### Questionário

O que faz a tag ````<meter>````?
Não existe esta tag.
Utilizada para saber o status de um e-mail enviado.
Serve apenas para medir o espaço em disco.
Server para ilustrar medidas, como temperatura, espaço em disco, entre outros.
Serve para definir uma barra de progresso. Geralmente ilustra um carregamento que tem um começo, meio e fim.

O que faz o novo atributo "maxlength" em um textarea?
Permite colocar imagens no campo textarea.
Permite que a largura ultrapasse o tamanho da tela do dispositivo.
Não permite Copiar e colar conteúdo.
Define uma quantidade mínima de caracteres a serem inseridos.
Define uma quantidade máxima de caracteres a serem inseridos.

Qual a finalidade da tag ````<summary>````?
Coloca um resumo da notícia dentro da tag ````<article>````
Vai no rodapé da página, descreve um resumo da página como um todo. Aceita no máximo 250 caracteres.
Vai no header da página, descreve um resumo da página como um todo. Aceita no máximo 250 caracteres.
Usado dentro da tag ````<details>````, ele exibe um título, facilitando o entendimento sobre o aquele texto abaixo se refere.
Em uma tabela, coloca um resumo do que ela se refere, e sobre os dados que estão contidas nela.

O que faz o atributo "placeholder" na tag ````<input>````?
Torna o campo numérico.
Coloca um tamanho limite para você colar valores nele.
Não faz nada.
Torna o campo obrigatório.
Coloca uma espécie de marca d'agua no campo, mostrando como deve ser os valores inseridos nele.

O que faz a tag ````<canvas>````?
Serve para colocar comandos javascript em uma página web.
Delimita um espaço no HTML para colocar vídeos.
Server para colocar CSS em uma página Web.
Torna o carregamento da página assíncrono.
Tag voltada para ser manipulada graficamente, via javascript. Muito utilizada para desenvolvimento de jogos.

O que faz o atributo "required" na tag ````<select>````?
Torna o campo numérico.
Não faz nada.
Coloca um tamanho limite para você colar valores nele.
Seleciona sempre um valor, mesmo não selecionando nenhum.
Torna o campo de preenchimento obrigatório.

O que faz o atributo "form" na tag ````<input>````?
Deixa o conteúdo em negrito e desabilitado.
Apenas para tornar mais acessível os campos.
O campo, ao preencher, o formulário é validado automaticamente.
Seleciona o primeiro item da lista.
Mostra para o navegador, de qual formulário, aquele campo se refere.

O que faz a tag ````<progress>````?
Não existe esta tag.
Utilizada para saber o status de um e-mail enviado.
Server para ilustrar medidas, como temperatura, espaço em disco, entre outros.
Serve para definir uma barra de progresso. Geralmente ilustra um carregamento que tem um começo, meio e fim.
Serve apenas para medir o espaço em disco.

O que é DOM?
É o CSS depois de carregado e manipulado pelo javascript.
Determina o ranking que aparece seu site na busca do google.
Tecnologia utilizada somente libs como React.
É o Javascript depois de carregado e pronto para uso.
Document Object Model (Modelo de Documento por Objetos). É uma convenção, fiscalizada pela W3C, para representação de objetos em documentos html.

Para que serve a tag ````<kbd>````?
Serve para delimitar um texto que se refere comandos CSS.
Não existe esta tag.
Apenas ajuda a colocar uma cor no html.
Serve para delimitar um texto que se refere a teclas do teclado.
Serve para delimitar um texto que se refere comandos javascript.

### Desafio 

- Está dentro do desafio wikipedia. 

