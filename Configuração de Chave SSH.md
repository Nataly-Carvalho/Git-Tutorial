# Tutorial: Configuração de Chave SSH e Upload de Arquivos para o GitHub

## 1. Verificar se já existe uma chave SSH no computador

### Passo 1: Acessar o diretório das chaves SSH
```bash
cd ~/.ssh
```
Este comando navega até o diretório onde as chaves SSH são armazenadas no sistema.

### Passo 2: Listar os arquivos do diretório
```bash
ls
```
Este comando lista todos os arquivos e diretórios dentro do diretório `.ssh`. Se você já tiver uma chave SSH, ela estará listada aqui.

## 2. Criar uma nova chave SSH

### Passo 1: Gerar uma nova chave SSH
```bash
ssh-keygen -t ed25519 -C "exemplo@email.com"
```
- `ssh-keygen`: Inicia o processo de criação de uma nova chave SSH.
- `-t ed25519`: Especifica o tipo de algoritmo de criptografia a ser utilizado (neste caso, ed25519).
- `-C "exemplo@email.com"`: Adiciona um rótulo à chave, geralmente o seu e-mail, para identificação.

## 3. Obter a chave pública

### Passo 1: Visualizar a chave pública
```bash
cat ~/.ssh/id_ed25519.pub
```
Este comando exibe o conteúdo da chave pública recém-criada. A chave pública é usada para autenticação com serviços como GitHub.

## 4. Adicionar a chave pública no GitHub

### Passo 1: Adicionar a chave no GitHub
1. Acesse [GitHub](https://github.com) e faça login.
2. Vá para **Settings** (Configurações).
3. Selecione **SSH and GPG keys**.
4. Clique em **New SSH key** (Nova chave SSH).
5. Adicione um nome para identificar a chave.
6. Cole a chave pública obtida anteriormente e clique em **Add SSH key**.

## 5. Clonar um repositório e subir um arquivo para o GitHub

### Passo 1: Navegar para o diretório inicial
```bash
cd
```

### Passo 2: Clonar o repositório
```bash
git clone git@github.com:exemplo/Softex-Ruby.git
```
Este comando clona o repositório especificado para o seu computador local.

### Passo 3: Navegar para o diretório do projeto
```bash
cd Softex-Ruby/
cd Calculadora-Ruby/
```
Esses comandos navegam para o diretório do projeto clonado.

### Passo 4: Inicializar o repositório Git
```bash
git init
```
Este comando inicializa um novo repositório Git no diretório atual.

### Passo 5: Verificar os repositórios remotos
```bash
git remote -v
```
Este comando lista os repositórios remotos associados ao projeto.

### Passo 6: Adicionar o repositório remoto de origem
```bash
git remote add origin git@github.com:exemplo/LP-Calculadora.git
```
Este comando adiciona um repositório remoto chamado `origin` ao projeto local, apontando para o repositório especificado.

### Passo 7: Verificar os repositórios remotos novamente
```bash
git remote -v
```
Este comando verifica se o repositório remoto foi adicionado corretamente.

### Passo 8: Criar uma nova branch
```bash
git checkout -b exemplo-branch
```
Este comando cria uma nova branch chamada `exemplo-branch` e troca para ela.

### Passo 9: Adicionar arquivos ao repositório
```bash
git add .
```
Este comando adiciona todos os arquivos modificados no diretório atual ao próximo commit.

### Passo 10: Fazer o commit das alterações
```bash
git commit -m "Adicionando a calculadora"
```
Este comando cria um commit com a mensagem "Adicionando a calculadora", que descreve as alterações feitas.

### Passo 11: Enviar as alterações para o repositório remoto
```bash
git push origin exemplo-branch
```
Este comando envia as alterações na branch `exemplo-branch` para o repositório remoto no GitHub.

---

Certifique-se de substituir as informações de exemplo, como e-mail e URLs de repositório, com os seus dados específicos.
