# Giliade — Claude Code OS

## O que e esse workspace
Central operacional dos dois projetos do Giliade: G.L Trafego (agencia de trafego pago) e Vinci Tech (e-commerce de smartwatches). Aqui ficam contexto, processos, templates, conteudo e tudo que o Claude precisa pra trabalhar.

**Estrutura de pastas:**
- `gl-trafego/` — clientes, propostas e processos da agencia
  - `clientes/` — uma pasta por cliente (usar `_modelo-cliente/` como template)
  - `propostas/` — propostas comerciais
  - `processos/` — documentacao de processos e fluxos
- `vinci-tech/` — criativos, ofertas e campanhas da marca
  - `criativos/` — pecas e roteiros de anuncios
  - `ofertas/` — estrategias de kits, combos e bonus
  - `campanhas/` — estrutura de campanhas ativas
- `conteudo/` — conteudo para redes sociais
  - `instagram-pessoal/` — posts e roteiros pro @ogiliadebarth
- `_contexto/` — contexto do negocio, preferencias e estrategia
- `marca/` — guia de identidade visual
- `dados/` — arquivos pra analise (CSV, XLSX, PDF)
- `templates/skills/` — templates de skills prontos pra personalizar com /mapear
- `templates/ferramentas/catalogo.md` — APIs e ferramentas disponiveis pra usar em skills

## Sobre o negocio
Giliade da Silva Bartolomeu opera dois projetos separados: G.L Trafego (agencia de gestao de trafego pago, funis e estrutura comercial pra clientes externos) e Vinci Tech (marca propria de smartwatches, e-commerce B2C). Atuacao solo com apoio pontual.

## O que mais fazemos aqui
- Gestao de trafego pago (Meta Ads e Google Ads)
- Estrategia de campanhas e funis (Ads > WhatsApp > Venda)
- Roteiros de anuncios e criativos (UGC, direto, comercial)
- Propostas comerciais pra clientes da agencia
- Criativos e ofertas pra Vinci Tech
- Conteudo pro Instagram (@ogiliadebarth e @usevincitech)
- Relatorios de resultados
- Analise de metricas e otimizacao

## Clientes e contexto
G.L Trafego atende clientes externos — negocios locais e empresas que ja vendem e querem escalar. Vinci Tech vende direto pro consumidor final (B2C). Foco atual: bater 30 clientes ativos na agencia.

## Tom de voz
Direto, comercial, estrategico, sem enrolacao. Linguagem simples e focada em resultado. Sem textos longos, sem linguagem generica, sem excesso de emojis, sem complexidade desnecessaria. Sempre com CTA claro.

## Ferramentas conectadas
- Meta Ads
- Google Ads
- Google Tag Manager (GTM)
- ManyChat
- Notion
- Nuvemshop
- HostGator
- WhatsApp
- Planilhas

---

## Contexto do negocio

No inicio de toda conversa, ler os seguintes arquivos (se existirem e estiverem configurados):

1. `_contexto/empresa.md` — quem e o usuario, o que faz, como funciona o negocio
2. `_contexto/preferencias.md` — tom de voz, estilo de escrita, o que evitar
3. `_contexto/estrategia.md` — foco atual, prioridades, o que pode esperar

Usar essas informacoes como base pra qualquer resposta ou decisao. Ao sugerir prioridades, formatos ou abordagens, considerar o foco atual descrito em `estrategia.md`.

Para qualquer tarefa visual (carrossel, proposta, slide, landing page), consultar `marca/design-guide.md` como referencia de estilo.

Nao e necessario listar o que foi lido nem confirmar a leitura. Apenas usar o contexto naturalmente.

---

## Fluxo de trabalho

Antes de executar qualquer tarefa, verificar se existe uma skill relevante em `.claude/skills/` ou `.claude/commands/`.
Se encontrar, seguir as instrucoes da skill.
Se nao encontrar, executar a tarefa normalmente.

Ao concluir uma tarefa que nao tinha skill mas parece repetivel (o usuario provavelmente vai pedir de novo no futuro), perguntar:

> "Isso pode virar uma skill pra proxima vez. Quer que eu crie?"

Nao perguntar pra tarefas pontuais ou perguntas simples. So quando o padrao de repeticao for claro.

---

## Aprender com correcoes

Quando o usuario corrigir algo, melhorar uma resposta ou dar uma instrucao que parece permanente (frases como "na verdade e assim", "nao faca mais isso", "prefiro assim", "sempre que...", "evita...", "da proxima vez..."), perguntar:

> "Quer que eu salve isso pra nao precisar repetir?"

Se sim, identificar onde faz mais sentido salvar:

- **Sobre o negocio** (quem sao os clientes, como funciona a empresa, servicos, mercado) → adicionar em `_contexto/empresa.md`
- **Sobre preferencias e estilo** (tom de voz, formato de resposta, o que evitar, como estruturar textos) → adicionar em `_contexto/preferencias.md`
- **Sobre prioridades e foco atual** (projetos em andamento, metas do momento, prazos importantes, o que e prioridade agora) → adicionar em `_contexto/estrategia.md`
- **Regra de comportamento nessa pasta** (onde salvar arquivos, como nomear, fluxos especificos) → adicionar no proprio `CLAUDE.md`

Salvar com uma linha nova clara, sem reformatar o arquivo inteiro. Confirmar o que foi salvo mostrando a linha adicionada.

Nao perguntar se a correcao for obvia de contexto imediato (ex: "na verdade o arquivo se chama X"). So perguntar quando a informacao tiver valor duradouro.

---

## Criacao de skills

Quando o usuario pedir pra criar uma nova skill:

1. Verificar se existe um template relevante em `templates/skills/`. Se existir, usar como base e adaptar pro contexto do usuario
2. Perguntar: "Essa skill e especifica pra esse projeto ou vai ser util em qualquer projeto?"
   - Especifica desse negocio → salvar em `.claude/skills/nome-da-skill/SKILL.md` (local)
   - Util em qualquer projeto → salvar em `~/.claude/skills/nome-da-skill/SKILL.md` (global)
3. Ler `_contexto/empresa.md` e `_contexto/preferencias.md` pra calibrar o conteudo da skill ao contexto do negocio
4. Se a skill precisar de arquivos de apoio (templates, referencias, exemplos), criar dentro da pasta da skill
5. Seguir o fluxo da skill-creator nativa do Claude Code
