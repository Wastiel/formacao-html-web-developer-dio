# HTML I: Conceitos Basicos

## Trabalhando com formulários HTML

### Apresentação

Principal aprendizado deste curso são Formulários.
Vai ser abordado algumas Tags focadas em formulários. 

- Conteudo Abordado: 
    - Tag ````<form>````
    - Tag ````<input>````
    - Tag ````<checkbox>```` e ````<radio>````
    - Tag ````<button>````
    - Tag ````<select>````
    - Tag ````<textarea>````

Rever algumas tags HTML, entender como funcionam os formulários e como uma informação enviada através de um formulário chega até o servidor.

A ideia aqui é somente formatar o formulário. 

### Tag Form

O que seria um formulário? Um trecho do HTMl onde vai conter campos que o usuário vai inserir informações. 
Formulário anda de mão dadas com servidores. 

O formulario guarda as informações e envia para o servidor, onde são guardado informações em um banco de dados. 

O formulário consiste em uma tag ````<form>````, que abre e fecha. 

````html
    <form name="signup">
        Nome: <input type="text" name="name" /><br>
        idade: <input type="number" name="age" /><br>
        Senha: <input type="password" name="password" /><br>
        <button type="submit">Enviar</button>
    </form>
````

Dentro dos formulários, temos os protocolos Http e Http's, focado na segurança do trafego de informações.
As validações do formulário são feitas em javaScript.

Mandar um formulário para outro, somente se formos proprietário.

- Meios de mandar o formulário:
    - Get: Envia dados através da URL em uma requisição HTTP, geralmente usado para solicitações simples ou leitura de dados. Os parâmetros são visíveis na URL.
    - Post: Envia dados encapsulados no corpo da requisição HTTP, mais adequado para envio de informações maiores ou sensíveis. No lado do servidor, esses dados são desencapsulados para processamento.
    - target: Define onde o resultado da submissão do formulário será exibido, podendo ser na mesma aba, em uma nova aba/janela ou em um iframe.
    - autocomplete: Indica se o navegador deve armazenar os dados preenchidos nos campos do formulário, permitindo o preenchimento automático em futuras visitas.
    - on: através de um evento. 

### Tag Input e Seus Tipos

Input: Tag para inserir diversos valores
Nem todos os navegadores tem implementados certos recursos, assim a tag input tem diferenças. 

Diversos Tipos de input:
````html
    <form>        
        <label>Text: </label><input type="text" /><br>
        <label>Number: </label><input type="number" min="0" max="99" step="5"/><br>
        <label>Button: </label><input type="button" value="Enviar"/><br>        
        <label>Button: </label><input type="range" value="10"/><br>
        <label>Color: </label><input type="color"/><br>
        <label>E-mail: </label><input type="email"/><br>
        <label>URL: </label><input type="url"/><br>
        <label>Date: </label><input type="date"/><br>
        <label>Week: </label><input type="week"/><br>
        <label>Month: </label><input type="month"/><br>
        <label>CheckBox: </label><input type="checkbox"/><input type="checkbox"/><br>
        <label>Radio: </label><input type="radio" name="aceita"/><input type="radio" name="aceita"/><br><br>
        <label>Hidden: </label><input type="hidden"/><br>
        <label>File: </label><input type="file"/><br>
        <label>Search: </label><input type="search"/><br>
        <label>Button: </label><input type="submit"/><br>        
    </form>
````

### Check e Radio

Vamos abordar dois campos que vamos utilizar muito no futuro
Checkbox pode ter muitas seleções.

A ideia do checkbox é selecionar multiplos valores. Enviamos para o servidor todos enviados. 

Quando enviamos o checkbox para o servidor, temos que configurar ele da seguinte maneira: 

````html
<form method="post">
<input type="checkbox" name="opicional[]" value="queijo"> + queijo <br>
````

Radio Button é um ou outro. Não deixa multipla opções.


### Bytton e seus Tipos

