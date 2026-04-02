# Brandbook — G.L Tráfego

**Versão:** 1.0
**Data:** Abril 2026
**Criado por:** Design Squad (Brad Frost + Dan Mall)
**Metodologia:** Atomic Design

---

## 1. Essência da Marca

### Propósito
Transformar tráfego em vendas previsíveis. Não só gerar cliques — construir máquinas de aquisição.

### Promessa
Estrutura comercial + tráfego pago = previsibilidade de vendas.

### Personalidade da marca
- **Estratégico** — não operacional, mas arquiteto de resultados
- **Direto** — sem enrolação, focado no que importa
- **Premium** — qualidade percebida em cada ponto de contato
- **Confiável** — dados e processo, não achismo

### Tagline sugerida
> "Tráfego que vende."

---

## 2. Logotipo

### 2.1 Conceito

O logotipo da G.L Tráfego é tipográfico (wordmark). A escolha é intencional: agências de performance vendem inteligência, não estética decorativa. O logo comunica precisão, profissionalismo e modernidade.

**Construção:**
- As letras **G** e **L** aparecem em caixa alta, peso **Bold (700)**, separadas por um ponto final: **G.L**
- A palavra **TRÁFEGO** aparece abaixo ou ao lado, em caixa alta, peso **Medium (500)**, com tracking expandido (+80)
- A fonte é **Inter** (ou Helvetica Neue como fallback)

### 2.2 Variações

#### Versão Principal (Horizontal)
```
G.L
TRÁFEGO
```
- "G.L" em Inter Bold 700, tamanho base 48px
- "TRÁFEGO" em Inter Medium 500, tamanho base 18px, tracking +80
- Alinhamento: esquerda
- "TRÁFEGO" alinhado abaixo do "G.L"

#### Versão Compacta (Uma linha)
```
G.L TRÁFEGO
```
- Tudo na mesma linha
- "G.L" em Bold 700, "TRÁFEGO" em Medium 500
- Separados por espaço equivalente a 1 caractere

#### Ícone Solo (Favicon / Avatar)
```
G.L
```
- Apenas "G.L" em Inter Bold 700
- Dentro de um quadrado com cantos arredondados (8px radius)
- Fundo preto, texto branco (ou inverso)

#### Versão Monocromática
- **Sobre fundo escuro:** Logo todo em #FFFFFF
- **Sobre fundo claro:** Logo todo em #000000
- **Sobre foto/textura:** Logo em branco com leve sombra sutil (0 2px 8px rgba(0,0,0,0.3))

### 2.3 Área de proteção

Manter uma margem mínima ao redor do logo equivalente à altura da letra "G" em todos os lados. Nenhum elemento pode invadir essa área.

### 2.4 Tamanhos mínimos

| Contexto | Tamanho mínimo do "G.L" |
|----------|------------------------|
| Digital (tela) | 24px |
| Impresso | 12mm |
| Favicon / ícone | 16px (usar versão ícone solo) |

---

## 3. Paleta de Cores

### 3.1 Cores Primárias

| Token | Hex | Uso |
|-------|-----|-----|
| `brand-black` | #000000 | Fundo principal, textos sobre claro |
| `brand-white` | #FFFFFF | Textos sobre escuro, CTAs, destaques |

### 3.2 Cores Neutras (Expandidas)

| Token | Hex | Uso |
|-------|-----|-----|
| `neutral-950` | #0A0A0A | Fundo alternativo sutil |
| `neutral-900` | #111111 | Cards, seções alternativas |
| `neutral-800` | #1A1A1A | Bordas ativas, separadores fortes |
| `neutral-700` | #2A2A2A | Hover em elementos escuros |
| `neutral-600` | #3A3A3A | Bordas padrão |
| `neutral-500` | #6B6B6B | Texto secundário, placeholders |
| `neutral-400` | #8A8A8A | Texto desabilitado |
| `neutral-300` | #B0B0B0 | Ícones inativos |
| `neutral-200` | #D4D4D4 | Bordas em fundo claro |
| `neutral-100` | #EDEDED | Fundo claro alternativo |
| `neutral-50`  | #F5F5F5 | Fundo claro principal |

### 3.3 Cores Semânticas (Feedback)

| Token | Hex | Uso |
|-------|-----|-----|
| `success` | #22C55E | Confirmações, métricas positivas |
| `warning` | #EAB308 | Alertas, atenção |
| `error` | #EF4444 | Erros, métricas negativas |
| `info` | #6B6B6B | Informativo neutro (cinza, não azul) |

> As cores semânticas são usadas **apenas** para feedback funcional (gráficos, alertas, status). Nunca como decoração.

---

## 4. Tipografia

### 4.1 Família tipográfica

| Uso | Fonte | Fallback |
|-----|-------|----------|
| Principal | Inter | Helvetica Neue, Arial, sans-serif |

### 4.2 Escala tipográfica

