# Design System: Landing Page Estética Premium

Base extraída das 3 referências: o site Lumina Botanicals (layout e UI), o post Face Odontologia & Medicina (tipografia serif forte + script) e o post Dra. Nathalia Frias (serif com itálico + sans geométrica sobre foto). O sistema une esses padrões em regras reutilizáveis para uma landing de **agendamento de consultas, apresentação de resultados e coleta de feedbacks**.

## Padrões recorrentes identificados

- Paleta quente e neutra (verde-floresta profundo, creme, areia, rosé nude), sem cores saturadas.
- Títulos em serif de alto contraste, com contraste de peso ou estilo dentro da mesma frase (itálico ou script).
- Texto de apoio em sans-serif geométrica, leve e pequena.
- Fotografia de rosto/pele em close, iluminação suave, sensação de cuidado e luxo discreto.
- Muito respiro, poucos elementos por bloco, CTAs em formato pílula.
- Cantos bastante arredondados em cards e imagens, sombras quase imperceptíveis.
- Alternância de seções escuras e claras para criar ritmo.
- Eyebrow (texto pequeno em caixa alta com espaçamento) acima de títulos.

## 1. Cores

### Paleta principal

| Token | HEX | Uso |
|---|---|---|
| `--color-forest-900` | #141A14 | Fundo de hero escuro, rodapé, botão primário |
| `--color-forest-800` | #1F261D | Seções escuras alternadas, hover do botão escuro |
| `--color-cream-100` | #F6EFE6 | Fundo geral da página |
| `--color-sand-200` | #EADBC8 | Superfícies (cards, seções de destaque) |
| `--color-rose-500` | #B9807A | Acento (palavras em destaque, ícones, CTA de conversão) |

### Secundárias e de suporte

| Token | HEX | Uso |
|---|---|---|
| `--color-white-warm` | #FBF8F3 | Cards sobre fundo areia, inputs |
| `--color-rose-600` | #9C6660 | Hover/active do acento |
| `--color-rose-100` | #F0DDD8 | Fundo de badges e tags, estados selecionados |
| `--color-gold-500` | #B8935A | Filetes, detalhes finos, estrelas de avaliação |
| `--color-lilac-300` | #B9A7C6 | Destaque pontual em frases-chave (máx. 1 por seção) |
| `--color-sage-500` | #6F8467 | Ícones de apoio e sucesso suave |

### Texto, bordas e estados

| Token | HEX | Uso |
|---|---|---|
| `--text-title` | #1E1E1C | Títulos sobre fundo claro |
| `--text-body` | #3A3A3A | Corpo de texto (grafite quente) |
| `--text-muted` | #6B655E | Texto secundário, legendas, placeholders |
| `--text-on-dark` | #F6EFE6 | Texto sobre fundos escuros |
| `--border-soft` | #DCCDB8 | Bordas de cards e divisores |
| `--border-strong` | #3A3A3A | Borda de botão outline |
| `--color-success` | #5F7A5A | Confirmação de agendamento |
| `--color-error` | #A5473F | Erros de formulário |
| `--focus-ring` | #B9807A a 40% | Anel de foco |

### Hierarquia de uso (regra 60-30-10)

- **60%**: creme e off-white (fundos).
- **30%**: verde-floresta e areia (seções de contraste e superfícies).
- **10%**: rosé (acento e conversão), com dourado e lilás apenas como detalhe.
- Máximo de **uma cor de acento por seção**. Rosé nunca é fundo de seção inteira.
- Texto sobre fundo escuro sempre em creme, nunca branco puro. Contraste mínimo AA (4.5:1) no corpo de texto.
- O CTA principal da página usa sempre o mesmo estilo para ser reconhecido de imediato.

## 2. Tipografia

### Estilos identificados