Vamos verificar botões com funcionalidades diferentes

````html
<button type="button" ></button>
<button type="reset" ></button>
<button type="submit" ></button>
````

Temos que validar o formulário também no backend.

### select e seus tipos

Combo Box ou Select Box: Lista pé definida do que queremos que o usuários selecione.

````html
  <label for="opcoes">Escolha uma opção:</label>
    <select id="opcoes" name="opcoes">
        <option value="opcao1">Opção 1</option>
        <option value="opcao2">Opção 2</option>
        <option value="opcao3">Opção 3</option>
        <option value="opcao4">Opção 4</option>
    </select>
````

### Text Area

Tag para inserir informações de texto

````html
<textarea rows="20" cols="50" name="message" ></textarea>
````

### Questionário:

O que é a tag ````<input type="range">````?
Cria um campo numérico com setinhas pra cima e pra baixo.
Cria uma janela de aviso para usuário.
Cria um controle interativo que aumenta e diminui na horizontal um valor numérico.
Não existe este tipo de input.
Cria um campo texto que vai de A a Z.

É característica do Checkbox:
Permite selecionar mais de um valor para um mesmo campo.
Tem formato circular e quando selecionado fica preenchido.
Tem o formato quadrado, e quando selecionado fica vazio.
Não permite selecionar mais de um valor para um mesmo campo.
Não existe este tipo de formulário.

É característica do RadioButton
Permite selecionar mais de um valor para um mesmo campo.
Tem o formato quadrado, e quando selecionado fica vazio.
Não existe este tipo de formulário.
Permite selecionar apenas um valor para um campo específico.
Tem formato quadrado e quando selecionado fica preenchido.

O que faz o ````<button type="reset">````?
Recarrega a página toda com o formulário sem informações.
Envia um comando reset para o servidor.
Limpa o campo password do formulário.
Não existe este tipo de button.
Limpa os campos do formulário.

O evento onSubmit do formulário é mais utilizado para...
Executar uma mensagem de sucesso com som, quando enviado o formulário.
Para liberar o envio, caso o usuário pressione CTRL + Shift + Q.
Validar o formulário antes do envio ao servidor.
Executar um CSS.
Aplicar uma ação em um campo específico.

O que faz o atributo action de um formulário html?
É o mesmo que GET e POST.
Define o caminho de onde as informações do formulário serão enviadas.
Coloca as informações no endereço da página.
Serve para fazer uma ação javascript.
Define campos escondidos e visíveis.

O que é a tag ````<input type=""number"" min=0 max=100 step=10 />````
Renderiza um campo numérico, que aceita no mínimo 0, e no máximo 100. Clicando nas setinhas, aumenta de 10 em 10, e diminui de 1 em 1.
Renderiza um campo numérico, onde você pode clicar nas setinhas apenas 10 vezes.
Renderiza um campo numérico, que aceita no mínimo 0, e no máximo 100. Clicando nas setinhas, aumenta ou diminui de 10 em 10.
Campo numérico que aceita números negativos.
Renderiza um campo numérico, que aceita no mínimo 10, e no máximo 100. Clicando nas setinhas, aumenta ou diminui de 1 em 1.

O que o atributo multiple faz na tag ````<select>````?
Permite selecionar múltiplos arquivos.
Permite selecionar múltiplos itens da lista pré-definida.
Não existe esta tag.
Envia o formulário para múltiplos destinos.
Desativa o campo.

Qual a diferença entre o method GET e POST?
GET = não existe este método e POST = envia as informações na url.
GET e POST são métodos apenas utilizados no javascript.
GET = pega e envia informações para o mesmo site e POST = somente envia informações para o mesmo site.
GET = envia as informações na url e POST = envia os formulários com dados embutidos.
GET = pega informações de outros sites e POST = envia informações para outros sites.

## Estruturando seu HTML + Formatações

Foco em algumas Tags do HTML para formatação de documento. 