| Token | Tamanho | Peso | Line-height | Uso |
|-------|---------|------|-------------|-----|
| `heading-1` | 48px / 3rem | Bold 700 | 1.1 | Títulos de página, hero |
| `heading-2` | 36px / 2.25rem | Bold 700 | 1.15 | Seções principais |
| `heading-3` | 24px / 1.5rem | Semibold 600 | 1.2 | Subtítulos |
| `heading-4` | 20px / 1.25rem | Semibold 600 | 1.3 | Títulos de card |
| `body` | 16px / 1rem | Regular 400 | 1.6 | Texto corrido |
| `body-sm` | 14px / 0.875rem | Regular 400 | 1.5 | Texto auxiliar |
| `caption` | 12px / 0.75rem | Medium 500 | 1.4 | Labels, legendas |
| `label` | 14px / 0.875rem | Medium 500 | 1 | Botões, badges |
| `overline` | 12px / 0.75rem | Bold 700 | 1 | Categorias, tags (uppercase + tracking +80) |

### 4.3 Regras

- **Títulos:** Sempre em caixa alta ou sentence case. Nunca title case.
- **Corpo:** Sentence case sempre.
- **CTAs e botões:** Caixa alta com tracking expandido.
- **Máximo de pesos por página:** 3 (Regular, Semibold, Bold).

---

## 5. Espaçamento

### 5.1 Escala base (4px)

| Token | Valor |
|-------|-------|
| `space-0` | 0px |
| `space-1` | 4px |
| `space-2` | 8px |
| `space-3` | 12px |
| `space-4` | 16px |
| `space-5` | 20px |
| `space-6` | 24px |
| `space-8` | 32px |
| `space-10` | 40px |
| `space-12` | 48px |
| `space-16` | 64px |
| `space-20` | 80px |
| `space-24` | 96px |

### 5.2 Uso

- **Entre elementos inline:** `space-2` a `space-4`
- **Padding de cards:** `space-6` (24px)
- **Gap entre seções:** `space-12` a `space-16`
- **Margens de página:** `space-6` (mobile) / `space-16` (desktop)

---

## 6. Bordas e Sombras

### 6.1 Border radius

| Token | Valor | Uso |
|-------|-------|-----|
| `radius-sm` | 4px | Badges, tags |
| `radius-md` | 8px | Cards, inputs, botões |
| `radius-lg` | 12px | Modais, containers grandes |
| `radius-full` | 9999px | Avatares, pills |

### 6.2 Bordas

| Token | Valor | Uso |
|-------|-------|-----|
| `border-subtle` | 1px solid #1A1A1A | Separadores em fundo escuro |
| `border-default` | 1px solid #2A2A2A | Bordas de cards e inputs |
| `border-strong` | 1px solid #FFFFFF | Destaque, CTAs outline |

### 6.3 Sombras

| Token | Valor |
|-------|-------|
| `shadow-sm` | 0 1px 2px rgba(0,0,0,0.4) |
| `shadow-md` | 0 4px 12px rgba(0,0,0,0.5) |
| `shadow-lg` | 0 8px 24px rgba(0,0,0,0.6) |

> Sombras usadas com moderação. Preferir separação por cor/borda.

---

## 7. Grid e Layout

### 7.1 Breakpoints

| Token | Valor | Contexto |
|-------|-------|----------|
| `mobile` | 0 — 639px | Celular |
| `tablet` | 640 — 1023px | Tablet |
| `desktop` | 1024 — 1279px | Desktop |
| `wide` | 1280px+ | Tela grande |

### 7.2 Grid

- **Colunas:** 12 (desktop) / 4 (mobile)
- **Gutter:** 24px
- **Max-width do conteúdo:** 1200px
- **Alinhamento:** Centralizado

---

## 8. Componentes Visuais (Atoms)

### 8.1 Botões

| Variante | Fundo | Texto | Borda |
|----------|-------|-------|-------|
| **Primary** | #FFFFFF | #000000 | nenhuma |
| **Secondary** | transparente | #FFFFFF | 1px solid #FFFFFF |
| **Ghost** | transparente | #FFFFFF | nenhuma |
| **Disabled** | #2A2A2A | #6B6B6B | nenhuma |

- Padding: `12px 24px`
- Border-radius: `8px`
- Texto: `label` (14px Medium 500, uppercase, tracking +40)
- Hover Primary: fundo #E0E0E0
- Hover Secondary: fundo rgba(255,255,255,0.08)

### 8.2 Cards

