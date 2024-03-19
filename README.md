![Banner Git Cheat](https://i.imgur.com/Qj4inph.png)

# <p align="center">Usando o git pela primeira vez</p>

Para usar o git pela primeira vez precisa configurar sua maquina ("Só é necessário fazer na primeira vez")

Use os seguintes comandos:

    git config --global user.name "Seu-Nome"

    git config --global user.email "seu-email-cadastrado-no-git-hub"

**Se fizer com outro e-mail não vai funcionar**
<br>
OBS: **O git tem que esta instalado**
<br>
[Baixe aqui o git](https://git-scm.com/downloads)

# <p align="center">Criando um Repositorio </p>

### <p>1 - Na sua pagina de perfil clique em repositórios </p>

![foto de repositorio](https://i.imgur.com/KW6FMkG.png)

### <p>2 - Depois em new</p>

![foto de repositorio](https://i.imgur.com/GU8h8cM.png)

### <p>3 - Adicione o nome e uma descrição(descrição é opcional) </p>

![foto de repositorio](https://i.imgur.com/alDXOct.png)

### <p>4 -selecione a caixa Add a README file e Clique em create repository</p>

![foto de repositorio](https://i.imgur.com/EKbGYer.png)

### <p>5 - Clique em code e logo em seguida vai abrir um pequeno menu copie a URL</p>

![foto de repositorio](https://i.imgur.com/kGBDmbw.png)

### <p> 6 - Va ate o lugar que você quer colocar o repositório e abra o terminal de sua preferencia (CMD / Bash)
(o git bash e o cmd  aparece se você clicar como segundo botão do mouse dependendo da configuração da maquina)

### 7 - git clone https://github.com/o-url-que-voce-copiou.git
![foto de repositorio](https://i.imgur.com/c5VOaM2.png)
<br>
### E seu repositório vai está pronto para ser usado!</p>

# <p align="center"> Como criar um repositório sem precisar clonar</p>
### <p> 1 - Crie seu repositório no git hub e vá ate a pasta que você quer transformar em repositório e abra o prompt e digite os seguintes comandos: </p>

### 2 - Inicia seu repositório
    git init

### 3 - Altera o nome da sua branch principal de master para main
    git branch -M main

### 4 - Adiciona seus arquivos
    git add . ou git add seu-arquivo.tipo

### 5 - Grava um snapshot permanente do arquivo no histórico da versão.
    git commit -m "curta descrição do que foi feito"

### 6 - Adiciona os arquivos ao repositório
    git remote add origin https://github.com/seu-repositorio.git

### 7 - Envia as modificações para Sua brabch main no repositório do GitHub
    git push -u origin main
    
# <p align="center">Criando uma nova branch, selecionando e excluindo  </p>
### <p>O que é uma branch?</p>
<p>Branch, ou ramo em português, é uma cópia das linhas de código de um software gerenciada por um sistema de controle de versão (VSC). A ramificação serve para ajudar as equipes de desenvolvimento a consertar bugs e inserir funções, separando o trabalho em andamento a consertar bugs e inserir funções, separando o trabalho em andamento do código testado e estável.</p>

### <p>1 - Va ate o git bash ou terminal de sua preferencia e digite os seguintes comandos 
### 2 -  Cria um novo branch
    git branch nome-da-branch

### 3 - Muda para a branch especificada e atualiza o diretório de trabalho
    git checkout nome-da-branch

### 4 - Lista todas as branches locais no repositório atual
    git branch

### 5 - Exclui o branch especificado
    git branch -d nome-da-branch

# <p>Subindo modificações para o git hub e atualizando seu repositorio<p>
### 1 - Abra o git bash ou qualquer terminal da sua preferencia e digite os seguintes comandos

### 2 - Adiciona todas as modificações adicionadas/modificadas
    git add .

### 3 - Lista os arquivos novos ou modificados para serem comitados
    git status

### 4 - Grava um snapshot permanente do arquivo no histórico da versão
    git commit -m "curta descrição do que foi feito"

### 5 - Envia as modificações para seu repositório no GitHub
    git push origin nome-da-branch
    
# <p align="center">Trabalhando em equipe</p> 
### 1 - Vá ate Repositório que você deseja colocar colaboradores clique em settings
![foto de repositorio](https://i.imgur.com/1W6FV3Y.png)

### 2 - No menu lateral vai aparecer a opção collaborators clique nela e vai pedir para você adicionar sua senha
![foto de repositorio](https://i.imgur.com/TzS0mMO.png)

### 3 - Clique em add people
![foto de repositorio](https://i.imgur.com/12gtgyl.png)
### 4 - Digite o nome de usuário ou email do colaborador 
![foto de repositorio](https://i.imgur.com/iznSodJ.png)
### 5 - Clique em add (Fulano) to this repository
![foto de repositorio](https://i.imgur.com/QeUugQk.png)