- Formatando textos ````<strong>, <i>, <b>, <u>````
- Formatando textos: ````<font>````
- Tag ````<div> e <span>````
- Tag ````<fieldsets>````
- Tag ````<embeds>````
- Tag ````<iframes>````
- Resenha sobre cores

Entender como formatar alguns textos pensando também em acessibilidade. Estruturar melhor seu HTML, preparando ele para aplicar o css. Conhecer como funcionam as cores no css

### Formatando textos

Semantica no HTML: Uma forma de você estruturar o seu HTML que ao olhar, saibamos o que aquela estrutura quer dizer.

Tag font: Basicamente utilizada para formatar a sua fonte, a sua letra. O mais indicado é utilizar a fonte via CSS, mas o conteudo aqui é mais para aprendizado. 

Exemplos de textos

````html
<body>
    <!--Italico: Deixar o txto italico-->
    <i>Programe seu futuro global agora!</i><br>
    <!--Negrito: Deixar o texto em negrito-->
    <b>Programe seu futuro global agora!</b><br>
    <!--underline: Texto Sublinhado-->
    <u>Programe seu futuro global agora!</u><br>
    <!--mark: Texto Marcado -->
    <mark>Programe seu futuro global agora!</mark><br>
    <!--sup: texto superior-->
    <sup>Programe seu futuro global agora!</sup><br>
    <!--sub: texto inferior-->
    <sup>Programe seu futuro global agora!</sup><br>
    <!--bloquote: Espacamento do lado esquerdo para formatar o texto-->
    <blockquote>Programe seu futuro global agora!</blockquote><br>
    <!--Strong: enfase no texto-->
    <strong>Programe seu futuro global agora!</strong><br>

    <!--Font: enfase no texto, tem que ter os atributos para funcionar-->
    <!--Font: A fonte que utilizarmos tem que estar no computador, senão o html pega uma fonte padrão-->
    <!--Font: A fonte que utilizarmos tem que estar no computador, senão o html pega uma fonte padrão-->
    <!--Font: Conseguimos colocar uma fonte em sequencia caso não exita a primeira-->
    <font color="red" face="arial, tahoma">Programe seu futuro global agora!</font><br>
</body>
````

### Div e Span

A estrutura do HTMl é bem importante, por isto vamos verificar as tags div e span e são usadas para estruturar o HTML. Elas são consideradas tag's coringas.

Sempre estruturamos o HTML de fora para dentro sempre. 

Div é com display block... Ela trava a tela inteira. 


````html
<div id="menu-lateral">
    <div id="links">
        <ul>
            <li>Link 1</li>
            <li>Link 2</li>
            <li>Link 3</li>
        </ul>
    </div>
````

### Fieldset

Fildset é tipo o label do formulario. 

````html
    <form id="filterForm">
        <fieldset>
            <legend>Exemplo Formulario</legend>
            <div>
                <label for="category">Selecione uma categoria:</label>
                <select id="category" name="category">
                    <option value="todos">Todos</option>
                    <option value="frutas">Frutas</option>
                    <option value="vegetais">Vegetais</option>
                    <option value="laticinios">Laticínios</option><br>
                </select>
            </div>            
            <div>
                <label>Campo Texto</label><input type="text"/><br>
                <label>Campo Texto</label><input type="text"/>
            </div>
            <button type="submit">Enviar</button>
        </fieldset>
    </form>
````

### Embeds

Surgiu na decada de 90 um problema de estrutura de carregar toda a página. Carregamento da página em pequenos pedaços.

Começou a surgir a necessidade de colocar plugins no navegador para esta aceleração. 

O embed veio para carregar uma midia externa em um trecho do código com mídia. 

Hoje ja temos outra tag para substituir o embed que é a tag ````<video>````.

### iframe

Iframe: Mesmo funcionamento que o embed. 
Iframe pode afetar a segurança do seu site. 
Serve para carregar uma página dentro de outra página.

