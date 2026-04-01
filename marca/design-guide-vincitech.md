# Design System — Vinci Tech

> Identidade visual completa para o e-commerce de smartwatches.
> Criado pelo Design Squad (Brad Frost + Dan Mall methodology).
> Toda peça visual da Vinci Tech deve seguir este guia.

---

## 1. Fundamentos da Marca

**Posicionamento:** Tecnologia premium acessível — smartwatches modernos com custo-benefício real.
**Tom visual:** Minimalista, tecnológico, confiável, premium sem ser elitista.
**Referências estéticas:** Apple, MVMT Watches, Xiaomi global — clean, produto como protagonista.

---

## 2. Paleta de Cores

### Cores Primárias

| Token | Hex | Uso |
|-------|-----|-----|
| `brand-black` | #0A0A0A | Fundo principal, textos, headers |
| `brand-white` | #FAFAFA | Fundo alternativo, textos sobre escuro |
| `brand-accent` | #C8C8C8 | Destaque sutil, bordas, elementos secundários |

### Cores Secundárias

| Token | Hex | Uso |
|-------|-----|-----|
| `surface-dark` | #141414 | Cards sobre fundo preto, elevação 1 |
| `surface-medium` | #1E1E1E | Elevação 2, hover states |
| `surface-light` | #F5F5F5 | Fundo claro (páginas de produto, checkout) |
| `border-subtle` | #2A2A2A | Bordas em modo escuro |
| `border-light` | #E0E0E0 | Bordas em modo claro |

### Cores de Feedback

| Token | Hex | Uso |
|-------|-----|-----|
| `success` | #22C55E | Confirmação, em estoque, sucesso |
| `warning` | #F59E0B | Últimas peças, atenção |
| `error` | #EF4444 | Erro, esgotado |
| `info` | #3B82F6 | Informação, frete grátis |

### Cores de Oferta

| Token | Hex | Uso |
|-------|-----|-----|
| `discount-bg` | #0A0A0A | Badge de desconto (fundo) |
| `discount-text` | #FAFAFA | Badge de desconto (texto) |
| `price-old` | #999999 | Preço riscado |
| `price-new` | #0A0A0A | Preço atual (modo claro) |
| `price-new-dark` | #FAFAFA | Preço atual (modo escuro) |

### O que NÃO usar

- ~~#1abc9c (teal atual do site)~~ — remover
- ~~#c0392b (vermelho atual)~~ — remover
- ~~#f1c40f (amarelo atual)~~ — remover
- Nenhuma cor vibrante como protagonista. Cor = funcional, nunca decorativa.

---

## 3. Tipografia

### Família

| Uso | Fonte | Fallback |
|-----|-------|----------|
| Principal | **Inter** | Helvetica Neue, Arial, sans-serif |
| Alternativa (headings impactantes) | **Instrument Sans** (já presente no site) | Inter, sans-serif |

### Escala Tipográfica

| Token | Tamanho | Peso | Line-height | Uso |
|-------|---------|------|-------------|-----|
| `display` | 48px / 3rem | 700 | 1.1 | Hero, banners principais |
| `h1` | 36px / 2.25rem | 700 | 1.2 | Título de página |
| `h2` | 28px / 1.75rem | 600 | 1.25 | Seções |
| `h3` | 22px / 1.375rem | 600 | 1.3 | Subtítulos, nomes de produto |
| `h4` | 18px / 1.125rem | 600 | 1.35 | Labels de seção |
| `body` | 16px / 1rem | 400 | 1.5 | Texto geral |
| `body-sm` | 14px / 0.875rem | 400 | 1.5 | Descrições curtas |
| `caption` | 12px / 0.75rem | 400 | 1.4 | Badges, notas, parcelamento |
| `cta` | 16px / 1rem | 700 | 1 | Botões e CTAs |
| `price` | 24px / 1.5rem | 700 | 1 | Preço principal |
| `price-old` | 14px / 0.875rem | 400 | 1 | Preço riscado |

### Regras

- Nunca usar mais de 2 pesos na mesma seção (400 + 600 ou 400 + 700)
- Títulos sempre em UPPERCASE quando em banners ou CTAs
- Corpo de texto nunca em uppercase
- Letter-spacing em headings: -0.02em (ligeiramente condensado)
- Letter-spacing em uppercase: +0.05em (mais aberto)

---

## 4. Espaçamento

### Escala (base: 4px)

| Token | Valor | Uso |
|-------|-------|-----|
| `space-1` | 4px | Micro ajustes |
| `space-2` | 8px | Padding interno de badges, gaps pequenos |
| `space-3` | 12px | Gap entre elementos inline |
| `space-4` | 16px | Padding padrão de cards e botões |
| `space-6` | 24px | Gap entre cards em grid |
| `space-8` | 32px | Separação de seções menores |
| `space-12` | 48px | Separação de seções principais |
| `space-16` | 64px | Margens top/bottom de seções hero |
| `space-24` | 96px | Separação de blocos maiores |