- **Display**: serif de alto contraste, elegante e editorial (referências 1 e 3), ou serif didone mais pesada em linhas curtas (referência 2).
- **Itálico expressivo**: uma palavra da frase em itálico ("desejo") para criar ênfase emocional.
- **Script**: caligrafia fina e fluida como contraponto ("facial"), apenas como detalhe decorativo.
- **Sans de apoio**: geométrica, leve, limpa (aparência de Poppins/Jost).

### Fontes recomendadas (Google Fonts)

| Função | Fonte principal | Alternativas |
|---|---|---|
| Display (H1, H2) | **Cormorant Garamond** (500/600) | Playfair Display, Bodoni Moda |
| Itálico de ênfase | **Cormorant Garamond Italic** | Instrument Serif Italic |
| Script decorativo | **Pinyon Script** | Mrs Saint Delafield, Allura |
| Texto e UI | **Poppins** (300/400/500) | Jost, Montserrat |

Para a versão mais pesada da referência 2, use **Playfair Display 600** nos H1 de campanha. Escolha uma só família serif por projeto.

### Hierarquia (desktop)

| Nível | Fonte | Peso | Tamanho | Line-height | Letter-spacing |
|---|---|---|---|---|---|
| H1 | Cormorant Garamond | 500 | 64px | 1.05 | -0.02em |
| H2 | Cormorant Garamond | 500 | 44px | 1.1 | -0.01em |
| H3 | Cormorant Garamond | 600 | 28px | 1.2 | 0 |
| H4 | Poppins | 500 | 18px | 1.4 | 0 |
| Texto de destaque (lead) | Poppins | 300 | 18px | 1.7 | 0 |
| Corpo | Poppins | 400 | 16px | 1.7 | 0 |
| Texto secundário | Poppins | 400 | 14px | 1.6 | 0 |
| Label / eyebrow | Poppins | 500 | 12px, caixa alta | 1.4 | 0.18em |
| Botão | Poppins | 500 | 13–14px, caixa alta | 1 | 0.1em |
| Link | Poppins | 500 | herda | herda | 0, sublinhado fino |
| Script decorativo | Pinyon Script | 400 | 56–72px | 1 | 0 |

### Regras tipográficas

- Títulos com no máximo 2 a 3 linhas.
- Dentro de um título, destaque **uma** palavra com itálico ou cor rosé (nunca os dois).
- Corpo de texto com no máximo 60 a 70 caracteres por linha.
- Eyebrow em caixa alta acima do título quando houver contexto de seção.

## 3. Componentes

### Botão primário (escuro)

- **Aparência**: pílula sólida, texto em caixa alta com tracking.
- **Cores**: fundo #141A14, texto #F6EFE6.
- **Tamanho/padding**: altura 48px, padding 14px 32px; mobile 52px e largura total.
- **Border-radius**: 999px. **Borda**: nenhuma. **Sombra**: nenhuma em repouso.
- **Hover**: fundo #1F261D, translateY(-1px), sombra 0 8px 20px rgba(20,26,20,.18).
- **Active**: fundo #0C100C, sem elevação.
- **Focus**: anel 3px rosé a 40% com offset 2px.
- **Disabled**: fundo #B9B3A8, texto #F6EFE6, cursor not-allowed.

### Botão de conversão (CTA "Agendar consulta")

- Mesma geometria do primário, fundo **rosé #B9807A**, texto #FBF8F3. Sobre fundos escuros, pode usar a versão clara (fundo #F6EFE6, texto #141A14), como no hero da referência 1.
- **Hover**: #9C6660. **Active**: #8A5750. **Disabled**: #E3D3CE com texto #9A8F88.
- Ícone opcional à direita (seta ou WhatsApp) de 16px.

### Botão secundário (outline)

- Pílula com borda 1px #3A3A3A, fundo transparente, texto #3A3A3A, Poppins 14px, altura 44px, padding 12px 24px.
- **Hover**: fundo #3A3A3A com texto creme. **Active**: fundo #1E1E1C. **Focus**: anel rosé. **Disabled**: borda e texto #B9B3A8.
- Sobre fundo escuro: borda e texto em creme.