````html
<!-- Exemplo iframe disponibilizado pelo google, tanto do maps, quanto do youtube-->

 <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d9769.498516650956!2d-51.16245255324268!3d-30.035727596210396!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1spt-BR!2sbr!4v1729785364190!5m2!1spt-BR!2sbr" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

 <iframe width="1250" height="703" src="https://www.youtube.com/embed/GNm5drtAQXs?list=RDGNm5drtAQXs" title="Fall Out Boy - This Ain&#39;t A Scene, It&#39;s An Arms Race (Official Music Video)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

````

### Resenha sobre cores

Vamos usar muito cores no CSS e no HTML
Navegadores modernos aceitam aproximadamente 140 nomes de cores. 

- Formas de aplicar cor no navegador:
    - RGB
    - HEX
    - HSL
    - RGBA
    - HSLA

### Questionário

Que cor é rgba(255, 0, 0, 0.5)?
Preto com transparência 50%.
Amarelo com transparência 50%.
Vermelho com transparência 50%.
Verde com transparência 50%.
Azul com transparência 50%.

Qual a diferença entre ````<strong>```` e ````<b>````?
Apesar de aparentarem ser a mesma coisa, ````<b>```` tem mais semântica do que o ````<strong>````.
Nenhuma diferença.
Apesar de aparentarem ser a mesma coisa, ````<strong>```` tem mais semântica do que o ````<b>````.
````<strong>```` não tem semântica nenhuma, assim como o ````<b>````, mas deixa o texto maior e itálico.
````<strong>```` não tem semântica nenhuma, assim como o ````<b>````, mas deixa o texto maior e sublinhado.

O que faz a tag ````<iframe>````?
A mesma coisa que ````<embed> e <object>````, só que apenas para navegadores antigos.
Só serve para colocar youtube na página.
Serve para isolar o conteúdo da página para utilizar javascript de forma segura.
Só serve para colocar o google maps.
Permite inserir conteúdos externos (web ou do projeto) dentro de sua página html.


Qual o display padrão da tag ````<div>````?
display: none;
display: inline-block;
display: inline-none;
display: block;
display: not-show;

O que o atributo face faz na tag ````<font>````?
Altera a cara do usuário.
Aplica CSS no paragrafo inteiro.
Altera a cor do parágrafo.
Altera o texto para leitores de tela (acessibilidade).
Altera a fonte do texto.

O que faz a tag <u>?
Coloca um underline no texto.
Coloca o texto em negrito.
Coloca o texto em itálico.
Coloca o texto em itálico e sublinhado.
Não faz nada.

O que faz a tag ````<blockquote>````?
Insere dados em blocos.
Não funciona em nenhum navegador.
Define uma margem a direita do texto.
Define uma citação longa dentro do texto.
É apenas uma tag estrutural.

O que faz a tag ````<mark>````?
Coloca negrito, itálico e sublinhado tudo de uma vez.
Deixa o texto com aparência de escrito a mão.
Melhora na questão de SEO.
Troca o formato do texto.
Aplica um destaque ao texto, semelhante a um marca textos.


O que faz o ````<fieldset>````?
Faz com que os campos do formulário fiquem de outra cor para facilitar o preenchimento.
Apenas aplica uma margem esquerda ao formulário.
Aplica uma margem esquerda e direita ao formulário.
Usado para delimitar textos, aplicando uma margem esquerda e um itálico.
É uma forma de agrupar campos de formulário, deixando-os mais visivelmente melhores.

## Trabalhando com Mídias

- Percurso do conceito de audio
    - Entendendo tags de mídia
    - Tag````<img>````
    - Tag````<audio>````
    - Tag````<video>````
    - Tag````<track>````
    - Tag````<iframe>````

### Tags de mídia

São tg's relacionados a som e a imagens. São próprias do HTML 5.
Pontos inportantes relacionado a acessibilidade

### Tag img

A tag de imagem tem uma complexidade maior do que aparenta. 

- Propriedades da tag img
    - src: Caminhou ou local da imagem
    - width: largura
    - alt: descrição da imagem
    - title: titulo da imagem

