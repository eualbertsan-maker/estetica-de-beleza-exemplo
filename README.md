# Design System: Landing Page Estética Premium

Design System para landing page de clínica de estética/harmonização, focado em **agendar consultas, apresentar resultados e coletar feedbacks**. Derivado de três referências visuais: paleta quente (verde-floresta, creme, areia, rosé nude), serif de alto contraste com itálico/script e sans geométrica de apoio.

## Estrutura

```
.
├── index.html              # Página de preview dos componentes
├── src/
│   ├── tokens.css          # Variáveis CSS (cores, fontes, espaçamento, raios, sombras)
│   ├── tokens.json         # Os mesmos tokens em JSON (Figma Tokens, Style Dictionary)
│   └── components.css      # Botões, inputs, cards, badges, depoimentos, formulário, FAQ
└── docs/
    └── design-system.md    # Documentação completa (7 tópicos)
```

## Como usar

1. Abra `index.html` no navegador para ver o preview.
2. Em outro projeto, importe os dois CSS nesta ordem:

```html
<link rel="stylesheet" href="src/tokens.css">
<link rel="stylesheet" href="src/components.css">
```

3. Use as classes: `btn btn--cta`, `btn btn--primary`, `btn btn--outline`, `card`, `badge`, `tag`, `input`, `select`, `textarea`, `testimonial`, `booking`, `faq`, entre outras.

Para publicar o preview no GitHub Pages: **Settings > Pages > Deploy from a branch > main / (root)**.

## Fontes

Carregadas via Google Fonts em `tokens.css`: Cormorant Garamond, Pinyon Script e Poppins.

## Observações

- Os valores HEX foram estimados visualmente a partir das imagens de referência. Valide com o manual de marca, se houver.
- O preview usa placeholders no lugar de imagens. Troque pelas fotos reais da clínica.
- Para divulgação de antes e depois e promessas de resultado, confirme as regras vigentes do CFM/CRO.