### Botão circular de ícone

- 32 a 40px, fundo #141A14, ícone "+" ou seta em creme. Hover: rosé.

### Links

- Cor herdada ou #141A14, peso 500, sublinhado 1px com offset 4px. Hover: #9C6660. Na navegação, sem sublinhado, com indicador de 1px no item ativo.

### Navegação

- Header transparente sobre o hero: logo à esquerda, links centralizados (Poppins 13px 500), ícones ou CTA à direita.
- Ao rolar: fundo #141A14 a 92% com blur de 12px, altura 72px.
- Mobile: logo + botão de menu; menu em tela cheia com fundo #141A14, links em serif 32px e CTA de agendamento fixo no rodapé do menu.

### Inputs, selects e textareas

- **Cores**: fundo #FBF8F3, texto #3A3A3A, placeholder #6B655E, borda 1px #DCCDB8.
- **Tamanho**: altura 52px; textarea mínimo 120px. Padding 14px 20px.
- **Radius**: 14px. Pílula (999px) apenas em campo de busca/newsletter. Sem sombra.
- **Hover**: borda #B9A98F. **Focus/Active**: borda #B9807A + anel 3px rosé a 25%. **Disabled**: fundo #EFE7DB, texto #A59E94.
- **Erro**: borda #A5473F e mensagem de 12px abaixo do campo.
- **Select**: mesmo estilo, chevron fino de 16px em #6B655E; lista com radius 14px, fundo #FBF8F3 e sombra 0 12px 32px rgba(20,26,20,.12).
- **Label**: Poppins 12px, 500, caixa alta, tracking 0.12em, cor #3A3A3A.

### Cards (serviço / produto / procedimento)

- **Aparência**: imagem no topo com cantos arredondados e bloco de texto abaixo, tudo em um card suave.
- **Cores**: fundo areia #EADBC8 (ou off-white sobre fundo areia).
- **Radius**: 20px; imagem com 16px. **Borda**: nenhuma ou 1px #DCCDB8.
- **Padding**: 16px ao redor da imagem, 20px no bloco de texto.
- **Tipografia**: título em serif 22px, descrição em Poppins 13px #6B655E, preço ou rótulo em 600.
- **Sombra**: 0 2px 12px rgba(20,26,20,.06).
- **Hover**: sombra 0 14px 32px rgba(20,26,20,.12), imagem com zoom 1.03. **Active**: escala 0.99. **Focus**: anel rosé. **Disabled**: opacidade 55%.

### Badges e tags

- Pílula de 28px de altura, padding 6px 14px, fundo #F0DDD8, texto #9C6660, Poppins 12px 500, sem borda.
- Variante escura: fundo #141A14 com texto creme. Variante outline: borda 1px #DCCDB8.
- Tags de filtro selecionadas: fundo #141A14 e texto creme.

### Seções de conteúdo e elementos de destaque

- Hero escura, seção clara com duas colunas (imagens + texto), grade de cards e seção escura de fechamento com CTA.
- Destaque de frase-chave: caixa com fundo lilás #B9A7C6 a 35% e radius 4px (referência 3), no máximo uma vez por seção.
- Filete decorativo de 1px dourado com ornamento no centro, entre eyebrow e título.

### Depoimentos e prova social

- Card com fundo #FBF8F3, radius 20px, padding 28px, borda 1px #DCCDB8.
- Aspas decorativas em Cormorant 56px rosé; texto em serif itálico 20px; nome em Poppins 500 14px e procedimento em #6B655E 12px.
- Avatar circular de 48px, estrelas em #B8935A.
- Faixa de números de confiança (anos de experiência, pacientes atendidos, avaliação média) em serif 40px, rótulo em caixa alta 12px.
- Carrossel com setas circulares e indicadores de 6px.
- Resultados (antes e depois): par de imagens lado a lado com radius 16px, legenda discreta e aviso de que resultados variam.

