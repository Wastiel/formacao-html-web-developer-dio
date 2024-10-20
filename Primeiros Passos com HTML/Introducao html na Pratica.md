# Primeiros Passos com HTML

## Onboarding

Aprender na prática como utiliza e desenvolver com html

- Vão ser abordados os seguintes assuntos: 
    - Ferramentas utilizadas.
    - Inspetor de elementos do navegador
    - Estrutura básica do HTML
    - Tags
    - Astributos Básicos
    - Executando uma página HTML
    - Textos
    - Listas ordenadas e não ordenadas
    - links

- Aprender a instalar e configurar o ambiente de desenvolviment. Entender o funcionametno do inspetor de elementos do navegador e criar sua primeira página HTML

## Ferramentas utilizadas

- Preparação do ambiente:
    - Fazer o download Visual Studio code (procurar o software no google).
    - Nos plugins do Vscode, instalaro live Server.

## Inspetor de Elementos

- Apertar F12 no navegador, abrimos o console no navegador (Inspetor de elementos). 
- Dentro do F12, entramos em elements.
- Ao navegarmos pela página pegamos e navegamos pelos elementos podendo ver como o elemento é construido
- Podemos alterar de forma prévia os determinados elementos. 

## Estrutura básica do HTML

- Definir uma pasta onde o projeto vai ficar.
- Pagina principal da nossa aplicação vai ser o index.
- Consiste o HTMl:
    - Tag no html tem uma palavra dentro
    - Princpais tags do html:
        - HTML
        - HEAD
        - BODY
    - No Head, vai carregar antes de mostrar para o usuário. 
[Exemplo de Página HTML](index.html)

## Falando sobre Tags
    
- O que são TAG's e qual é seu funcionamento.
- Tudo que estiver dentro da Tag o navegador vai executar conforme ainstrução da própria TAG este é o funcionamento da TAG.
- Algumas Tags não tem fechamento.
- Algumas Tag's tem atributos que mudam o comportamento das tag's.

## Atributos das Tags

- id: identificar a tag
- style: formatar o html da forma que instruimos
- class: Podemos identiicar com o nome, e padronizamos conforme o determinado nome. 

## Textos

O usuário vai entrar no determinado site e vai acabar lendo textos. 
A referencia sobre textos é a tipografia.

- Principais Tipografias no HTML em formato de Tag
    - H1 (H2... H6): Titulos
    - p: siginifica o paragrafo ditiado no HTML
    - blockquote: Sitação
    - strong: Deixar o texto forte
    - u: Marca o texto
    - i: deixa em italico


## Listas

3 tipos de listas

Ordenadas e não ordenadas:

- Maçã
- Banana
- Laranja

Exemplo em HTML:
```html
<ul>
  <li>Maçã</li>
  <li>Banana</li>
  <li>Laranja</li>
</ul>

Lista ordenada:

1. Primeiro item
2. Segundo item
3. Terceiro item

Exemplo em HTML:
```html
<ol>
  <li>Primeiro item</li>
  <li>Segundo item</li>
  <li>Terceiro item</li>
</ol>
```

Lista de Definição: 

Exemplo em HTML:
```html
<dl>
  <dt>HTML</dt>
  <dd>Linguagem de marcação para criar páginas da web.</dd>
  <dt>CSS</dt>
  <dd>Folhas de estilo em cascata usadas para estilizar páginas da web.</dd>
</dl>
```

## Links

Vamos criar uma navegação no nosso site.
O link é uma ligação de uma página com a outra

A tag do link/ancora é o a

Exemplo de link: <a href="http://dio.me">Dio</a>
- Exemplo de comportamento de abertura:
    - target="blank",a bre em uma nova aba
    - target="self", abre na mesma aba
- Atributo title, descreve o texto em que o mouse fica em cima

## Questionários


1/10
O que são tags no HTML?
São marcações em redes sociais (hashtags).
São tipos de imagens publicadas na internet.
Mostra para o usuário o que ele está fazendo.
Não servem para nada.
São comandos utilizados para informar o navegador a estrutura do site.

Para que serve a tag <a>?
Colocar uma imagem ancorada.
É uma tag apenas estrutural.
Colocar um hyperlink em nossa página.
Serve apenas para executar javascript.
Abrir um novo formulário.

Estrutura correta de uma lista não-ordenada
<ul> <li>Item 1</li> <li>Item 2</li> <li>Item 3</li> </ul>
<ul> </li>Item 1<li> </li>Item 2<li> </li>Item 3<li> </ul>
</ul> </li>Item 1<li> </li>Item 2<li> </li>Item 3<li> <ul>
<ol> <li>Item 1</li> <li>Item 2</li> <li>Item 3</li> </ol>
<ul> <ol>Item 1</ol> <ol>Item 2</ol> <ol>Item 3</ol> </ul>

O que faz o atributo target="_blank" na tag de link?
Abre o link em outra aba no navegador.
Abre apenas uma página em branco na mesma janela.
Toca uma música.
Abre um link na mesma janela do navegador.
Abre um link dentro de uma tabela.

Estrutura correta de uma lista ordenada
<ul> <ol>Item 1</ol> <ol>Item 2</ol> <ol>Item 3</ol> </ul>
<ul> <li>Item 1</li> <li>Item 2</li> <li>Item 3</li> </ul>
</ul> </li>Item 1<li> </li>Item 2<li> </li>Item 3<li> <ul>
<ul> </li>Item 1<li> </li>Item 2<li> </li>Item 3<li> </ul>
<ol> <li>Item 1</li> <li>Item 2</li> <li>Item 3</li> </ol>



São exemplos de tags geralmente aplicadas em Textos
<h1>, <p>, <b>, <h4>
<div>, <head>, <html>
<input>, <table>, <tr>
<form>, <label>, <textarea>
<button>, <ol>, <li>, <ul>

O que faz a tag <p>?
<p> significa picture (imagem). Insere uma imagem em nossa página.
Inicia uma ponta, onde inicia uma tabela, até outra.
É uma tag apenas estrutural
Adiciona recurso multimídia em nossa página.
Inicia e termina um parágrafo no texto.

Exemplos de atributos básicos de tags
height, width, color.
border, cellpadding, width.
id, style, name, class.
caption, id, title.
name, description, summary.

O que faz a tag <title>?
É usada para dar titulo em uma tabela.
É o título de uma lista não ordenada.
O mesmo que a tag <a>.
O mesmo que a tag <h1>. Deixa um texto maior e mais escuro.
Localizada dentro de <head>, ela muda o texto que aparece na janela (ou aba) do navegador.

O que faz a tag <title>?
É usada para dar titulo em uma tabela.
É o título de uma lista não ordenada.
O mesmo que a tag <a>.
O mesmo que a tag <h1>. Deixa um texto maior e mais escuro.
Localizada dentro de <head>, ela muda o texto que aparece na janela (ou aba) do navegador.

O que faz a tag <body>?
Define o corpo do texto.
Ela define o corpo da página HTML, o que aparece para o usuário.
Não existe esta tag.
Define o local de inserir apenas links e tabelas.
Delimita o HTML para executar o javascript.

## Desafio
<a href="desafio.html">Desafio dio</a>