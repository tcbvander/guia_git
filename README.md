# **📚 Guia Completo de Git e GitHub**  

Um guia abrangente com os principais conceitos e comandos do Git e GitHub, baseado no curso "Git do Básico ao Avançado".  

---

## **🔧 Configuração Inicial**  

### **Instalação**  
- **Windows**:  
  ```bash
  # Baixe em: https://git-scm.com/downloads
  ```
- **Linux**:  
  ```bash
  # Instale via gerenciador de pacotes (apt, yum, etc.)
  sudo apt install git
  ```

### **Configuração do Usuário**  
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
git config --list  # Verificar configurações
```

---

## **🚀 Iniciando com Git**  

### **Repositórios**  
- **Criar um repositório local**:  
  ```bash
  git init
  ```
- **Clonar um repositório remoto**:  
  ```bash
  git clone <URL-do-repositório>
  ```

### **GitHub**  
- **Criar um repositório no GitHub**:  
  - Acesse [GitHub](https://github.com) e siga os passos.  
- **Vincular repositório local ao remoto**:  
  ```bash
  git remote add origin <URL-do-repositório>
  ```

---

## **📂 Controle de Versão**  

### **Verificando Alterações**  
```bash
git status          # Verifica arquivos modificados
git log             # Exibe histórico de commits
git log --oneline   # Histórico simplificado
```

### **Adicionando e Commitando**  
```bash
git add <arquivo>    # Adiciona um arquivo específico
git add .            # Adiciona todos os arquivos
git commit -m "Mensagem descritiva"  # Cria um commit
```

### **Enviando para o Repositório Remoto**  
```bash
git push -u origin main   # Primeiro push
git push                  # Pushs subsequentes
```

### **Recebendo Atualizações**  
```bash
git pull origin main   # Atualiza o repositório local
```

---

## **🌿 Branches (Ramificações)**  

### **Criando e Gerenciando Branches**  
```bash
git branch                  # Lista branches
git branch <nome>           # Cria uma nova branch
git checkout <nome>         # Muda para a branch
git checkout -b <nome>      # Cria e muda para a branch
git merge <branch>          # Mescla uma branch na atual
git branch -d <nome>        # Deleta uma branch local
```

### **Stash (Armazenamento Temporário)**  
```bash
git stash           # Armazena alterações temporariamente
git stash list      # Lista stashes
git stash pop       # Recupera alterações do stash
git stash clear     # Limpa todas as stashes
```

### **Tags (Checkpoints)**  
```bash
git tag -a v1.0 -m "Versão 1.0"  # Cria uma tag
git push origin v1.0              # Envia tag para o remoto
git checkout v1.0                 # Muda para uma tag
```

---

## **🔄 Compartilhamento e Atualização**  

### **Sincronizando com o Remoto**  
```bash
git fetch           # Busca atualizações sem mesclar
git pull            # Busca e mescla atualizações
git push            # Envia alterações para o remoto
```

### **Submódulos (Projetos dentro de Projetos)**  
```bash
git submodule add <URL>   # Adiciona um submódulo
git submodule update      # Atualiza submódulos
```

---

## **🔍 Inspeção e Administração**  

### **Verificando Diferenças**  
```bash
git diff            # Mostra alterações não commitadas
git show <commit>   # Exibe detalhes de um commit
```

### **Limpeza e Otimização**  
```bash
git clean -n        # Mostra arquivos não rastreados (dry run)
git clean -f        # Remove arquivos não rastreados
git gc              # Otimiza o repositório (garbage collector)
```

### **Recuperando Arquivos**  
```bash
git reflog          # Mostra histórico de ações
git reset --hard <hash>  # Volta para um estado específico
```

---

## **📄 GitHub: Abas e Funcionalidades**  

| **Aba**         | **Função**                                                                 |
|-----------------|---------------------------------------------------------------------------|
| **Code**        | Código-fonte, README.md e licença.                                       |
| **Issues**      | Gerenciamento de tarefas e bugs.                                         |
| **Pull Request**| Envio de código para revisão antes de mesclar à branch principal.        |
| **Actions**     | Automação de CI/CD (Integração Contínua/Deploy Contínuo).                |
| **Projects**    | Quadro Kanban para organização de tarefas.                               |
| **Wiki**        | Documentação detalhada do projeto.                                       |
| **Insights**    | Estatísticas do projeto (contribuidores, commits, etc.).                |
| **Settings**    | Configurações do repositório (colaboradores, permissões, etc.).         |

---

## **📝 Markdown (README.md)**  

### **Sintaxe Básica**  
```markdown
# Título (h1)  
## Subtítulo (h2)  

**Negrito** ou __Negrito__  
*Itálico* ou _Itálico_  

- Lista não ordenada  
1. Lista ordenada  

![Imagem](URL)  
[Link](URL)  

`Código inline`  
```bash  
# Bloco de código  
git status  
```  
```

---

## **🚀 GitHub Pages (Hospedagem Grátis)**  

1. Crie um repositório: **`usuario.github.io`**  
2. Adicione arquivos HTML/CSS/JS.  
3. Faça push:  
   ```bash
   git push origin main
   ```
4. Acesse: **`https://usuario.github.io`**  

---

## **💡 Boas Práticas**  

### **Commits Organizados**  
- **Assunto**: Máximo 50 caracteres, comece com maiúscula.  
- **Corpo**: Explique o "porquê" e o "como" (máximo 72 caracteres por linha).  

Exemplo:  
```bash
git commit -m "Corrige bug de login" -m "O botão de login não respondia devido a um erro no evento de clique."
```

### **Branches Eficientes**  
- Use **`feature/nome-da-funcionalidade`** para novas funcionalidades.  
- Use **`fix/nome-do-bug`** para correções.  

---

## **📚 Recursos Adicionais**  
- **Documentação Oficial**: [git-scm.com](https://git-scm.com/doc)  
- **GitHub Learning Lab**: [lab.github.com](https://lab.github.com)  


