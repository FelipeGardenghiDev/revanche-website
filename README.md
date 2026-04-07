<div align="center">

# 🎸 REVANCHE — Site Oficial

**Tributo visceral ao emo dos anos 2000 e à Fresno.**

[![Site](https://img.shields.io/badge/🌐_Site-bandarevanche.com.br-AB2217?style=for-the-badge)](https://bandarevanche.com.br)
[![GitHub Pages](https://img.shields.io/badge/Hospedado_em-GitHub_Pages-181717?style=for-the-badge&logo=github)](https://pages.github.com/)
[![License](https://img.shields.io/badge/Licença-MIT-D9CDB5?style=for-the-badge)](LICENSE)

</div>

---

## 📖 Sobre o Projeto

Site oficial da **Revanche**, banda de tributo ao universo emo dos anos 2000 com foco na Fresno. O site apresenta a banda, divulga a agenda de shows, exibe galerias de fotos dos membros e centraliza os canais de contato e imprensa.

Desenvolvido com tecnologias puramente front-end para funcionar perfeitamente no **GitHub Pages**, sem necessidade de back-end ou banco de dados.

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Finalidade |
|---|---|
| **HTML5** | Estrutura semântica das páginas |
| **Tailwind CSS** (via CDN) | Estilização utilitária e responsividade |
| **JavaScript (Vanilla)** | Interatividade: menu mobile, lightbox, carrossel, agenda |
| **Font Awesome 6** | Ícones |
| **Google Fonts — Montserrat** | Tipografia oficial da banda |
| **GitHub Gist** | Fonte de dados dinâmica para a agenda de shows |
| **Google Analytics 4** | Monitoramento de tráfego e comportamento |

---

## ✨ Funcionalidades

- 🎨 **Parallax background** com foto da banda em todas as páginas
- 📱 **Totalmente responsivo** — menu hamburguer, grid adaptativo, carrossel mobile
- 🔍 **SEO completo** — meta tags, Open Graph (WhatsApp/Facebook) e Twitter Card
- ♿ **Acessível** — navegação por teclado, `aria-label`, `aria-expanded`, `focus-visible`
- 🖼️ **Lightbox** nas galerias de fotos dos membros (mouse e teclado)
- 📅 **Agenda dinâmica** via GitHub Gist — sem precisar mexer no código para atualizar shows
- 🎵 **Embed do Spotify** com a playlist oficial
- 🤝 **Carrossel de parceiros** com suporte a drag/swipe no mobile
- ⚡ **Lazy loading** em todas as imagens abaixo da dobra
- 🛒 **Loja** (em desenvolvimento)

---

## 📁 Estrutura do Projeto

```
revanche-website/
│
├── index.html              # Página principal
├── felipe.html             # Página do Felipe Gardenghi
├── edu.html                # Página do Eduardo Opaleiro
├── leo.html                # Página do Leonan Artal
├── yago.html               # Página do Yago Borges
├── loja.html               # Loja (em desenvolvimento)
│
└── assets/
    ├── img/
    │   ├── Logo-Revanche-PNG.png
    │   ├── Felipe.jpg
    │   ├── Eduardo.jpg
    │   ├── Leonan.jpg
    │   ├── Yago.jpg
    │   ├── banda/
    │   │   └── banda.jpg           # Foto usada no parallax
    │   ├── felipe/                 # Galeria de fotos (Fe 1-6.JPG)
    │   ├── edu/                    # Galeria de fotos (Edu 1-6.JPG)
    │   ├── leo/                    # Galeria de fotos (Leo 1-6.JPG)
    │   └── yago/                   # Galeria de fotos (Ynhago 1-6.JPG)
    ├── parceiros/                  # Logos dos parceiros
    └── merch/                      # Imagens de merchandise
```

---

## 🗓️ Como Atualizar a Agenda de Shows

A agenda é carregada dinamicamente a partir de um **GitHub Gist**, sem precisar alterar o código do site.

**Acesse:** [gist.github.com](https://gist.github.com) → busque pelo arquivo `shows.json`

### Formato do JSON:

```json
[
  {
    "data": "30 AGO 2026",
    "local": "Toca do Jack",
    "cidade": "Ribeirão Preto/SP",
    "status": "confirmado",
    "ingresso_url": "https://link-para-ingresso.com",
    "ingresso_texto": "COMPRAR INGRESSO"
  },
  {
    "data": "15 SET 2026",
    "local": "Os Pirata",
    "cidade": "São Carlos/SP",
    "status": "em_breve",
    "ingresso_url": "",
    "ingresso_texto": ""
  }
]
```

| Campo | Valores possíveis |
|---|---|
| `status` | `"confirmado"` — exibe link de ingresso \| `"em_breve"` — exibe "INFO EM BREVE" |
| Array vazio `[]` | Exibe mensagem "Em breve mais datas!" |

> ⚠️ **Atenção com o cache:** a URL do Gist utilizada é sempre a versão mais recente (`/raw/shows.json`), com `?nocache=Date.now()` para garantir que o navegador não use versão antiga.

---

## 🖥️ Como Rodar Localmente

Por ser um projeto puramente estático, basta abrir os arquivos em qualquer servidor local:

```bash
# Opção 1: VS Code com extensão Live Server
# Clique com botão direito em index.html → "Open with Live Server"

# Opção 2: Python
python -m http.server 8000

# Opção 3: Node.js (npx)
npx serve .
```

---

## 🎨 Paleta de Cores

| Nome | Hex | Uso |
|---|---|---|
| `rev-primary` | `#AB2217` | Vermelho — cor principal da marca |
| `rev-secondary` | `#D9CDB5` | Off-white vintage — texto e detalhes |
| `rev-black` | `#000000` | Fundo |

---

## 👥 A Banda

| Membro | Instrumento | Página |
|---|---|---|
| Felipe Gardenghi | Vocal / Guitarra | [felipe.html](felipe.html) |
| Eduardo Opaleiro | Guitarra / Voz de Apoio | [edu.html](edu.html) |
| Yago Borges | Baixo / Voz de Apoio | [yago.html](yago.html) |
| Leonan Artal | Bateria | [leo.html](leo.html) |

---

## 🤝 Parceiros

- [Caramujo Store](https://instagram.com/caramujo_store)
- [Toca do Jack](https://instagram.com/toca_pub_underground)
- [Os Pirata](https://instagram.com/ospirata_sao_carlos)

---

## 📬 Contato

- 🌐 [bandarevanche.com.br](https://bandarevanche.com.br)
- 📧 contato@bandarevanche.com
- 📱 [Instagram](https://instagram.com/banda.revanche) · [TikTok](https://tiktok.com/@bandarevanche) · [Spotify](https://open.spotify.com/playlist/3uoiG5vPNcJg1i81Dlv5Ae)

---

<div align="center">

Desenvolvido por **FG SOFTWARE** &copy; 2026 REVANCHE — Todos os direitos reservados.

</div>
