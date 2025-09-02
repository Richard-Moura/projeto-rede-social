
# REDEMIN — Hub de Redes Sociais dentro de um “celular”

Projeto estático que simula um smartphone no centro da tela e, dentro dele, carrega telas de redes sociais via `iframe`. Cada tela exibe uma imagem estática e um botão **ACESSE** com o link real da rede.

> **Status:** pronto para uso • **Stack:** HTML + CSS (sem JavaScript) • **Autor:** Richard Dean

---

## ✨ Funcionalidades
- Smartphone central com moldura de iPhone.
- Navegação por ícones das redes (à direita) que trocam a página exibida no `iframe`.
- Cada página de rede possui botão **ACESSE** para abrir o perfil real em nova aba.
- Layout responsivo simples e visual limpo.

---

## 🗂️ Estrutura de pastas
```
REDEMIN/
│── index.html
│── home.html
│── facebook.html
│── github.html
│── instagram.html
│── youtube.html
│
├── estilos/
│   ├── style.css        # layout principal (smartphone, fundo, ícones)
│   └── social.css       # estilo das páginas internas (rede + botão ACESSE)
│
└── imagens/             # coloque aqui suas imagens
    ├── fundo-madeira.jpg
    ├── frame-iphone.png
    ├── tela-home.jpg
    ├── tela-facebook.jpg
    ├── tela-github.jpg
    ├── tela-instagram.jpg
    ├── tela-youtube.jpg
    ├── logo-home.jpg
    ├── logo-facebook.jpg
    ├── logo-github.jpg
    ├── logo-instagram.jpg
    └── logo-youtube.jpg
```

> ⚠️ **Importante:** este repositório não inclui as imagens por padrão. Crie a pasta `imagens/` e adicione os arquivos com os nomes acima.

---

## 🚀 Como executar localmente
1. Baixe/clone o projeto.
2. Crie a pasta `imagens/` e adicione as imagens citadas.
3. Abra o arquivo `index.html` no seu navegador (duplo clique).

---

## 🛠️ Personalização rápida
### Trocar links das redes
Edite cada arquivo da rede (`facebook.html`, `instagram.html`, etc.) e altere o `href` do botão **ACESSE**.

### Adicionar uma nova rede
1. Duplique um arquivo de rede (ex.: `instagram.html`) e renomeie (ex.: `tiktok.html`).
2. Troque o `<title>`, `src` da imagem e o link do **ACESSE**.
3. No `index.html`, adicione um novo ícone na seção `#redes-sociais` apontando `target="tela"` para o novo arquivo:
```html
<a href="tiktok.html" target="tela">
  <img src="imagens/logo-tiktok.jpg" alt="Logo TikTok">
</a>
```

### Acessibilidade
- Use `alt` descritivos nas imagens (ex.: `alt="Tela inicial do Instagram"`).
- Garanta contraste adequado do botão **ACESSE** (já há `:hover` em `social.css`).

---

## 🌐 Publicando no GitHub Pages
1. Faça um repositório no GitHub (ex.: `redemin`).
2. Faça push do projeto (exemplo de comandos abaixo).
3. No GitHub: **Settings → Pages → Branch: `main` /root → Save**.
4. Após alguns minutos, o site ficará disponível em:
```
https://Richard-Moura.github.io/projeto-rede-social
```

---

## ⬆️ Enviando para o GitHub (via Git)
> Execute estes comandos dentro da pasta do projeto:

```bash
git init
git add .
git commit -m "Primeiro commit: REDEMIN"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/redemin.git
git push -u origin main
```

> Depois ative o GitHub Pages conforme descrito acima.

---

## 📄 Arquivos principais

- **index.html**  
  Contém a moldura do celular (`section#telefone`) e o `iframe` (`#tela`), além do menu de ícones à direita.

- **home.html**  
  Tela inicial (papel de parede) que abre por padrão no `iframe`.

- **facebook.html / github.html / instagram.html / youtube.html**  
  Cada um exibe uma imagem de “tela” + botão **ACESSE**.

- **estilos/style.css**  
  Layout geral: fundo de madeira, posição e tamanho da moldura do celular, área do `iframe`, ícones laterais, efeitos de hover, etc.

- **estilos/social.css**  
  Estilo das páginas internas (largura da imagem para caber na tela, botão **ACESSE** e `:hover`).

---

## ✅ Checklist de qualidade
- [x] `<title>` correto em cada página de rede.
- [x] `alt` descritivo nas imagens.
- [x] Links **ACESSE** abrindo em nova aba (`target="_blank"`).
- [x] Layout funciona em telas comuns de desktop e mobile.

---

## 📜 Licença
Uso pessoal e educacional. Ajuste para suas necessidades e inclua créditos(cursoemvideo) das imagens/icons conforme aplicável.

---


