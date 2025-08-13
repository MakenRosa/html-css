# Curso em Vídeo — **Desafios & Exercícios** (HTML5, CSS3 e um tiquinho de JS)

> Repositório de **estudos** baseado na trilha do **Curso em Vídeo**.
> **Status:** conteúdo **legado** (últimos commits há **+2 anos**). Mantido para **documentação/arquivo**.

---

## Sumário

* [Visão Geral](#visão-geral)
* [Estrutura](#estrutura)
* [Conteúdo por Diretório](#conteúdo-por-diretório)

  * [Desafios `d001` → `d015`](#desafios-d001--d015)
  * [Exercícios `ex001` → `ex026`](#exercícios-ex001--ex026)
* [Como Executar](#como-executar)
* [Dependências Externas & Mídia](#dependências-externas--mídia)
* [Avisos de Legado](#avisos-de-legado)
* [Ideias de Manutenção](#ideias-de-manutenção)
* [Créditos](#créditos)
* [Licença](#licença)

---

## Visão Geral

Coleção de **páginas estáticas** para praticar **HTML5**, **CSS3** e noções de **JavaScript** (bem pontuais).
Os exemplos cobrem: **texto, imagens, ícones, listas, links, mídia (áudio/vídeo), fontes, seletores, pseudo-classes, box model, backgrounds, tabelas, iframes, formulários e media queries**.

---

## Estrutura

```
/
├─ curso-em-video/
│  ├─ desafios/           # 15 “desafios” temáticos (d001 a d015)
│  └─ exercicios/         # exercícios guiados (ex001 a ex026, c/ subpastas)
├─ LICENSE
└─ curso-em-video/README.md   # (histórico antigo, mantido)
```

---

## Conteúdo por Diretório

### Desafios `d001` → `d015`

Resumo rápido do que cada um demonstra:

* **d001 – Mensagens**: parágrafos e quebras simples.
* **d002 – Imagens**: `<img>` + favicon.
* **d003 – Mapa**: mosaic de imagens alinhadas.
* **d004 – Emojis**: listas usando entidades Unicode.
* **d005 – Social**: mini “perfil” com foto e links (LinkedIn/GitHub/Instagram/Twitter).
* **d006 – Tags/Abbr**: dicas via `<abbr>` para tag correta.
* **d007 – Imagem flexível**: `<picture>` com `source` responsivo.
* **d008 – Navegação**: 3 páginas com cores diferentes e links entre si.
* **d009 – Vídeos**: “hub” com thumbs levando a páginas com **YouTube embed** e botão “voltar”.
* **d010 – Android (artigo)**: página temática (“Curiosidades de Tecnologia”), **Bootstrap 4.5 via CDN**, CSS autoral (`estilo/style.css`), fontes (Google Fonts + `@font-face`).
* **d011 – Astronauta**: posicionamento absoluto/centrado sobre background de espaço.
* **d012 – Cordel Moderno**: tipografia com **Google Fonts**, seções com **background fixo** (efeito parallax simples).
* **d013 – Tabelas**: mesclagens (`rowspan/colspan`), escopo, cabeçalho, médias.
* **d014 – Redes Sociais (mock)**: moldura de celular + `<iframe>` trocando “telas” (home, LinkedIn, GitHub, Instagram, Twitter).
* **d015 – Login Responsivo**: layout que muda com **media queries** (arquivos `style.css` + `media-query.css`).

> Dicas de navegação: cada desafio possui seu **`index.html`** (ou página principal) dentro de `curso-em-video/desafios/d0xx/`.

---

### Exercícios `ex001` → `ex026`

Destaques por tema (não exaustivo):

* **ex001–ex006**: “olá mundo”, parágrafos/quebras, **imagens locais/remotas**, **favicon**, **hierarquia de títulos**.
* **ex007**: HTML4 x HTML5 (boas práticas vs. tags antigas).
* **ex008–ex008b**: **formatações** (negrito/ênfase/mark/delete/insert/sub/sup), `<code>`, `<pre>`, citações, `<abbr>`, `<bdo>`.
* **ex009**: **listas** ordenadas, não ordenadas, aninhadas e de definição.
* **ex010**: **links** externos/internos, navegação entre páginas, **download** (pdf/zip).
* **ex011**: **imagem responsiva** com `<picture>` e **áudio** com múltiplos formatos.
* **ex012**: **vídeo** local (mp4/webm/ogv) e **YouTube embed**.
* **ex013–ex015**: estilos **inline**, **internos** e **externos**; navegação entre páginas com mesmo CSS.
* **ex016**: **cores** (nome, hex, rgb, hsl), **gradientes**, site exemplo com CSS externo.
* **ex017–ex018**: **fontes** (Google Fonts, `@font-face` local), alinhamentos e pesos.
* **ex019–ex020**: **seletores**, classes/ids, **pseudo-classes**, `:hover`, personalização de **links**.
* **ex021**: **box model**, grouping tags semânticas, **`border-image`**.
* **ex022**: **backgrounds** (repeat/size/position/fixed), centralização absoluta.
* **ex023**: **tabelas** (caption, thead/tbody/tfoot, sticky header, colgroup, responsividade via container com scroll).
* **ex024**: **iframes** (páginas extras carregadas na mesma view).
* **ex025**: **formulários** (múltiplas variações `formulario001`…`010` + `cadastro.html`).
* **ex026**: **media queries** (mq001…mq005) com CSS para **tela**, **impressão** e **orientação** (retrato/paisagem).

> Para cada exercício, abra o **`index.html`** (ou arquivo nomeado) na pasta correspondente, por exemplo:
> `curso-em-video/exercicios/ex024/iframe001.html`.

---

## Como Executar

Como é tudo **estático**, basta abrir os `.html` no navegador. Para evitar problemas com paths relativos, recomendo servir um HTTP local:

**Via VS Code (mais prático)**

1. Instale a extensão **Live Server**.
2. Clique em “Go Live” na barra de status (ou botão direito no `index.html` → *Open with Live Server*).

**Via Python (qualquer terminal)**

```bash
# na raiz do repositório
python -m http.server 5500
# acesse http://localhost:5500/curso-em-video/desafios/d010/index.html (exemplo)
```

---

## Dependências Externas & Mídia

Algumas páginas puxam recursos externos:

* **CDNs**: Bootstrap 4.5 (d010), **Google Fonts** (d010, d012, ex017, ex018).
* **YouTube**: vários embeds (d009, ex012).
* **Áudio/Vídeo locais**: `curso-em-video/exercicios/ex011/media/*`, `ex012/media/*`.
* **`@font-face` local**: `d010/estilo/style.css` referencia `../fontes/idroid.otf` (coloque a fonte na pasta indicada se quiser o visual idêntico).

> Se algum arquivo de **imagem/fonte** não carregar, verifique os caminhos e a existência dos assets mencionados nos HTML/CSS.

---

## Avisos de Legado

* **Compatibilidade**: exemplos refletem práticas da época; alguns atributos/links podem estar **obsoletos ou quebrados**.
* **Autoplay** de mídia pode ser bloqueado por navegadores modernos.
* **Segurança/Privacidade**: páginas com embeds/links externos dependem de políticas atuais dos provedores.
* **Intenção**: material **educacional**, **não** pensado para produção.

---

## Ideias de Manutenção

* Normalizar **encoding** e remover pequenos typos de marcação (ex.: tags não fechadas ou trocadas).
* Consolidar **assets** (imagens/fonts) em pastas previsíveis; revisar caminhos relativos.
* Adicionar um **index geral** com links para todos os desafios/exercícios.
* Incluir **A11y** (alt text descritivo, contraste, navegação por teclado) e **metas** de SEO básicas.
* Pinar versões de **CDNs** e substituir recursos que não existam mais.
* Converter trechos inline para **CSS externo** quando fizer sentido (boa prática).

---

## Créditos

* Conteúdo e inspiração da trilha **Curso em Vídeo (Gustavo Guanabara)**.
* **“Cordel Moderno”** por **Milton Duarte** (link referenciado no próprio desafio d012).
* Imagens, ícones e mídias conforme arquivos incluídos e/ou links nos próprios HTML.

---

## Licença

Veja `LICENSE`. Este acervo é voltado a **estudo**. Ao reutilizar trechos, verifique as **licenças** de terceiros (Bootstrap, Google Fonts, YouTube, etc.) e mantenha os **créditos**.

---

> *“Snapshot de aprendizado: bom para revisitar fundamentos. Se for continuar do ponto atual, vale modernizar as dependências e reforçar acessibilidade.”*
