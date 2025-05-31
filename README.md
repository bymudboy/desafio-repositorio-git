# 🧠 Git e GitHub: O Guia Prático do Dia a Dia de um Dev

## 🚀 O que é Git?

Git é um **sistema de controle de versão distribuído**. Ele permite que desenvolvedores acompanhem todas as mudanças feitas no código, colaborem em equipe e revertam alterações quando necessário.

## ☁️ O que é GitHub?

GitHub é uma **plataforma na nuvem que hospeda repositórios Git**. Ele facilita o trabalho colaborativo, permitindo compartilhar projetos, abrir issues, fazer pull requests e até contribuir com projetos open source.

---

## 🛠️ Principais Comandos Git no Dia a Dia

### 🔸 Configuração inicial (feito uma vez)
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### 🔸 Clonar um repositório existente
```bash
git clone https://github.com/usuario/repositorio.git
```

### 🔸 Verificar o status dos arquivos
```bash
git status
```

### 🔸 Adicionar arquivos para serem commitados
```bash
git add .
# ou adicionar um arquivo específico
git add nome-do-arquivo
```

### 🔸 Salvar mudanças (commit)
```bash
git commit -m "Mensagem clara sobre o que foi alterado"
```

### 🔸 Enviar as alterações para o GitHub (push)
```bash
git push
```

### 🔸 Puxar alterações do repositório remoto (pull)
```bash
git pull
```

### 🔸 Criar uma nova branch
```bash
git checkout -b nome-da-branch
```

### 🔸 Trocar de branch
```bash
git checkout nome-da-branch
```

### 🔸 Mesclar branch (merge)
```bash
git checkout main
git merge nome-da-branch
```

---

## 🔄 Fluxo de Trabalho Mais Usado

1. Atualizar seu repositório local
```bash
git pull
```

2. Criar uma branch para sua tarefa
```bash
git checkout -b minha-feature
```

3. Fazer mudanças no código

4. Adicionar mudanças
```bash
git add .
```

5. Salvar (commit) com mensagem
```bash
git commit -m "Descrição clara da alteração"
```

6. Enviar para o GitHub
```bash
git push -u origin minha-feature
```

7. No GitHub → Abrir um **Pull Request (PR)** para revisão e merge

8. Após aprovação → Merge na branch principal (`main` ou `master`)

---

## 🤝 GitHub na Prática

- **Pull Request (PR)** → Proposta de alteração no código
- **Issues** → Relatar problemas, bugs ou sugerir melhorias
- **Fork + Pull Request** → Contribuir com projetos de terceiros
- **Actions** → Automatizar processos (CI/CD)

---

## 🐛 Erros Mais Comuns no Git e GitHub e Como Corrigir

Um dos erros mais comuns é fazer commit na branch errada, como na main, sem querer. Para resolver, você pode criar uma nova branch com `git checkout -b nome-da-branch` e depois fazer `git push origin nome-da-branch`. Assim seus commits ficam na branch certa e você evita bagunçar a main.

Outro erro bem comum é esquecer de adicionar arquivos antes do commit. Se isso acontecer, é só usar `git add nome-do-arquivo` e depois fazer `git commit -m "mensagem"`. Caso queira incluir no commit anterior, pode usar `git commit --amend` para corrigir rapidamente sem criar outro commit separado.

Por fim, errar na mensagem do commit também acontece bastante. Dá pra corrigir facilmente com `git commit --amend -m "mensagem nova"`. Se já tiver enviado pro GitHub, será necessário forçar o push com `git push origin sua-branch --force` pra atualizar o commit no repositório remoto.


## 🎯 Boas Práticas com Git e GitHub

- ✅ Commits pequenos e frequentes
- ✅ Mensagens de commit claras e objetivas
- ✅ Usar branches descritivas:
  - `feature/login-page`
  - `fix/navbar-error`
  - `hotfix/bug-critical`
- 🚫 Nunca trabalhar diretamente na branch `main` ou `master`
- 🔄 Sempre sincronizar (`git pull`) antes de começar a trabalhar

---

## 🚀 Conclusão

Dominar Git e GitHub não é só requisito básico: é **essencial para qualquer desenvolvedor**. Eles garantem segurança, organização e possibilitam trabalho colaborativo de forma eficiente. Com esses conhecimentos, você está preparado para trabalhar em qualquer projeto, seja pessoal, em equipe ou open source.

---
