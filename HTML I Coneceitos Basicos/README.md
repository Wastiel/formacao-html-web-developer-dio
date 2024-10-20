# Introdução aos Conceitos de Git Hub

## Princípios do Git e GitHub

Vamos aprender sobre Git, GitHub, colaboração de código, focando em facilitar processos para guardar códigos e construção de histórias.

Trabalhar com versionamento de código. 

### O que é Git e Github

Git: possiblita ter um controle melhor e organizado de versões do software. Traz um sistema que altere, gerencie as versões do nosso código. Como funciona a colaboração e como.

Github: Uma plataforma online que serve cmo repositório para guardar todos os nossos códigos fontes, como foco também no trabalho colaborativo. Plataforma online para comportar o nosso código.


### Como ambos se relacionam

- Hospedagem de repositórios: gerencia controle de versões e hospeda repositórios git remotamente.
- Colaboração em Equipe: Possiblita colaboração em equipe, varios desenvolvedores atuando em colaboração no mesmo projeto.
- Rastramento de Problemas e Projetos: Ferramentas para reasrear problemas, gerenciar integrações, além de controle de versão
- Forks e Branches: Isolar desenvolvimento de novos crecursos ou construçaõ de bugs.

### Instalação Git

Passo a passo para instalação

Download: [Download GIT](https://git-scm.com/downloads)
- Processo de instalação simples, next, next finish. 
- Adicionar o gitBash

Git bash vai ser a principal ferramente que vamos utilizar. "Terminal do Git"

Configuração:
- Atribuir nome
    - configuração: git config --global "wsilva"
- Atribuir e-mail
    - git config --global user.mail "*****@gmail.com"


### Criando conta no Git:

Processo de instalação:
- Ir para a página do git: [GIT](https://github.com/)
    - Inscrever-se
    - e-mail
    - senha
    - nome de usuário
    - Colocar o dódigo de verificacao
    - Conta pronta

### Princiapais comandos do Git


- git init 
    - inicia um novo respositório Git no diretório atual
- git clone [URL]
    - Clona um respositório do Git hub
- git add .
    - adicionar as alterações para peraparalas para commit
- git commit -m "mensagem"
    - Realiza o commit com as alterações adiconadas, incluindo uma mensagem que descreve as alterações feitas. 
- git status
    - Exibe o estado atual do repositorio, mostrando alterações pendentes e ja adicionadas
- git log
    - Mostra o historico de commits do repositório
- git branch
    - Lista todas as branch's
- git branch [nome-da-branch]
    - Cria uma nova branch
- git chackout [nome-da-branch]
    - Altera para uma branch específica
- git pull
    - Atualiza o respositório local com as alterações
- git push [remote][branch]
    - Envia os commits locasi para o repositório remoto.
- git remote -v
    - Lista os repositórios remotos configurados
- git fetch
    - Recupera as ultimas alterações do repositório, mas não faz merge automáticamente
- git reset
    - Desfaz as alterações no arquivo especifico, removendo-o do indice
- git rm [arquivo]
    - Remove um arquivo do repositório e inclui no próximo commit
- git diff
    - Mostra as diferenças entre as alterações que ainda não foram adicionadas ao indice
- git remote add [nome-remoto][URL]
    - adicionar um repositorio remoto com um nome especifico.
- git push add origin main
    - Execuando para efetuar push das alterações locais para o repositório online. 

### Questionário

Como interagir com comunidades de código aberto no GitHub?
Apenas enviando sugestões por e-mail.
Envolva-se em discussões em issues, participe de pull requests e contribua para projetos abertos.
Ignorando discussões existentes.
Limitando-se a apenas observar repositórios.
Criando repositórios privados.

Como fazer e acompanhar alterações no código usando Git?
git save guarda instantâneos das alterações.
git push envia alterações para o repositório remoto.
git track monitora automaticamente todas as mudanças.
git add para preparar alterações, git commit para confirmá-las e git log para exibir o histórico.
git show exibe apenas alterações não confirmadas.

Como criar um novo projeto Git e configurá-lo?
Utilize git new para iniciar um repositório.
Crie um novo projeto com git create.
Execute git start para começar um novo projeto.
Inicie um projeto com git setup.
Use "git init" para iniciar repositório e configure com "git config".

Quais são os recursos fundamentais do GitHub?
Histórico de atividades.
Templates e plugins.
Documentação e tutoriais.
Ferramentas de edição de código.
Repositórios, issues, pull requests, branches e colaboradores.

O que é controle de versão?
Um método para compactar documentos.
Um sistema de organização de pastas.
Registro de alterações em arquivos ao longo do tempo.
Um software para editar código.
Uma técnica para backup de arquivos.

O que são sistemas de controle de versão distribuídos, como Git?
São sistemas que não permitem rastrear alterações.
São sistemas sem a capacidade de ramificação.
São sistemas que permitem a colaboração em projetos através de cópias locais completas do repositório.
São sistemas exclusivos para grandes empresas.
São sistemas que funcionam apenas com conexão à internet.

## Autenticações 

### Nome e senha, Token e SSH


Tipos de autenticações para acessar os projetos
- Usuario e Senha
- tokens de acesso pessoal
- chaves SSH

### Chaves de implementação, SSO da SAML e LPDA

Chaves de Implementação: Chaves de implementação são como chaves especiais que permitem acesso a apenas um lugar específico no GitHub. Esa chave somente da permissão de leitura. Para algo diferente, deve ser configurado a chave para dar acesso a escrita.

Autenticação de dois fatores - SFA: É adicionar uma camada extra de segurança quanvo cê entra em sistes ou aplicativos além de mais uma prova de autenticação, sendo este um código adicional.

SSO do SAML:  é uma forma segura do GITHUB que permite constrolar os acesso da organização de maneira centralizada. São direcionados para acesso através de um login de um controle de LDAP.

LDPA: Protocolo usado para acessar e organizar informações em diretórios em grandes empresas. No contexto Enterprise Server é permitido integrar e gerenciar centralmente o acesso aos repositórios usando contas existentes. É compativel com vários serviços LDAP. 

### Nome e Senha e Token - Parte Prática 1

Primeiramente vamos acessa a nossa conta do Git
Vamos fazer um repositório de um projeto para testes

Primeiramente criamos um repositório: meu-repositorio-de-autenticacoes, colocamos descrição simples e marcamos o reade.me

Configuramos o nosso usuário e senha no git:

Configuração:
- Atribuir nome
    - configuração: git config --global "wsilva"
- Atribuir e-mail
    - git config --global user.mail "*****@gmail.com"
- Ver as configurações do git
    - git config --list

Agora vamos clonar o repositório que criamos e vamos clonar ele: "https://github.com/Wastiel/meu-respositorio-de-autenticacoes.git"

Utilizamos o comando "git clone https://github.com/Wastiel/meu-respositorio-de-autenticacoes.git", para puxar o nosso repositório.

Primeiro erro que enfrentamos é tentarmos adicionar coisas ao nosso reposiotorio, temos o err "fatal: not a git repository (or any of the parent directories): .git". Isto ocorre por que quando clonamos o repositório não caimos dentro do mesmo diretório.

Entramos dentro do diretório com o comando "cd" do linux.

git add .: adicionamos dados para preparar o commit
git. commit -m "mensagem": executamos a confirmação dos dados que irão para o nosso respositório
git push -u origin main: Mandamos as alterações para o nosso repositório.

Ao adicionarmos o comando anterior, nos é solicitado usuário e senha.
    - Este Usuáro e senha, ficam salvos dentro do gerenciador de senhas do windows

- Podemos criar tamém um token. Para isto vamos dentro de:
    - Perfil
    - Settings
    - <> Developer settings
    - colocamos tempos de expiração
    - Configurações de projetos
    - Posterior é nos gerado o token

Ao solicitar a autenticação no momento que subirmos as alterações, vamos adicionar o nosso token ao invés de usuário e senha. 

### SSH - Parte prática 2

Autenticação via chave de SSH, onde conseguimos utilizar multplas contas no nosso computador.

ssh-keygen: comando para gerar a nossa chave ssh

Ao criarmos a chave ssh, vamos no diretório criado a chave, entramos com o git bach e adicioanrmos a chamave publica no github.

cat id_***.pub, onde verificamos a chava publica.
Posteiror vamos no nosso git , vamos em settings, Chaves SSh e GPG e ali dentro colocamos esta determinada chave. 

Pegamos a chave do ssh do repositório e setamos a url:
    - git remote set-url origin **chave SSH**

### 2FA - Parte prática 3

Autenticação em 2 fatores

Entramos em Setting - Password nad authentication.
Duas formas de autenticação, via QR Code ou via sms, por um numero que esteja funcionando.

Vai ser gerado alguns tokens de segurança. Deve ser feito download do mesmo e salvo em um lugar super seguro. 

### Questionario: 

Como você pode habilitar a autenticação de dois fatores no GitHub?
Alterando sua foto de perfil.
Através das configurações de segurança da sua conta.
Enviando um e-mail para o suporte do GitHub.
Atualizando seu navegador.
Instalando um aplicativo de terceiros.

Como as chaves SSH tornam as interações com o GitHub mais seguras e convenientes?
Configurando Chaves de Implementação.
Permitindo conexões seguras a computadores remotos sem digitar senha ou token.
Utilizando Tokens de Acesso Pessoal (PATs).
Ativando a 2FA.
Integrando LDAP.

Como você pode adicionar uma camada extra de segurança ao acessar sua conta do GitHub, além de usar nome de usuário e senha?
Ativando a Autenticação de Dois Fatores (2FA)
Configurando Chaves SSH
Utilizando Tokens de Acesso Pessoal (PATs)
Integrando SSO do SAML
Implementando LDAP

Qual é a atual medida adicional de segurança implementada no GitHub para dificultar o acesso não autorizado?
SSO do SAML
Autenticação de Dois Fatores (2FA)
Configurando LDAP
Chaves de Implementação
Utilizando Tokens de Acesso Pessoal (PATs)

## Colaboração no GitHub

### Criando Repositórios e Branches, aplicando comandos Git

O que é um repositório: Local onde ficam guardados todos os detalhes de um código fonte. 

Beranches: é uma linha de desenvolvimmento separada. Um controle de versão. Uma linha segura de desenvolvimento. Ela somente entra na branch princial "Main", depois as alteraçoes são acopladas ao desenvolvimento principal.

Pull Rerquest e Merge: pedido de mesclagem, e dpois da visotrria se junta o código fonte ao ponto principal. 

Fork: Processo de cópia de um repositório ou um projeto. 

### Criando repositórios, Branches e pull Requests 

- Criar um Repositório local e adicionarlo ao nosso git:
    - Criamos uma pasta meu-repositório-teste.
    - Criamos um arquivo README.md dentro do nosso repositório.
    - Vamos ao GitHub e criamos o nosso repositório.
    - Observação: O github sugere o que temos que fazer para adicionar o repositorio criado a uma diretorio no computador
    - utilizamos o comando git add . para sinalizar os arquivos que vamos adicionar
    - git commit -m "para commitar o que construimos"
    - git add origin "Caminho do repositório"
    - git push -u origin main, para adicionar os dados ao nosso git hub

- Clonar um respositório:
    - Pegamos  a url do repositorio
    - git clone "O respositório copiado"

- Realizar alterações:
    - git add .
    - git commit -m "realizando alterações no projeto"
    - git push origin main

- Criar uma branch
    - git branch versao_01, cria a nova branch
    - git checkou versao_01, vamos ir para a nova branch
    - git checkout main, voltamos para a main
    - git merge versao_01, mandamos para a main a nossa branch

- Realizando um pull request:
    - Ir na pagina do repositorio e clicar em fork
    - clicamos em criar fork, o fork estamos apontando para uma branch de outra pessoa.
    - Criamos o cmmmit
    - criamos um pull request no proejto.
    - Posterior o titular da branch, tem que aprovar o pull request ou sinalizar mudanças ou alterações de correções que devem ser feitas.

### Tags

Tags, trazem oportunidades de trazer versões especificas do nosso código

- git tag -a V1.1 -m "Mensagem da versão"
- git push origin V1.1, mandamos a tage para o nosso repositório.
    
### Realeses

Considerada uma maneira de de c riar uma versão para empactor o software com notas de versão e arquivos para downloads e para uso de outras pessoas.

- Dentro do git, criamos uma realese.
    - Utilizamos uma tag 
    - Geramos uma realese Notes

### Gists

- Facilita a compartilhaçao de pequenos trechos de código.
- Se assemelha a criar um repositório
- Na programação podemos compartilhar trechos de códigos.
- Podem ser incorporados a sites divertos
- Após a criação, adicionamos uma parte do arquivo ou código para compartilhar com outras pessoas. Ou até alguma chamada especifico. 

### Issues

- Relacionado a codigos fontes
- Utilizadas para apontar correção de bugs e até mesmo rastrear tarefas, vinculadas ao código fonte.
- São solicitações de melhorias e correções de bug
- Ponto de colaboração, assim as issues podem ser abertas por qualquer pessoa.

- Pegamos um repositório para contribuirmos com o mesmo
    - Vamos abrir uma issue para melhorar o jogo da velha.
    - Issues no próprio GitHub, no repositório
    - Criamos uma issue, com título e descrição
    - conseguimos adicionar imagens.
    - É enviado um email sobre a issue
    - Podemos sinalizar sobre a issue, com comentarios e outros detalhes para quem solicitou a mesma.
    - Podemos atribuir a issue para alguém.

### Wikis

- São um readme melhorados. Podemos fazer uma documentação de forma mais detalhadas, detalhar de forma mais completa do que o próprio Reade.me
- Objetivo é a wiki ser uma documentação mais detalhada sobre o projeto.
- Organizar de uma forma mais profissional.
- Todos os detalhes do nosso nprojeto

### Pesquisas e Refêrencias

- Tipos de pesquisa do GitHub
    - Na busca do git, podemos buscar dentro do repositório de um usuário especifico.
    - Buscarmos de forma geral, trazendo por exemplo angular, conseguimos encotnrar diveros itens, como projetos, repositoirios, marketplace, wikis, users.

- Conseguimos procurar alguns conceitos maiores.
- Referencias de ligação automatica
    - Conseguimos referenciar a um outro pull request. 

- Conseguimos fazer muitas referencias dentro do nossos pull requestes. Ajuda a organizar o proejto e fluxos.

- Conseguimos associar um commit a uma issue.

### Questionário

Para que serve o Fork no GitHub?
Excluir um repositório no GitHub.
Realizar um Pull Request.
Criar uma cópia de um branch.
Criar uma cópia de um repositório para o seu próprio espaço no GitHub.

O que são Gists no GitHub?
Gists são pequenos repositórios Git e independentes, geralmente contendo um único arquivo, usados para compartilhar trechos de código.
Mensagens de erro no GitHub
Solicitações para criar novos repositórios.
Branches temporárias para testes.

O que é um Pull Request no GitHub?
Pedido para criar um novo branch.
Pedido para excluir um repositório.
Solicitação para fazer o download do repositório.
Um Pull Request é uma solicitação para revisão e mesclagem de alterações em um repositório.


Qual é o propósito das Wikis no GitHub?
Documentar bugs no código.
Fornecer uma plataforma colaborativa para documentação de projetos.
Gerenciar branches no repositório.
Facilitar a comunicação por meio de issues.

## Formatação Markdown

- Markdown é muito utilizado no Github, para documentação e apresentação de repositórios e projetos. 
- Todo repositório ou quase todo tem um READEME.me
- Detalhamento de projetos.
- É usado para detalhamento por ser mais simples.

### Sintaxe do Markdown

- Sintaxe Basica:
    - Cabeçalhos
        - # Título 1
        - ## Título 2
        - ### Título 3
        - #### Título 4
        - ##### Título 5
        - ###### Título 6
    - Formatação
        - *italico* ou _italico_
        - **Negrito** ou __Negrito__
        - ___negrito e italico___
    - Lista:  
        - Lista 1
        - Lista 2
            - Sublista
        1. Lista 1
        2. Lista 2
            1. Sublista
    - Link com imagem: 
        [Texto da Imagem](Link da imagem)
    - Adicionar a imagem dentro do markdown
        - ![Texto da imagem](link da imagem)
    - Crases significa código``
        - `Quando colocamos as crases, siginifica que é codigo`
    - Citações com simbolo de maior
        - >
    - Tabela:
        | Cabeçalho| Cabecalho2 |
        |----------|------------|
        |Texto1    | Texto2     |
        |Texto3    | Texto4     |
    - Check
        - [X] Tarefa 1
        - [] Tarefa 2

- Exercicio de construção 
    - [Atividade Exemplo](Exemplo.md)
---------
[git hub status](https://github.com/anuraghazra/github-readme-stats) 
---------
[Icones](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)

### Questionários

Como adicionar um bloco de citação no Markdown?
Usando asteriscos (*) no início de cada linha.
Adicionando pontos de exclamação (!) antes e depois do texto.
Cercando o texto com dois sinais de mais (++).
Utilizando colchetes angulares (>) antes do texto.

Como você pode enfatizar a importância de um texto no GitHub?
Usando três asteriscos (***) antes e depois do texto.
Utilizando barras invertidas (`) ao redor do texto.
Adicionando dois sinais de mais (++) no início e no final do texto.
Cercando o texto com um único asterisco (*) ou sublinhado (_).

Qual é a sintaxe correta para criar uma tabela no Markdown?
Separando as colunas com vírgulas.
Inserindo hashtags (#) no início de cada linha.
Usando colchetes angulares (<>) para definir colunas.
Utilizando barras verticais (|) para quebras de coluna e traços (-) para cabeçalhos.

Como criar uma lista ordenada no Markdown?
Inserindo asteriscos (*) antes de cada item.
Começando cada linha com um numeral seguido de ponto.
Utilizando barras verticais (|) para separar os itens.
Cercando os itens com colchetes angulares (<>) antes e depois.