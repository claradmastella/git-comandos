### `git config`
Um dos comandos git mais usados é o **"git config"** que pode ser usado para definir valores de configuração específicos do usuário como e-mail, algoritmo preferido para diff, nome de usuário e formato de arquivo etc.
   Por exemplo, o seguinte comando pode ser usado para definir o email: 
   `git config --global user.email exemplo@google.com `

### `git clone`
O comando git clone é usado para fins de verificação de repositório. Se o repositório estiver em um servidor remoto, use: 
   `git clone alex@93.188.160.58:/path/to/repository`

Por outro lado, se uma cópia de trabalho de um repositório local for criada, use: 
   `git clone /path/to/repository`

### `git init`
criar novo repositório 

### `git status`
Verificar estado dos arquivos/diretórios

---
 
### Adicionar arquivo/diretório (staged area) 

Adicionar um arquivo em específico:
   `git add meu_arquivo.txt`

Adicionar um diretório em específico 
   `git add meu_diretorio`

Adicionar todos os arquivos/diretórios 
   `git add .`

Adicionar um arquivo que esta listado no .gitignore (geral ou do repositório) 
   `git add -f arquivo_no_gitignore.txt`

O comando **"git add"** pode ser usado para adicionar arquivos ao índice. Por exemplo, o seguinte comando irá adicionar um arquivo chamado temp.txt presente no diretório local para o índice: 
   `git add temp.txt`

---

### Commitar arquivo/diretório 

Commitar um arquivo 
   `git commit meu_arquivo.txt`

Commitar vários arquivos 
   `git commit meu_arquivo.txt meu_outro_arquivo.txt`

Comitar informando mensagem 
   `git commit meuarquivo.txt -m "minha mensagem de commit"`

O comando **"git commit"** é usado para confirmar as alterações na cabeça. Tenha em atenção que quaisquer alterações efetuadas não irão para o repositório remoto. Uso: 
   `git commit –m “coloque sua mensagem aqui”`

O comando **"git status"** exibe a lista de arquivos alterados juntamente com os arquivos que ainda não foram adicionados ou confirmados. Uso: 
    `git status`

**"git push"** é outro dos comandos git básicos mais usados. Um simples envio envia as alterações feitas para o ramo mestre do repositório remoto associado ao diretório de trabalho. Por exemplo:
   `git push origin master`

--- 

O comando **"git remote"** permite que um usuário se conecte a um repositório remoto. O comando a seguir lista os repositórios remotos atualmente configurados: 

### `git remote –v`
   Esse comando permite que o usuário se conecte a um servidor remoto:
   `git remote add origin <93.188.160.58>``

---

### Branches

O comando **"git checkout"** pode ser usado para criar ramos ou alternar entre eles. Por exemplo, o seguinte cria um novo ramo e muda para ele:
   `command git checkout -b <branch-name>`

Para simplesmente mudar de um ramo para outro, use:
   `git checkout <branch-name>`

### `git branch`
   Mostra todas as branches existentes no repositório

Para excluir um ramo:
   `git branch –d <branch-name>`

---

Para mesclar todas as alterações presentes no repositório remoto para o diretório de trabalho local, o comando pull é usado. Uso:
   `git pull`

O comando **"git merge"** é usado para mesclar uma ramificação no ramo ativo. Uso:
   `git merge <branch-name>`

O comando **"git diff"*** é usado para listar os conflitos. Para visualizar conflitos com o arquivo base, use:
   `git diff --base <file-name>`

O seguinte comando é usado para exibir os conflitos entre ramos about-to-be-merged antes de mesclá-los:
   `git diff <source-branch> <target-branch>`

Para simplesmente listar todos os conflitos atuais, use: 
   `git diff`



