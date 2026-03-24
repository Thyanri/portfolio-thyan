# Portfólio - Guia de Deploy

## O que foi criado

3 arquivos na raiz do repositório:

```
portfolio-thyan/
├── index.html
├── estilo.css
└── script.js
```

---

## Passo a passo pelo VSCode

### 1. Clonar o repositório

Abra o terminal no VSCode (`Ctrl + '`) e rode:

```bash
git clone https://github.com/Thyanri/portfolio-thyan.git
cd portfolio-thyan
```

---

### 2. Fazer suas alterações

Edite o `index.html` e personalize:

- **Linha com `Rithyan Goncalves`** → coloque seu nome completo
- **Seção `#sobre`** → edite o texto de apresentação
- **Tags de skills** → adicione ou remova tecnologias que você conhece
- **Seção `#formacao`** → atualize com sua escola/curso real
- **Seção `#portfolio`** → troque pelos seus projetos reais do GitHub

---

### 3. Commitar e enviar

Depois de editar, no terminal do VSCode:

```bash
git add .
git commit -m "Personalizando portfólio"
git push origin main
```

Ou use a aba **Source Control** do VSCode (ícone de ramificação na barra lateral):
1. Clique em `+` nos arquivos alterados para fazer stage
2. Escreva a mensagem do commit
3. Clique em **Commit** e depois **Sync Changes**

---

### 4. Ativar o GitHub Pages

1. Acesse o repositório em **github.com/Thyanri/portfolio-thyan**
2. Clique em **Settings** (aba no topo)
3. No menu lateral, clique em **Pages**
4. Em **Source** selecione:
   - Branch: `main`
   - Pasta: `/ (root)`
5. Clique em **Save**

Aguarde ~2 minutos e o site estará em:

```
https://thyanri.github.io/portfolio-thyan/
```

---

## Funcionalidades do site

| Recurso | Descrição |
|---|---|
| Tema claro/escuro | Botão ☀/☾ no canto do menu, salva preferência |
| Menu mobile | Botão ≡ em telas pequenas |
| Formulário de contato | Valida campos e exibe mensagem de sucesso |
| Scroll suave | Links do menu rolam até a seção |

---

## Dicas para personalizar

**Mudar a cor de destaque** (amarelo → outra cor):

No `estilo.css`, procure `--accent: #e2b714` e troque pelo hex da cor desejada. Aparece em 2 lugares (tema dark e light).

**Adicionar novo projeto:**

Copie o bloco `.project-card` no `index.html` e troque nome, descrição e link do repo.

**Adicionar nova skill:**

```html
<span class="tag">nome-da-skill</span>
```