- tipos de img
    - png
    - giff
    - jpg
    - svg

### Tag Audio

É uma tag simples ````<audio>```` ela é complementada pela tag ````src````. 

````html
<audio controls>
    <source src="musica.mp3">
    Seu navegador não suporta audio.
</audio>
````

### Tag Vídeo

````html
<video controls>
    <source src="musica.mp4">
    Seu navegador não suporta vídeo.
</video>
````

### Tag Track

A tag track fica dentro do vídeo aidicionando legendas.

`````html
<video controls>
    <source src="musica.mp4">
    <track src="legenda.vtt" kind="captions" srclang="pt-br">
    Seu navegador não suporta vídeo.
</video>
`````

### Tag ifrmae

Se usa muito para youtube e google maps. 

### Questionário

Para que serve a tag <track>?
Serve para colocar faixas musicais na tag áudio.
Adiciona controles nos vídeos.
Adiciona legendas ao seu vídeo.
Adiciona trechos de musicas sobrepostas nos vídeos.
Serve para carregar imagens externas no vídeo.

O que o atributo default faz na tag <track>?
Permite definir qual musica será a padrão ao carregar a página.
Não tem utilidade.
Permite abrir um vídeo especifico no chrome.
Permite definir qual vídeo será o padrão ao carregar a página.
Permite definir qual legenda é a padrão ao carregar a página.

O que acontece com a imagem se apenas atribuir uma largura (width) na tag <img>?
Diminui o tempo de carregamento da imagem.
Aumentando ou diminuindo vai distorcer toda a imagem, deixando o navegador lento.
O navegador redimensionará proporcionalmente a imagem, evitando que ela distorça.
O navegador redimensionará a imagem, distorcendo por completo.
Não permite adicionar apenas o atributo width. Deve se atribuir height também para funciona.

Por que usar ````<video> ou <audio>```` ao invés de ````<embed>```` ?
Embed é melhor para acessibilidade, mas não funciona em vário navegadores.
Nenhuma diferença. Tag embed só muda os controles do player e música e vídeo.
Não tem diferenças na verdade, a aparência do áudio só que é mais apresentável.
Navegadores não entendem a tag ````<embed>, já <video> e <audio>```` entendem.
Embed não tem um peso semântico. Já as tags video e audio, só de olhar, já sabemos que se trata de áudio e/ou vídeo.

O que são Gifs?
Imagens utilizadas para criação de imagens com som.
Vídeo de curta duração enviados por e-mail.
Imagens dinâmicas, não podem sofrer alterações na largura ou altura senão para de funcionar.
Imagens estáticas, que podem ser dimensionadas e não perdem qualidade.
Imagens interpoladas realizando animação.

O que faz o atributo controls, nas tags ````<video> e <audio>````?
Faz com que o navegador não renderize controles básicos para manipular a mídia. Play, Stop, Volume, etc...
Permite que o navegador renderize controles básicos para manipular a mídia. Play, Stop, Volume, etc...
Faz com que o navegador renderize controles básicos para manipular a mídia. Play, Stop, Volume, etc... Funciona apenas no vídeo.
Deixa todos os controles desabilitados do áudio ou vídeo.
Faz com que o navegador renderize controles básicos para manipular a mídia. Play, Stop, Volume, etc... Funciona apenas no áudio.

O que é multimídia?
É tudo relacionado a navegadores web.
É tudo relacionado a dispositivos móveis.
É tudo relacionado a som e imagem.
Textos e sons.
Apenas coisas relacionadas a áudio. Vídeos é cinematografia.


9/10
O que faz o align na tag ````<img>````?
Permite alinhar as imagens entre o cabeçalho e rodapé do site.
Alinha a imagem dentro de um texto.
Deixa a imagem com sombra para delimitar uma distância entre outras imagens.
Deixa a imagem com borda para alinhar com outras imagens.
Centraliza a imagem na tela.