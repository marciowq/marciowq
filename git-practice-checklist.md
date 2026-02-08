# 📝 Checklist de Prática: Git & GitHub

Este guia foi criado para ajudar você a dominar os comandos essenciais e fluxos de trabalho. Marque as caixas conforme concluir as tarefas.

## 1. Configuração Inicial (Setup)
- [x] Instalar o Git no computador.
- [x] Configurar nome de usuário: `git config --global user.name "Seu Nome"`
- [x] Configurar e-mail: `git config --global user.email "seu@email.com"`
- [x] Configurar a branch padrão como `main`: `git config --global init.defaultBranch main`

## 2. O Básico (Workflow Local)
- [x] Inicializar um repositório em uma pasta nova: `git init`
- [x] Criar um arquivo `README.md`.
- [x] Verificar o status dos arquivos: `git status`
- [x] Adicionar o arquivo à área de preparação (stage): `git add README.md`
- [x] Fazer o primeiro commit: `git commit -m "Initial commit"`
- [x] Visualizar o histórico de commits: `git log`

## 3. Conectando com o GitHub (Remoto)
- [x] Criar um repositório vazio no GitHub (sem selecionar README/gitignore na criação).
- [x] Adicionar a origem remota: `git remote add origin <URL-DO-REPO>`
- [x] Enviar (Push) o código local para o GitHub: `git push -u origin main`

## 4. Trabalhando com Branches (Ramificações)
- [ ] Criar uma nova branch: `git branch feature-nova`
- [ ] Mudar para a nova branch: `git checkout feature-nova` (ou `git switch feature-nova`)
- [ ] Fazer uma alteração no arquivo e commitar na nova branch.
- [ ] Voltar para a `main`: `git checkout main`
- [ ] Mesclar (Merge) a branch nova na main: `git merge feature-nova`
- [ ] Deletar a branch antiga (opcional): `git branch -d feature-nova`

## 5. Simulação de Conflitos (Importante!)
- [ ] Criar uma branch `dev-a` e editar a **linha 1** de um arquivo. Commitar.
- [ ] Voltar para `main`, criar branch `dev-b` e editar a **MESMA linha 1** com texto diferente. Commitar.
- [ ] Tentar fazer merge de `dev-a` em `main` (Funcionará).
- [ ] Tentar fazer merge de `dev-b` em `main` (Gerará conflito).
- [ ] Resolver o conflito manualmente no editor de código (escolher qual código fica).
- [ ] Finalizar o merge: `git add .` e `git commit`.

## 6. Avançado / Utilitários
- [ ] Criar um arquivo `.gitignore` e adicionar arquivos que não devem subir (ex: `*.log`).
- [ ] Usar `git stash` para guardar mudanças temporárias sem commitar.
- [ ] Recuperar mudanças do stash: `git stash pop`
- [ ] Criar uma Tag de versão: `git tag v1.0.0`
- [ ] Enviar tags para o GitHub: `git push origin --tags`

---
> **Dica:** Use `git status` frequentemente para saber onde você está!