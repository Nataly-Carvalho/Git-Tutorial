![Banner Git Cheat](https://i.imgur.com/Qj4inph.png)

# 🚀 Usando o Git pela Primeira Vez

Para usar o Git pela primeira vez, é necessário configurar sua máquina. *(Este passo só precisa ser feito uma vez.)*

### 🔧 Configuração Inicial:
```bash
git config --global user.name "Seu-Nome"
git config --global user.email "seu-email-cadastrado-no-git-hub"
```
⚠️ **Se usar um e-mail diferente do cadastrado no GitHub, não funcionará!**

🔗 **[Baixe o Git aqui](https://git-scm.com/downloads)** se ainda não estiver instalado.

---

# 📂 Criando um Repositório

### 🛠️ Passo a passo:

1️⃣ Na sua página do GitHub, clique em **Repositórios**.

   ![Repositórios](https://i.imgur.com/KW6FMkG.png)

2️⃣ Clique em **New**.

   ![Novo Repositório](https://i.imgur.com/GU8h8cM.png)

3️⃣ Adicione um **nome** e uma **descrição** *(opcional)*.

   ![Nome do Repositório](https://i.imgur.com/alDXOct.png)

4️⃣ Selecione **Add a README file** e clique em **Create Repository**.

   ![Criar Repositório](https://i.imgur.com/EKbGYer.png)

5️⃣ Clique em **Code** e copie a URL do repositório.

   ![Copiar URL](https://i.imgur.com/kGBDmbw.png)

6️⃣ No terminal, vá até o diretório onde deseja armazenar o repositório e digite:
```bash
git clone https://github.com/o-url-que-voce-copiou.git
```
   ![Clonar Repositório](https://i.imgur.com/c5VOaM2.png)

🎉 **Pronto! Seu repositório está configurado!**

---

# 🔨 Criando um Repositório sem Clonar

### 🔧 Passos:
1️⃣ Crie um repositório no GitHub.
2️⃣ No terminal, vá até a pasta que deseja transformar em repositório e digite:
```bash
git init
```
3️⃣ Altere a branch principal para `main`:
```bash
git branch -M main
```
4️⃣ Adicione os arquivos:
```bash
git add .
```
5️⃣ Faça um commit:
```bash
git commit -m "curta descrição do que foi feito"
```
6️⃣ Adicione o repositório remoto:
```bash
git remote add origin https://github.com/seu-repositorio.git
```
7️⃣ Envie os arquivos para o GitHub:
```bash
git push -u origin main
```

---

# 🌿 Gerenciando Branches

### 📌 O que é uma branch?
Branch é um ramo do código, usado para desenvolver funcionalidades sem afetar o código principal.

### 🔀 Comandos essenciais:
1️⃣ Criar uma nova branch:
```bash
git branch nome-da-branch
```
2️⃣ Mudar para a branch:
```bash
git checkout nome-da-branch
```
3️⃣ Listar branches:
```bash
git branch
```
4️⃣ Excluir uma branch:
```bash
git branch -d nome-da-branch
```
5️⃣ Criar e mudar para uma branch ao mesmo tempo:
```bash
git checkout -b nome-da-branch
```

---

# 🚀 Subindo Modificações para o GitHub

### 📤 Passos:
1️⃣ Adicionar arquivos ao commit:
```bash
git add .
```
2️⃣ Verificar status:
```bash
git status
```
3️⃣ Fazer um commit:
```bash
git commit -m "curta descrição do que foi feito"
```
4️⃣ Enviar para o repositório remoto:
```bash
git push origin nome-da-branch
```

---

# 👥 Trabalhando em Equipe

### 📌 Adicionando colaboradores:
1️⃣ No repositório, vá em **Settings**.
   ![Configurações](https://i.imgur.com/1W6FV3Y.png)

2️⃣ No menu lateral, clique em **Collaborators** e insira sua senha.
   ![Collaborators](https://i.imgur.com/TzS0mMO.png)

3️⃣ Clique em **Add people**.
   ![Adicionar Pessoas](https://i.imgur.com/12gtgyl.png)

4️⃣ Digite o nome de usuário ou e-mail do colaborador.
   ![Nome do Colaborador](https://i.imgur.com/iznSodJ.png)

5️⃣ Clique em **Add (Fulano) to this repository**.
   ![Adicionar](https://i.imgur.com/QeUugQk.png)

🎉 **Agora sua equipe pode colaborar no repositório!** 🚀
