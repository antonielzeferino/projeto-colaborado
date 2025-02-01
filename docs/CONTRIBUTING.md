# Contribuindo para o Projeto

Obrigado por querer contribuir para este projeto! Para garantir um fluxo de trabalho organizado e evitar conflitos, siga as diretrizes abaixo.

## 🚀 Fluxo de Trabalho no GitHub

### 1. Organização do Repositório
- **`main`**: Branch principal, somente código testado e aprovado entra aqui.
- **`dev`**: Branch de desenvolvimento, onde todas as mudanças são integradas antes de irem para a `main`.
- **Branches de feature**: Cada funcionalidade deve ser desenvolvida em uma branch separada, seguindo o padrão `feature/nome-da-feature`.

### 2. Como Trabalhar Sem Conflitos

#### 1️⃣ Antes de começar qualquer coisa
Sempre **atualize seu código** antes de fazer mudanças:
```bash
# Vá para a branch dev
git checkout dev
# Pegue as últimas alterações do repositório
git pull origin dev
```

Crie uma branch para sua feature:
```bash
git checkout -b feature/nome-da-feature
```

#### 2️⃣ Durante o desenvolvimento
- **Nunca altere diretamente a `main` ou `dev`!**
- Faça commits pequenos e descritivos:
```bash
git add .
git commit -m "Adiciona seção de serviços"
```
- Envie sua branch para o repositório:
```bash
git push origin feature/nome-da-feature
```

#### 3️⃣ Antes de enviar seu código para `dev`
Sempre atualize sua branch antes de criar um **Pull Request**:
```bash
git checkout dev
git pull origin dev
git checkout feature/nome-da-feature
git merge dev
```

Se houver conflitos, resolva-os antes de enviar o **Pull Request (PR)**.

### 3. Como Criar um Pull Request (PR)
1. No GitHub, vá para a aba **Pull Requests** e clique em **New Pull Request**.
2. Escolha `feature/nome-da-feature` → `dev`.
3. Adicione uma descrição clara do que foi alterado.
4. Aguarde a revisão antes do merge.

---

## 📌 Regras de Desenvolvimento

### 🌎 HTML
✅ Estruture o código de forma semântica.  
✅ Use indentação consistente.  
✅ Nomeie classes e IDs de forma descritiva.

### 🎨 CSS
✅ Use **CSS modularizado** (arquivos separados, se necessário).  
✅ Utilize **variáveis CSS** para cores e estilos repetitivos.  
✅ Prefira Flexbox ou Grid para layout.

### ⚡ JavaScript
✅ Utilize **event listeners** ao invés de `onclick` no HTML.  
✅ Mantenha o código modular e reutilizável.  
✅ Evite funções muito grandes – prefira dividir em funções menores.

---

## ❌ O Que NÃO Fazer
🚫 **Não edite arquivos diretamente na `main` ou `dev`**.  
🚫 **Não faça commits muito grandes** – commits menores facilitam a revisão.  
🚫 **Não esqueça de dar `git pull` antes de começar** para evitar conflitos.  