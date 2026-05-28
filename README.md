# Master Landing Page Skill

Skill para Claude Code que cria landing pages premium com design autêntico — sem cara de IA.

Consolida regras de design de alto nível, anti-padrões de IA, copy persuasiva, motion choreography, e checklist de qualidade num único `SKILL.md` autocontido. Nenhuma dependência externa necessária.

## O que faz

- **Bloqueia padrões genéricos de IA** — lista negra de fontes (Inter, Roboto), layouts (grid 3-col Bootstrap), gradientes (purple-to-blue), meta-labels ("SECTION 01")
- **Obriga briefing antes do código** — sem referência visual, sem geração
- **Define arquétipos visuais** — Vidro Etéreo, Luxo Editorial, Estruturalismo Suave
- **Aplica design de agência $150k** — Double-Bezel, Button-in-Button, Navbar Ilha Flutuante
- **Motion premium** — cubic-bezier custom, scroll entry, hover physics
- **Checklist final anti-IA** — validação automática antes da entrega

## Instalação

### Via npx (recomendado)

```bash
npx skills add marlonr-design/master-landing-page --agent claude-code --yes
```

### Instalação global (disponível em todos os projetos)

```bash
npx skills add marlonr-design/master-landing-page --agent claude-code --yes -g
```

### Manual

```bash
# Clonar direto pra pasta de skills do Claude Code
mkdir -p ~/.claude/skills/master-landing-page
curl -o ~/.claude/skills/master-landing-page/SKILL.md \
  https://raw.githubusercontent.com/marlonr-design/master-landing-page/main/master-landing-page/SKILL.md
```

> Após instalar, reinicie o Claude Code para carregar a skill.

## Como usar

Basta pedir ao Claude Code para criar uma landing page:

```
Cria uma landing page pra minha mentoria de fotografia
```

```
Faz uma LP pra um curso de copywriting, tom premium, público mulheres 25-40
```

```
Quero uma página de vendas pro meu SaaS de gestão financeira
```

A skill vai automaticamente:

1. **Conduzir um briefing** — produto, público, tom, referência visual
2. **Definir direção criativa** — arquétipo visual, layout, tipografia
3. **Gerar o código** — seguindo todas as regras anti-IA
4. **Validar com checklist** — conferir se nenhum padrão genérico passou

## Compatibilidade

| Stack | Suporte |
|-------|---------|
| React / Vite / Tailwind | ✅ Completo |
| HTML estático | ✅ Completo |
| WordPress / Elementor | ✅ Completo |

## Regras que essa skill aplica

<details>
<summary>Lista negra (o que é bloqueado)</summary>

- Fontes: Inter, Roboto, Arial, Open Sans, Helvetica
- Ícones: Lucide traço grosso, FontAwesome, Material Icons
- Layouts: Navbar sticky edge-to-edge, grid simétrico 3-col, alternância esquerda-direita
- Motion: `ease-in-out`, `linear`, transições sem interpolação
- Visual: Gradiente purple-to-blue, `1px solid gray`, `shadow-md`, emojis como ícones
- Labels: "SECTION 01", "ABOUT US", "QUESTION 05"

</details>

<details>
<summary>Padrões obrigatórios</summary>

- Double-Bezel (Doppelrand) em cards e containers
- Button-in-Button com trailing icon
- Hero com máximo 2-3 linhas no H1
- Macro-whitespace: mínimo `py-24` entre seções
- Navbar Ilha Flutuante (não colada no topo)
- Cubic-bezier custom em todas as transições
- Scroll entry animations (nada aparece estático)
- Mobile-first com colapso gracioso abaixo de 768px

</details>

## Créditos

Baseada em regras consolidadas de skills de design premium da comunidade, incluindo princípios de:
- Design de agência de alto nível (Double-Bezel, motion choreography)
- UI/UX profissional (acessibilidade, performance, responsividade)
- Anti-padrões de IA generativa (variância obrigatória, ban de defaults)

## Licença

MIT — use, modifique e distribua livremente.