---

## 5. Componentes (Atoms)

### Botões

| Variante | Fundo | Texto | Borda | Uso |
|----------|-------|-------|-------|-----|
| **Primary** | #0A0A0A | #FAFAFA | nenhuma | Comprar, CTA principal |
| **Primary (hover)** | #1E1E1E | #FAFAFA | nenhuma | — |
| **Secondary** | transparente | #0A0A0A | 1px #0A0A0A | Ver mais, ação secundária |
| **Secondary (hover)** | #0A0A0A | #FAFAFA | 1px #0A0A0A | — |
| **Ghost** | transparente | #0A0A0A | nenhuma | Links, ações terciárias |
| **Disabled** | #E0E0E0 | #999999 | nenhuma | Esgotado |
| **WhatsApp** | #25D366 | #FFFFFF | nenhuma | CTA de WhatsApp (única cor permitida) |

**Especificações:**
- Border-radius: 6px
- Padding: 12px 24px
- Font: 16px / 700 / uppercase
- Letter-spacing: +0.05em
- Transição hover: 200ms ease

### Badges

| Variante | Fundo | Texto | Uso |
|----------|-------|-------|-----|
| **Desconto** | #0A0A0A | #FAFAFA | "-42% OFF" |
| **Frete grátis** | #0A0A0A | #FAFAFA | "FRETE GRÁTIS" |
| **Últimas peças** | transparente | #F59E0B | "Últimas peças" |
| **Novo** | #0A0A0A | #FAFAFA | "NOVO" |
| **Esgotado** | #E0E0E0 | #999999 | "ESGOTADO" |

**Especificações:**
- Border-radius: 4px
- Padding: 4px 8px
- Font: 12px / 700 / uppercase

### Inputs

- Border: 1px solid #E0E0E0
- Border-radius: 6px
- Padding: 12px 16px
- Font: 16px
- Focus: border 1px solid #0A0A0A
- Error: border 1px solid #EF4444

---

## 6. Componentes (Molecules)

### Product Card

```
┌─────────────────────────┐
│  [Badge: -42% OFF]      │
│                         │
│      [Foto produto]     │
│                         │
│  [Variantes de cor: ●●●]│
├─────────────────────────┤
│  Nome do Produto        │  ← h3, 600
│  ~~R$ 599,00~~          │  ← price-old, riscado
│  R$ 348,00              │  ← price, 700, destaque
│  6x de R$ 58,00 s/juros │  ← caption
│                         │
│  [   COMPRAR   ]        │  ← botão primary
└─────────────────────────┘
```

**Especificações:**
- Background: #FFFFFF
- Border: 1px solid #E0E0E0
- Border-radius: 8px
- Padding: 0 (imagem sangra) + 16px (área de texto)
- Hover: shadow 0 4px 12px rgba(0,0,0,0.08)
- Transição: 200ms ease

### Navigation Bar

```
┌──────────────────────────────────────────────┐
│  [Logo]    Smartwatches  Acessórios    [🔍] [🛒] │
└──────────────────────────────────────────────┘
```

- Fundo: #FFFFFF
- Height: 64px
- Border-bottom: 1px solid #E0E0E0
- Logo à esquerda, nav ao centro, ícones à direita
- Sticky on scroll

### Banner de Promoção (barra superior)

```
┌──────────────────────────────────────────────┐
│  FRETE GRÁTIS + 6X SEM JUROS | CUPOM: BEMVINDO │
└──────────────────────────────────────────────┘
```

- Fundo: #0A0A0A
- Texto: #FAFAFA
- Font: 13px / 600 / uppercase
- Height: 36px
- Substituir a barra vermelha atual

---

## 7. Diretrizes de Imagem

### Fotos de Produto

