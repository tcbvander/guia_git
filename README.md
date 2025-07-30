# **📚 Guia de Referência Git**  

Um guia rápido com os comandos fundamentais do Git para versionamento de código.  

---

## **🔧 Configuração Inicial**  
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
git config --list  # Verificar configurações
```

---

## **🚀 Iniciar um Repositório**  
```bash
git init          # Iniciar um repositório local
git clone <URL>   # Clonar um repositório remoto
```

---

## **📂 Verificar Status e Histórico**  
```bash
git status                 # Verificar arquivos modificados
git log                    # Histórico de commits
git log --oneline          # Histórico simplificado
```

---

## **💾 Adicionar e Confirmar Alterações**  
```bash
git add <arquivo>          # Adicionar arquivo específico
git add .                  # Adicionar todos os arquivos
git commit -m "Mensagem"   # Confirmar alterações
git commit -am "Mensagem"  # Adicionar e commit (arquivos rastreados)
```

---

## **🌿 Branches (Ramificações)**  
```bash
git branch                  # Listar branches
git branch <nome>           # Criar nova branch
git checkout <nome>         # Mudar de branch
git checkout -b <nome>      # Criar e mudar para branch
git merge <branch>          # Mesclar branch atual
git branch -d <nome>        # Excluir branch local
```

---

## **🌐 Repositórios Remotos (GitHub/GitLab)**  
```bash
git remote add origin <URL>   # Vincular repositório remoto
git push -u origin <branch>  # Enviar commits (1ª vez)
git push                     # Enviar commits (após 1ª vez)
git pull origin <branch>     # Baixar atualizações
git remote -v                # Listar repositórios remotos
```

---

## **⏪ Desfazendo Alterações**  
```bash
git restore <arquivo>        # Descartar mudanças (não staged)
git restore --staged <arquivo>  # Remover do staging
git commit --amend -m "Nova mensagem"  # Corrigir último commit
git revert <hash-do-commit>  # Reverter um commit
```

---

## **🔍 Outros Comandos Úteis**  
```bash
git diff            # Ver diferenças não commitadas
git stash           # Guardar alterações temporariamente
git stash pop       # Recuperar alterações do stash
```

---

### **💡 Dica:** Use `git status` para verificar o estado atual do repositório!  

📖 **Documentação oficial:** [git-scm.com](https://git-scm.com/doc)  

---