- Fundo: `neutral-900` (#111111)
- Borda: `border-default` (#2A2A2A)
- Border-radius: `radius-md` (8px)
- Padding: `space-6` (24px)
- Sem sombra (ou `shadow-sm` quando elevado)

### 8.3 Inputs

- Fundo: `neutral-950` (#0A0A0A)
- Borda: `border-default`
- Borda focus: `border-strong` (#FFFFFF)
- Texto: #FFFFFF
- Placeholder: `neutral-500` (#6B6B6B)
- Border-radius: `radius-md`
- Padding: `12px 16px`

---

## 9. Aplicações da Marca

### 9.1 Instagram (@ogiliadebarth)

**Avatar/Foto de perfil:**
- Usar versão ícone solo "G.L" em fundo preto

**Posts estáticos:**
- Fundo: #000000
- Texto principal: #FFFFFF, Inter Bold
- Texto secundário: #6B6B6B, Inter Regular
- CTA: botão branco com texto preto na parte inferior
- Margem interna: 48px em todos os lados (1080x1080)

**Stories:**
- Mesmo padrão visual
- Texto maior (heading-2 mínimo)
- CTA sempre visível na parte inferior

**Carrosséis:**
- Capa: headline forte, fundo preto, texto branco
- Slides internos: fundo #111111, texto branco
- Último slide: CTA claro

### 9.2 Propostas Comerciais

- Capa: fundo preto, logo G.L Tráfego centralizado, nome do cliente abaixo
- Páginas internas: fundo #0A0A0A, texto branco, títulos em heading-3
- Destaques/números: heading-1, branco
- Rodapé: logo pequeno + contato em caption

### 9.3 Apresentações / Slides

- Fundo: #000000
- Títulos: Inter Bold, branco, alinhados à esquerda
- Conteúdo: bullet points com body-sm
- Um conceito por slide — sem poluição
- Logo no canto inferior direito (versão compacta, pequena)

### 9.4 Relatórios

- Gráficos: usar branco para a métrica principal, cinzas para secundárias, verde/vermelho só para indicar variação positiva/negativa
- Tabelas: bordas em `neutral-800`, fundo alternando `#000000` e `#0A0A0A`
- Cabeçalhos de tabela: `overline` style (12px, bold, uppercase)

---

## 10. Elementos Gráficos

### 10.1 Ícones

- Estilo: **Outline** (traço fino, 1.5px)
- Cor: #FFFFFF (padrão) ou #6B6B6B (inativo)
- Tamanho: 20px (inline) / 24px (standalone)
- Biblioteca recomendada: Lucide Icons ou Phosphor Icons (light)
- Nunca usar ícones preenchidos (filled) — quebra o minimalismo

### 10.2 Fotografia

- **Estilo:** Alto contraste, tons escuros, iluminação direcionada
- **Tratamento:** Dessaturar levemente (saturation -20%), aumentar contraste
- **Sobreposição:** Quando texto sobre foto, usar overlay preto com 60-80% opacidade
- **Evitar:** Fotos genéricas de banco de imagem, fotos com cores vibrantes, imagens de baixa qualidade

### 10.3 Elementos decorativos

- **Linhas finas** (1px, #2A2A2A) como separadores
- **Gradiente sutil** permitido: de #000000 para #111111 (nunca cores)
- **Formas geométricas** podem ser usadas como background sutil (retângulos, linhas em diagonal) em opacidade muito baixa (5-10%)
- **Proibido:** Patterns complexos, texturas, elementos 3D, glassmorphism

---

## 11. Regras de Uso — Do's e Don'ts

### DO's (Faça)
- Use o logo sempre com a área de proteção respeitada
- Mantenha contraste alto (branco sobre preto ou preto sobre branco)
- Use no máximo 3 pesos tipográficos por peça
- Deixe espaço em branco (respiro visual)
- Mantenha alinhamento consistente (preferencialmente à esquerda)
- Use as cores semânticas apenas para feedback funcional

### DON'Ts (Não faça)
- Nunca distorça, rotacione ou aplique efeitos no logo
- Nunca coloque o logo sobre fundo colorido vibrante
- Nunca use fontes diferentes de Inter / Helvetica Neue
- Nunca misture mais de 2 tamanhos de heading por peça
- Nunca use sombras pesadas (drop shadow forte)
- Nunca adicione bordas arredondadas acima de 12px (exceto pills/avatares)
- Nunca use degradê com cores — apenas preto para cinza escuro
- Nunca use emojis em materiais da marca (exceto redes sociais quando necessário)

---

## 12. Tom Visual Resumido

| Atributo | Descrição |
|----------|-----------|
| **Mood** | Sério, premium, estratégico |
| **Sensação** | "Esse cara sabe o que faz" |
| **Referências** | Apple, agências de design internacionais, marcas de consultoria premium |
| **Densidade** | Baixa — espaço em branco é parte da comunicação |
| **Movimento** | Mínimo — transições suaves quando necessário, nunca chamativo |

---

## Resumo de Tokens

```yaml
design_system:
  name: "G.L Tráfego Design System"
  creators: [brad-frost, dan-mall]
  methodology: "Atomic Design"
  accessibility_target: "WCAG 2.1 AA"
  tokens:
    colors: 18
    typography: 9
    spacing: 14
    borders: 3
    shadows: 3
    radius: 4
    breakpoints: 4
  components:
    atoms: [button, input, card, badge, icon, label, divider]
    molecules: [input-field, button-group, stat-card, nav-item]
    organisms: [navbar, form, data-table, report-section]
  logo:
    versions: [principal, compacta, icone-solo, monocromatica]
    font: "Inter Bold 700"
    construction: "G.L (bold) + TRÁFEGO (medium, tracking +80)"
```

---

*Este brandbook é o documento de referência para qualquer material visual da G.L Tráfego. Toda peça produzida deve seguir estas diretrizes.*
