![Banner Git Cheat](https://imgur.com/BPAoakW.png)
# 🚨 Git Emergency Cheatsheet

## 📌 Corrigindo Commits

### Modificar último commit (mensagem ou arquivos)
```sh
# Modifica o último commit sem alterar o histórico remoto
git commit --amend
```
⚠️ Se já tiver enviado (`push`), use `git push --force` com cuidado.

---

## 🔄 Recuperação de Commits

### Resetar commit localmente (descartando mudanças)
```sh
git reset --hard HEAD~1
```
⚠️ Perde as alterações! Use `git reset --soft` para manter no staging.

### Recuperar commit deletado (caso tenha o hash)
```sh
git reflog
# Pegue o hash do commit perdido

git checkout <commit_hash>
git branch recovery-branch  # Opcional, para preservar
```

### Trazer commit de outra branch
```sh
git cherry-pick <commit_hash>
```
⚠️ Se houver conflitos, resolva e finalize com:
```sh
git cherry-pick --continue
```

---

## 🏥 Resolvendo Problemas com Branches

### Desfazer `git pull` que deu ruim
```sh
git reset --hard ORIG_HEAD
```

### Substituir branch remota com a versão local (forçar push)
```sh
git push --force
```
⚠️ Cuidado! Isso sobrescreve a branch remota.

### Trazer apenas uma branch sem afetar outras
```sh
git fetch origin <branch>
```

### Deletar branch localmente e remotamente
```sh
git branch -D <branch>
git push origin --delete <branch>
```

### Restaurar uma branch deletada
```sh
git reflog
# Pegue o hash do último commit da branch

git checkout -b <branch> <commit_hash>
```

---

## 🚀 Outras Situações de Emergência

### Stash: salvar alterações temporariamente
```sh
git stash
```
### Recuperar mudanças stashed
```sh
git stash pop
```

### Reverter commit sem removê-lo do histórico
```sh
git revert <commit_hash>
```

### Reaplicar commits de outra branch sem merge completo
```sh
git rebase <branch>
```
⚠️ Se der conflito, resolva e continue com:
```sh
git rebase --continue
```

### Reverter um `merge`
```sh
git revert -m 1 <merge_commit_hash>
```

### Recuperar arquivos deletados antes de um commit
```sh
git checkout HEAD~1 -- <caminho/do/arquivo>
```

### Recuperar arquivos deletados após um commit
```sh
git checkout <commit_hash> -- <caminho/do/arquivo>
```

### Desfazer alterações em um único arquivo
```sh
git checkout -- <arquivo>
```

### Resolver conflitos automaticamente aceitando a versão local
```sh
git checkout --ours <arquivo>
```
### Resolver conflitos automaticamente aceitando a versão remota
```sh
git checkout --theirs <arquivo>
```

---

💡 **Dica:** Sempre faça backup antes de comandos destrutivos! 😉