- **Fundo:** Branco puro (#FFFFFF) ou cinza muito claro (#F5F5F5)
- **Iluminação:** Suave, sem sombras duras
- **Ângulo:** 3/4 para smartwatches (mostra tela + pulseira)
- **Proporção:** 1:1 (quadrado) para cards, 4:3 para páginas de produto
- **Resolução mínima:** 1200x1200px

### Fotos de Lifestyle/UGC

- **Estilo:** Natural, pessoa real usando o relógio
- **Cores frias:** Ambientes neutros, clean
- **Foco:** No pulso/relógio, fundo desfocado
- **Evitar:** Cenários poluídos, cores vibrantes demais

### Fotos para Anúncios (Meta Ads)

- **Formato:** 1:1 (feed), 9:16 (stories/reels)
- **Regra:** Produto em 60% do frame, texto em 20%, respiro em 20%
- **Texto no criativo:** Máximo 3 linhas — hook + benefício + preço
- **CTA:** Sempre visível, botão preto com texto branco

---

## 8. Criativos e Anúncios

### Estrutura Visual de Anúncio

```
┌─────────────────────────────┐
│                             │
│  HOOK (texto impactante)    │  ← Inter 700, 24px, branco
│                             │
│      [Foto do produto       │
│       em uso real]          │
│                             │
│  R$ 348,00                  │  ← Inter 700, 32px
│  6x sem juros + frete grátis│  ← Inter 400, 14px
│                             │
│  [    COMPRAR AGORA    ]    │  ← botão branco sobre preto
│                             │
└─────────────────────────────┘
```

### Paleta de Criativos

| Tipo | Fundo | Texto | Elemento |
|------|-------|-------|----------|
| **Dark (padrão)** | #0A0A0A | #FAFAFA | Produto com luz suave |
| **Light** | #FAFAFA | #0A0A0A | Produto em fundo limpo |
| **Contraste** | Split preto/branco | Misto | Produto no centro |

### Regras para Criativos

1. Máximo 2 fontes (Inter regular + bold)
2. Máximo 3 cores por peça (fundo + texto + 1 destaque)
3. Produto SEMPRE visível — nunca só texto
4. CTA sempre na parte inferior
5. Logo Vinci Tech discreto no canto superior (pequeno)
6. Nunca usar: emojis em excesso, fundos coloridos, fontes decorativas

---

## 9. Instagram (@usevincitech)

### Grid Visual

- Alternar posts escuros e claros para criar ritmo no feed
- Padrão sugerido: Dark → Light → UGC → Dark → Light → UGC
- Reels: sempre com legendas em fonte Inter, fundo semitransparente preto

### Stories

- Fundo: #0A0A0A ou imagem com overlay preto 60%
- Texto: Inter 700, branco
- CTA: Sticker de link com fundo preto
- Evitar: Stickers coloridos do Instagram, GIFs excessivos

### Highlights

- Ícones: Linha fina, branco sobre fundo preto
- Categorias: Relógios | Ofertas | Reviews | FAQ | Sobre

---

## 10. Aplicações Adicionais

### Embalagem

- Caixa preta fosca com logo em branco (relevo seco ou hot stamping)
- Interior: Espuma preta, relógio visível ao abrir
- Sensação de unboxing premium (referência: MVMT, Daniel Wellington)

### WhatsApp

- Mensagem de boas-vindas: texto limpo, sem emojis em excesso (máximo 2)
- Fotos de produto: sempre com fundo branco
- Catálogo: organizado por categoria
- Tom: direto, amigável, sem forçar intimidade

### E-mail Marketing

- Template: fundo branco, header preto com logo
- Máximo 2 seções de produto por email
- CTA principal em botão preto
- Sem imagens de fundo ou layouts complexos

---

## 11. Breakpoints (Responsivo)

| Token | Valor | Contexto |
|-------|-------|----------|
| `mobile` | 0 — 767px | Layout em coluna única |
| `tablet` | 768px — 1023px | Grid 2 colunas |
| `desktop` | 1024px — 1439px | Grid 3-4 colunas |
| `wide` | 1440px+ | Container max-width: 1280px |

---

## 12. Acessibilidade

- Contraste mínimo: 4.5:1 para texto, 3:1 para elementos grandes
- Preto (#0A0A0A) sobre branco (#FAFAFA) = ratio 17.4:1 ✓
- Todos os botões com focus visible (outline: 2px solid #0A0A0A)
- Imagens de produto com alt text descritivo
- Formulários com labels visíveis

---

## 13. Resumo Rápido — Cheat Sheet

```
CORES:     Preto #0A0A0A | Branco #FAFAFA | Cinza #C8C8C8
FONTE:     Inter (400 / 600 / 700)
BOTÃO:     Preto, 6px radius, uppercase, 16px bold
CARD:      Branco, 8px radius, borda #E0E0E0
IMAGEM:    Fundo branco, produto em 3/4, 1200x1200px
CRIATIVO:  Dark mode padrão, produto + hook + preço + CTA
PROIBIDO:  Cores vibrantes, fontes decorativas, visual poluído
```

---

## Changelog

| Data | Mudança |
|------|---------|
| 2026-04-01 | Criação inicial — Design Squad (Brad Frost + Dan Mall methodology) |

---

*Este guia é a referência oficial pra qualquer material visual da Vinci Tech.*
*Skills de carrossel, proposta, slide e criativo leem este arquivo antes de criar.*
