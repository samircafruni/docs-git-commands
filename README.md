# Comandos e Atributos do Git

## 📌 Comandos Básicos

`git init`
Inicializa um novo repositório Git no diretório atual.

`git clone <url>`
Clona um repositório remoto para o seu computador.

`git status`
Exibe o estado atual do repositório, mostrando arquivos modificados, adicionados ou não rastreados.

`git add <arquivo>`
Adiciona um arquivo ao índice (staging area), preparando-o para o commit.

`git add .`
Adiciona **todos** os arquivos modificados e novos ao índice.

`git commit -m "mensagem"`
Salva as alterações no repositório local com uma mensagem descritiva.

`git commit -am "mensagem"`
Adiciona e faz commit de **todos** os arquivos modificados que já estão sendo rastreados.

`git log`
Mostra o histórico de commits do repositório.

`git log --oneline`
Exibe o histórico de commits de forma resumida.

`git diff`
Mostra as diferenças entre os arquivos modificados e o último commit.

---

## 🔄 Trabalhando com Branches

`git branch`
Lista todas as branches do repositório.

`git branch <nome>`
Cria uma nova branch.

`git checkout <branch>`
Muda para a branch especificada.

`git checkout -b <branch>`
Cria e muda para uma nova branch ao mesmo tempo.

`git merge <branch>`
Faz merge da branch especificada na branch atual.

`git rebase <branch>`
Aplica os commits da branch especificada sobre a branch atual.

`git branch -d <branch>`
Deleta uma branch local.

`git push origin --delete <branch>`
Deleta uma branch remota.

---

## 🌎 Trabalhando com Repositórios Remotos

`git remote -v`
Lista os repositórios remotos configurados.

`git remote add origin <url>`
Adiciona um repositório remoto.

`git push origin <branch>`
Envia commits da branch local para o repositório remoto.

`git pull origin <branch>`
Baixa as alterações do repositório remoto para a branch local.

`git fetch`
Baixa as atualizações do repositório remoto sem aplicá-las.

`git push --force`
Força a atualização do repositório remoto, sobrescrevendo alterações (⚠️ **Cuidado!**).

---

## 🔄 Revertendo Alterações

`git reset --soft <commit>`
Desfaz commits, mantendo as alterações no staging.

`git reset --mixed <commit>`
Desfaz commits e remove arquivos do staging, mas mantém as alterações no diretório de trabalho.

`git reset --hard <commit>`
Desfaz commits e remove completamente as alterações (⚠️ **Cuidado!**).

`git revert <commit>`
Cria um commit que desfaz as alterações de um commit específico.

`git stash`
Salva temporariamente as alterações pendentes sem fazer um commit.

`git stash pop`
Aplica as alterações salvas no último `stash` e remove da pilha de stashes.

---

## 🎭 Tags

`git tag`
Lista todas as tags.

`git tag <nome>`
Cria uma nova tag.

`git tag -a <nome> -m "mensagem"`
Cria uma tag anotada com uma mensagem.

`git push origin <tag>`
Envia a tag para o repositório remoto.

`git push origin --tags`
Envia todas as tags locais para o repositório remoto.

---

## ⚙️ Configurações e Informações

`git config --global user.name "Seu Nome"`
Define o nome de usuário globalmente.

`git config --global user.email "seu@email.com"`
Define o e-mail do usuário globalmente.

`git config --list`
Exibe todas as configurações do Git.

`git config --global alias.<atalho> "<comando>"`
Cria um atalho para um comando Git.

---

## 📌 Outros Comandos Úteis

`git blame <arquivo>`
Mostra quem editou cada linha de um arquivo.

`git show <commit>`
Exibe detalhes sobre um commit específico.

`git shortlog`
Exibe um resumo do histórico de commits, agrupado por autor.

`git cherry-pick <commit>`
Aplica um commit específico de outra branch na branch atual.

`git reflog`
Mostra um histórico de ações realizadas no repositório.

---

## 🔍 Atributos do Git

`.gitignore`
Define arquivos e diretórios que devem ser ignorados pelo Git.

`.gitattributes`
Permite configurar regras para arquivos, como normalização de fim de linha.

`.gitkeep`
Arquivo vazio usado para manter diretórios vazios no repositório.

---

Essa lista cobre os comandos e atributos mais utilizados no **Git**. 🚀
