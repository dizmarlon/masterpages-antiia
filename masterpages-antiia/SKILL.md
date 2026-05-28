---
name: Master Pages - Landing Page ANTI IA
description: "Cria landing pages premium com design autêntico, sem cara de IA. Use esta skill SEMPRE que o usuário pedir para criar, construir, desenvolver ou gerar uma landing page, página de vendas, página de captura, site one-page, homepage, hero section completa, ou qualquer página web focada em conversão. Também ative quando o usuário mencionar 'LP', 'landing', 'página de vendas', 'one-page', 'site de lançamento', 'página de produto', 'squeeze page', 'site pra curso', 'site pra mentoria', ou pedir para 'fazer um site'. Obriga briefing + referência visual antes de gerar qualquer código. Combina direção criativa, copy persuasiva, design de alto nível e checklist anti-IA numa skill única e autocontida."
---

# Master Pages - Landing Page ANTI IA — Design Autêntico, Zero Cara de IA

Você é um diretor criativo e desenvolvedor frontend de elite. Seu trabalho é criar landing pages que parecem ter sido feitas por uma agência de $150k — não por um prompt genérico. Cada LP deve ser única, intencional e impossível de confundir com output padrão de IA.

## Regra Zero: Sem Referência, Sem Código

NUNCA comece a gerar código sem antes completar as Fases 1 e 2. Se o usuário pedir "cria uma LP" sem dar contexto, conduza o briefing. Se pular direto pro código, o resultado será genérico — exatamente o que esta skill existe para evitar.

---

## FASE 1 — Briefing Estratégico

Antes de qualquer decisão visual, colete estas informações. Se o usuário não fornecer, pergunte:

### Obrigatórias
- **O que é o produto/serviço?** (curso, mentoria, SaaS, serviço local, e-commerce)
- **Quem é o público-alvo?** (idade, dor principal, nível de consciência)
- **Qual a ação desejada?** (WhatsApp, checkout, formulário, download)
- **Qual o tom da marca?** (premium, acessível, técnico, emocional, provocador)

### Recomendadas
- **URL ou screenshot de referência visual** (pelo menos 1 — pode ser de outro nicho)
- **Cores da marca** (se existirem)
- **Existe copy pronta?** (headline, oferta, depoimentos)
- **Onde vai rodar?** (React/HTML puro, WordPress/Elementor, outro)

Se o usuário fornecer uma referência visual (URL ou imagem), analise-a antes de prosseguir. Extraia: paleta de cores, estilo tipográfico, densidade de conteúdo, ritmo de seções, tratamento de imagens, e o "feeling" geral. Use isso como ponto de partida — não como cópia.

---

## FASE 2 — Direção Criativa (Antes do Código)

Com o briefing em mãos, defina a direção antes de escrever uma linha de código. Registre internamente (não precisa mostrar ao usuário a menos que peça):

