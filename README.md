# DPE-MT — Cabeçalhos para Metabase

Cabeçalhos HTML institucionais da **Defensoria Pública do Estado de Mato Grosso**, prontos para uso em dashboards do Metabase via "Custom Header HTML".

---

## 📁 Estrutura do Projeto

```
dpe-mt-headers/
├── assets/
│   ├── logo-fundo-branco.jpeg   # Logo versão fundo branco (uso interno)
│   └── logo-fundo-cinza.jpeg    # Logo versão fundo cinza (uso externo)
├── css/
│   └── tokens.css               # Variáveis de design compartilhadas (cores, fontes, espaçamentos)
├── headers/
│   ├── cabecalho-01-gradiente.html   # Gradiente horizontal verde (padrão)
│   ├── cabecalho-02-escuro.html      # Fundo escuro sólido com detalhe geométrico
│   ├── cabecalho-03-branco.html      # Fundo branco institucional clean
│   └── cabecalho-04-split.html      # Layout bicolor dividido com logo centralizada
└── README.md
```

---

## 🎨 Variantes de Cabeçalho

| Arquivo | Estilo | Indicado para |
|---|---|---|
| `cabecalho-01-gradiente.html` | Gradiente verde horizontal | Dashboard principal / geral |
| `cabecalho-02-escuro.html` | Verde escuro sólido | Painéis executivos / gestão |
| `cabecalho-03-branco.html` | Fundo branco com borda verde | Relatórios formais / impressão |
| `cabecalho-04-split.html` | Split bicolor verde + branco | Apresentações / painel público |

---

## ⚙️ Como usar no Metabase

1. Acesse **Admin → Configurações → Personalização**
2. Em **HTML do cabeçalho personalizado**, cole o conteúdo do arquivo desejado
3. Ajuste o texto de título/subtítulo conforme o dashboard
4. Certifique-se de que os assets (logo) estão hospedados em URL pública (ex: GitHub Pages ou CDN)

> **Dica:** Substitua os caminhos relativos `../assets/` pelo URL absoluto onde os arquivos de imagem estão hospedados, por exemplo:
> ```html
> src="https://seu-usuario.github.io/dpe-mt-headers/assets/logo-fundo-branco.jpeg"
> ```

---

## 🎨 Design Tokens

Todas as cores e fontes institucionais estão centralizadas em `css/tokens.css`:

```css
--verde-escuro:    #0b4f2f
--verde-principal: #16673c
--verde-claro:     #1f8f55
```

Para ajustar o tema, basta editar esse arquivo — todos os cabeçalhos serão atualizados automaticamente.

---

## 📌 Fontes utilizadas

- **Sora** — títulos e destaque (Google Fonts)
- **Source Sans 3** — corpo e subtítulos (Google Fonts)

> As fontes são carregadas via CDN do Google Fonts. Em ambiente sem internet, substitua por fontes do sistema (`system-ui, sans-serif`).

---

*Defensoria Pública do Estado de Mato Grosso — Coordenadoria de TI*