### Formulário de agendamento

- Card em fundo areia, radius 24px, padding 40px (mobile 24px). Título H3 serif e subtítulo curto.
- Campos: nome, WhatsApp, procedimento de interesse (select), melhor horário (select) e mensagem opcional.
- CTA de conversão em largura total. Abaixo, microtexto de 12px e checkbox de consentimento LGPD.
- Estado de sucesso: ícone de check em #5F7A5A e mensagem acolhedora com próximos passos.

## 4. Estética e layout

| Regra | Valor |
|---|---|
| Border-radius | Botões 999px, cards 20px, imagens 16 a 24px, inputs 14px, badges 999px |
| Sombras | Muito suaves: 0 2px 12px rgba(20,26,20,.06); hover 0 14px 32px rgba(20,26,20,.12) |
| Bordas | 1px #DCCDB8 só quando necessário; preferir contraste de superfície |
| Escala de espaçamento | 4, 8, 12, 16, 24, 32, 48, 64, 96, 128px |
| Padding de seção | 96px vertical (desktop), 72px (tablet), 56px (mobile) |
| Container máximo | 1200px (conteúdo), 1360px (hero e grids de imagem), margens laterais 24px |
| Grid | 12 colunas, gap 24px. Cards em 3 colunas; texto + imagem em 5/7 ou 6/6 |
| Alinhamento | Hero e seções de texto à esquerda; títulos de grades de produto centralizados |
| Densidade | Baixa: 1 mensagem, 1 CTA e 1 imagem principal por seção |
| Hierarquia | Imagem emocional > título serif > CTA > texto de apoio > metadados |
| Espaço negativo | Pelo menos 40% da área de cada seção sem conteúdo |
| Proporção texto/imagem | ~40% texto e 60% imagem no hero; imagens com foco no rosto ou na pele |

Para hero com foto, use gradiente de legibilidade da esquerda (rgba(20,26,20,.85) para transparente) ou desloque o rosto para a direita, deixando o texto na esquerda, como na referência 1.

## 5. Direção visual

- **Personalidade**: acolhedora, refinada e confiável; luxo calmo, não ostensivo.
- **Sensação**: cuidado, bem-estar, naturalidade e segurança clínica. Transmitir "resultado natural", não transformação radical.
- **Sofisticação**: alta, com minimalismo quente.
- **Densidade de informação**: baixa. Textos curtos e escaneáveis, detalhes em seções expansíveis (FAQ).
- **Imagens**: close de rosto e pele, luz suave e direcional, tons quentes, expressão relaxada. Tratamento consistente (levemente quente, contraste baixo). Evitar imagens frias, agulhas em primeiro plano em excesso e fotos de banco genéricas.
- **Textos**: títulos serif grandes e arejados, ênfase por itálico/script, corpo leve. Tom próximo, sem jargão técnico e sem promessas absolutas.
- **Contrastes**: fortes entre seções escuras e claras, suaves dentro de cada seção.
- **Elementos decorativos**: ornamento botânico de linha fina, filetes dourados, script em rosé como assinatura de campanha. Sem gradientes chamativos, ícones preenchidos ou ilustrações coloridas.
- **Linguagem dos CTAs**: pílulas, caixa alta com tracking, verbos suaves ("Agendar avaliação", "Ver resultados", "Conhecer procedimentos"), ícones finos (stroke 1.5px).

## 6. Responsividade

Breakpoints: mobile até 767px, tablet 768 a 1023px, desktop a partir de 1024px.