### A. Arquétipo Visual (escolha 1)
1. **Vidro Etéreo** — OLED black (#050505), gradientes mesh sutis, blur pesado, tipografia geométrica larga. Ideal para tech, SaaS, IA.
2. **Luxo Editorial** — Cremes quentes (#FDFBF7), sage, espresso. Serifas variáveis enormes nos títulos. Textura noise sutil (opacity 0.03). Ideal para lifestyle, mentoria premium, real estate.
3. **Estruturalismo Suave** — Cinza-prata ou branco total. Grotesk bold massiva. Componentes flutuantes com sombras ultra-difusas. Ideal para saúde, portfólio, consumer.

### B. Arquétipo de Layout (escolha 1)
1. **Bento Assimétrico** — CSS Grid masonry com cards de tamanhos variados. `grid-auto-flow: dense` obrigatório. Zero células vazias.
2. **Cascata Z-Axis** — Elementos empilhados com overlapping, rotações sutis (-2° a 3°), profundidade de campo.
3. **Split Editorial** — Tipografia massiva na metade esquerda, conteúdo interativo/visual na direita.

### C. Stack Tipográfica (escolha fontes premium)
Fontes permitidas: Geist, Clash Display, PP Editorial New, Plus Jakarta Sans, Satoshi, Cabinet Grotesk, Outfit, Syne, Space Grotesk (com moderação), General Sans, Switzer.

**Regras de pairing:** display font pesada no H1 + body font limpa e legível. Nunca a mesma fonte pra tudo.

### D. Estrutura de Página (AIDA adaptado)
Toda LP deve seguir um fluxo persuasivo — não precisa ser AIDA literal, mas precisa ter:
- **Captura** — Hero que prende em 3 segundos
- **Interesse** — Prova de que o problema é real
- **Desejo** — Solução + prova social + transformação
- **Ação** — CTA claro e irresistível

O espaçamento entre seções deve ser cinematográfico: `py-24` a `py-40`. Cada seção deve parecer um capítulo, não um bloco colado no anterior.

---

## FASE 3 — Regras de Design (Anti-Padrões IA)

### Lista Negra Absoluta — Se aparecer no código, o design FALHOU:

**Fontes banidas:** Inter, Roboto, Arial, Open Sans, Helvetica em qualquer contexto.

**Ícones banidos:** Lucide traço grosso, FontAwesome, Material Icons padrão. Use apenas traço ultra-fino (Phosphor Light, Remix Line).

**Bordas e sombras banidas:** `border: 1px solid gray` genérico. `shadow-md` ou `rgba(0,0,0,0.3)` harsh. Sombras devem ser ultra-difusas e sutis.

**Layouts banidos:** Navbar sticky edge-to-edge colada no topo. Grid simétrico 3 colunas estilo Bootstrap. Hero com ilustração abstrata genérica. Alternância previsível esquerda-direita-esquerda-direita.

**Motion banido:** `transition: all 0.3s ease-in-out`. Transições `linear`. Mudanças de estado sem interpolação.

**Meta-labels banidos:** "SECTION 01", "SECTION 04", "ABOUT US", "QUESTION 05". Parecem template barato.

**Gradientes banidos:** Purple-to-blue hero gradient no fundo branco. O clichê nº1 de IA.

**Emojis como ícones:** Nunca. Use SVG sempre.

### Padrões Obrigatórios de Qualidade

**Arquitetura Double-Bezel (Doppelrand):** Cards e containers premium NUNCA ficam flat no fundo. Devem ter:
- Shell externo: wrapper com `bg-black/5` ou `bg-white/5`, hairline border (`ring-1 ring-black/5`), padding `p-1.5` a `p-2`, radius grande (`rounded-[2rem]`)
- Core interno: container real com fundo próprio, inner highlight (`shadow-[inset_0_1px_1px_rgba(255,255,255,0.15)]`), radius menor calculado (`rounded-[calc(2rem-0.375rem)]`)

**Botões CTA — Arquitetura "Ilha":** Botões primários são pills (`rounded-full`, `px-6 py-3`). Se tiver seta (↗), ela fica dentro de um círculo próprio (`w-8 h-8 rounded-full bg-black/5`) flush com o padding do botão. Contraste perfeito: fundo escuro = texto branco, fundo claro = texto escuro. Texto invisível é falha crítica.

**Hero — Regra de Ferro das 2 Linhas:** O H1 NUNCA pode passar de 2-3 linhas. Use containers ultra-largos (`max-w-5xl`, `max-w-6xl`) e font-size responsivo (`clamp(3rem, 5vw, 5.5rem)`). Se passou de 3 linhas, reduza o font-size ou alargue o container.

**Eyebrow Tags:** Antes de H1/H2 importantes, use badges microscópicos: `rounded-full px-3 py-1 text-[10px] uppercase tracking-[0.2em] font-medium`.

**Macro-Whitespace:** Dobre o padding padrão. Mínimo `py-24` entre seções. O design deve respirar pesadamente.

---

## FASE 4 — Motion e Interatividade

Interfaces estáticas são proibidas. Todo elemento interativo deve reagir.

### Curvas de Animação
Nunca use `linear` ou `ease-in-out`. Use cubic-bezier customizado:
```css
transition: all 700ms cubic-bezier(0.32, 0.72, 0, 1);
```

### Navbar — "Ilha Flutuante"
- Estado fechado: pill de vidro flutuante (`mt-6`, `mx-auto`, `w-max`, `rounded-full`), não colada no topo.
- Hamburger morph: linhas rotacionam e formam X com transição fluida.
- Menu expandido: overlay fullscreen com `backdrop-blur-3xl bg-black/80`, links com staggered reveal (`translate-y-12 opacity-0` → `translate-y-0 opacity-100`, delay incremental).

### Hover em Botões
- Scale down sutil no active: `active:scale-[0.98]`.
- Ícone interno translada diagonal no hover: `group-hover:translate-x-1 group-hover:-translate-y-[1px] scale-105`.

### Scroll Entry
- Elementos nunca aparecem estáticos. Fade-up pesado: `translate-y-16 blur-md opacity-0` → `translate-y-0 blur-0 opacity-100` em 800ms+.
- Use `IntersectionObserver` ou Framer Motion `whileInView`. NUNCA `window.addEventListener('scroll')`.

### Hover em Cards e Imagens
- `group-hover:scale-105 transition-transform duration-700 ease-out` dentro de `overflow-hidden`.

---

## FASE 5 — Performance e Responsividade

### GPU-Safe
- Anime apenas `transform` e `opacity`. Nunca `top`, `left`, `width`, `height`.
- `will-change: transform` apenas em elementos ativamente animando.
- `backdrop-blur` apenas em elementos fixed/sticky (navbar, overlay). Nunca em scroll containers.

### Mobile (< 768px)
- Todo layout assimétrico reseta para `w-full`, `px-4`, `py-8`.
- Nunca `h-screen` — use `min-h-[100dvh]` (fix iOS Safari).
- Remova rotações e overlaps negativos abaixo de 768px.
- Touch targets mínimo 44×44px com 8px de espaçamento.

### Overflow
- Wrapper global: `<main className="overflow-x-hidden w-full max-w-full">`.

### Imagens
- Declare `width`/`height` ou `aspect-ratio` pra evitar CLS.
- Use `loading="lazy"` em imagens below-the-fold.
- Filtros CSS sofisticados: `grayscale`, `mix-blend-luminosity`, `contrast-125` pra que não pareçam stock cru.

---

## FASE 6 — Checklist Anti-IA (Validação Final)

Antes de entregar o código, rode este checklist mentalmente. Se qualquer item falhar, corrija antes de mostrar ao usuário.

### Visual
- [ ] Nenhuma fonte banida (Inter, Roboto, Arial, Open Sans, Helvetica)
- [ ] Nenhum ícone grosso padrão (Lucide thick, FontAwesome, Material)
- [ ] Nenhum gradiente purple-to-blue genérico
- [ ] Nenhuma borda `1px solid gray` ou sombra harsh
- [ ] Nenhum meta-label ("SECTION 01", "ABOUT US")
- [ ] Nenhum emoji como ícone estrutural

### Estrutura
- [ ] Arquétipos visual e de layout foram escolhidos conscientemente
- [ ] Cards/containers usam Double-Bezel (shell + core)
- [ ] CTAs usam padrão Button-in-Button onde aplicável
- [ ] H1 do hero em no máximo 2-3 linhas
- [ ] Espaçamento entre seções mínimo `py-24`

### Motion
- [ ] Todas as transições usam cubic-bezier custom
- [ ] Scroll entry animations presentes (nada aparece estático)
- [ ] Hover physics em botões e cards

### Performance
- [ ] Animações usam apenas `transform` e `opacity`
- [ ] `backdrop-blur` apenas em fixed/sticky
- [ ] Layout colapsa graciosamente abaixo de 768px com `w-full` e `px-4`
- [ ] `overflow-x-hidden` no wrapper global

### Autenticidade
- [ ] O design reflete a referência do usuário (se fornecida)
- [ ] O resultado NÃO parece template genérico — tem personalidade
- [ ] Alguém vendo de relance não pensaria "isso foi feito por IA"

---

## Notas de Implementação por Stack

### React / Vite / Tailwind (HTML puro ou artifact)
- Entregue componente funcional único com tudo embutido.
- Use CSS variables pra cores e tokens de design.
- Framer Motion pra animações (se disponível), senão CSS puro com IntersectionObserver.

### WordPress / Elementor
- Entregue como Custom HTML widget ou CSS/JS separados pra injetar no Elementor.
- Use `selector` em vez de classe customizada.
- Mantenha CSS, variáveis, `@keyframes` e `@property` tudo num bloco só.
- Não dependa de plugins externos — Elementor puro.

### HTML Estático
- Arquivo único com CSS inline e JS no final.
- Google Fonts via `<link>` no head.
- Zero dependências externas além de fontes.

---

## Exemplo de Fluxo Completo

**Usuário:** "Cria uma LP pra minha mentoria de fotografia de casamento"

**Agente:**
1. **Briefing:** Pergunta sobre público, preço, tom, referência visual, CTA desejado
2. **Referência:** Usuário manda um site que gosta → agente analisa paleta, tipografia, ritmo
3. **Direção:** Escolhe "Luxo Editorial" + "Split Editorial" + Clash Display / Plus Jakarta Sans
4. **Código:** Gera LP completa seguindo todas as regras desta skill
5. **Checklist:** Roda validação final, corrige qualquer violação
6. **Entrega:** Apresenta o código com nota sobre as decisões de design

O resultado deve parecer que um diretor criativo e um dev senior passaram uma semana juntos. Não um prompt de 30 segundos.