| Aspecto | Mobile | Tablet | Desktop |
|---|---|---|---|
| Grid | 4 colunas, gap 16px | 8 colunas, gap 20px | 12 colunas, gap 24px |
| H1 / H2 / H3 | 38 / 30 / 22px | 52 / 36 / 24px | 64 / 44 / 28px |
| Corpo | 16px (nunca abaixo) | 16px | 16px |
| Padding de seção | 56px vertical, 20px lateral | 72px, 32px | 96px, 24px |
| Navegação | Hambúrguer em tela cheia, CTA fixo | Hambúrguer ou links reduzidos | Links centralizados + CTA |
| Hero | Imagem no topo (60vh) com gradiente, texto abaixo, CTA largura total | 2 colunas 50/50 | 2 colunas, imagem sangrando à direita |
| Cards | 1 coluna (ou carrossel com peek de 15%) | 2 colunas | 3 colunas |
| Texto + imagem | Imagem primeiro, texto abaixo | 2 colunas | 2 colunas 5/7 |
| Imagens | Radius 16px, proporção 4:5 | 4:5 ou 1:1 | Proporções livres, radius 24px |
| Botões | Largura total, altura 52px | Largura automática | Largura automática, 48px |
| Formulários | Campos empilhados, padding 24px | 2 colunas para campos curtos | Card ao lado de texto persuasivo |
| Depoimentos | Carrossel de 1 card | 2 cards | 3 cards ou carrossel de 2 |

Regras adicionais: alvos de toque de no mínimo 44px, botão flutuante de WhatsApp no mobile (56px, rosé) e remoção de ornamentos decorativos em telas pequenas.

## 7. Usabilidade e conversão

Objetivo principal: **agendar consulta**. Secundários: apresentar serviços, mostrar resultados e coletar feedbacks.

### Estrutura recomendada da página

1. **Hero**: promessa emocional + CTA "Agendar avaliação" + indicador de confiança.
2. **Proposta de valor**: 2 a 3 pilares curtos (naturalidade, segurança, acompanhamento).
3. **Procedimentos**: cards com benefício, duração e botão "Saber mais".
4. **Resultados**: antes e depois em carrossel, com aviso de variação individual.
5. **Mitos e verdades** (referência 2): acordeões curtos que reduzem objeções.
6. **Profissional ou equipe**: foto, credenciais (CRO/CRM) e abordagem.
7. **Depoimentos**: cards com nome, procedimento e nota.
8. **Como funciona**: 3 passos (avaliação, plano, procedimento).
9. **Formulário de agendamento + FAQ**.
10. **Rodapé**: endereço, horários, mapa, redes sociais e WhatsApp.

### Regras de conversão

- Um CTA principal consistente (mesma cor, mesmo texto) no hero, após resultados, após depoimentos e no fechamento.
- CTA sempre visível: botão no header e botão flutuante de WhatsApp no mobile.
- Formulário curto (4 a 5 campos). Alternativa direta via WhatsApp com mensagem pré-preenchida.
- Microcopy que reduz fricção: "Sem compromisso", "Resposta em até 1 hora útil", "Avaliação personalizada".
- Feedback imediato: estado de carregamento no botão, confirmação clara e mensagem automática de retorno.
- Prova social próxima de cada CTA: nota média, quantidade de avaliações, depoimentos curtos.
- Coleta de feedbacks: após o atendimento, link de avaliação em 1 clique (estrelas) com campo opcional e autorização de uso do depoimento.

### Acessibilidade e conformidade

- Contraste AA, foco visível, labels sempre presentes, textos alternativos descritivos e animações com `prefers-reduced-motion`.
- Em saúde e estética no Brasil, evite promessas de resultado, respeite as normas do CFM e CRO sobre divulgação de antes e depois e inclua CRO/CRM do responsável técnico. Confirme a regra vigente com o conselho da sua categoria.
- Consentimento explícito (LGPD) em formulários e no uso de imagens de pacientes.

---

Os valores HEX foram estimados visualmente a partir das imagens. Se houver manual de marca ou arquivos originais, valide com um conta-gotas antes de implementar.
