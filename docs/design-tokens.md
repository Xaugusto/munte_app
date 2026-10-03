# 🎨 Tokens de Design — Caronas UTFPR

**Projeto:** Caronas UTFPR
**Versão:** 1.0.0
**Última atualização:** 2026-10-03

> Fonte da verdade para Tailwind (`tailwind.config.js`), Stitch, Figma e código.
> Não edite à mão — gere via `/utf-design` quando houver mudanças.

---

## Paleta (Semântica)

| Token | Light (Hex) | Dark (Hex) | Onde se usa |
|-------|-------------|------------|-------------|
| `primary` | `#0066CC` | `#3B82F6` | Botões primários, links ativos, chips de seleção, ícones de ação principal |
| `primary-hover` | `#0052A3` | `#60A5FA` | Hover/foco de botões primários |
| `surface` | `#FFFFFF` | `#1E293B` | Fundo de cards, modais, sheets, bottom sheets |
| `background` | `#F8FAFC` | `#0F172A` | Fundo geral das telas |
| `text` | `#0F172A` | `#F8FAFC` | Texto principal (títulos, corpo) |
| `text-muted` | `#64748B` | `#94A3B8` | Legendas, placeholders, contadores, textos de apoio |
| `border` | `#E2E8F0` | `#334155` | Divisórias, bordas de inputs/cards, separadores |
| `danger` | `#DC2626` | `#EF4444` | Erros, exclusão, cancelamento tardio, botões destrutivos |
| `danger-hover` | `#B91C1C` | `#F87171` | Hover/foco de ações perigosas |
| `success` | `#16A34A` | `#22C55E` | Confirmações, aceite, vagas disponíveis, chips de sucesso |
| `success-hover` | `#15803D` | `#4ADE80` | Hover/foco de ações de sucesso |
| `warning` | `#D97706` | `#FBBF24` | Alertas de atenção (ex: <30min para partida) |
| `disabled` | `#CBD5E1` | `#475569` | Controles desabilitados, placeholders inativos |
| `disabled-text` | `#94A3B8` | `#64748B` | Texto em controles desabilitados |

---

## Escala de Espaçamento (base 4px — Tailwind default)

| Token | Valor (rem) | px | Uso típico |
|-------|-------------|-----|------------|
| `xs` | `0.5rem` | 8px | Gap interno pequeno (chips, badges, ícones + texto) |
| `sm` | `0.75rem` | 12px | Padding de inputs, gap entre itens de lista |
| `md` | `1rem` | 16px | Padding padrão de cards, gap entre seções |
| `lg` | `1.5rem` | 24px | Padding de containers, gap entre blocos grandes |
| `xl` | `2rem` | 32px | Padding de tela (mobile), margens de seções |
| `2xl` | `3rem` | 48px | Padding de tela (desktop), hero sections |

---

## Tipografia (Sistema nativo — sem fonte customizada no MVP)

| Token | Família | Tamanho (rem) | Peso | Line-height | Papel |
|-------|---------|---------------|------|-------------|-------|
| `display-lg` | `system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif` | `2.25rem` (36px) | 700 | 1.1 | Título de tela (raro) |
| `display-md` | same | `1.875rem` (30px) | 700 | 1.2 | Título de seção principal |
| `heading-lg` | same | `1.5rem` (24px) | 600 | 1.3 | Título de card, modal |
| `heading-md` | same | `1.25rem` (20px) | 600 | 1.3 | Subtítulo, label de grupo |
| `body-lg` | same | `1.125rem` (18px) | 400 | 1.5 | Texto corrido importante |
| `body` | same | `1rem` (16px) | 400 | 1.5 | Texto padrão |
| `body-sm` | same | `0.875rem` (14px) | 400 | 1.5 | Texto secundário, ajuda |
| `caption` | same | `0.75rem` (12px) | 500 | 1.4 | Chips, badges, timestamps, contadores |
| `button` | same | `0.875rem` (14px) | 600 | 1.25 | Texto de botões |

---

## Raio de Borda

| Token | Valor | Uso |
|-------|-------|-----|
| `none` | `0` | Botões ghost, badges quadrados |
| `sm` | `0.25rem` (4px) | Chips, tags, inputs compactos |
| `md` | `0.5rem` (8px) | **Padrão**: botões, cards, modais, sheets |
| `lg` | `0.75rem` (12px) | Bottom sheets, modais grandes |
| `full` | `9999px` | Pills, avatares, botões circulares |

---

## Sombras (Elevation)

| Token | Valor (Tailwind) | Uso |
|-------|------------------|-----|
| `flat` | `none` | Cards flush, divs internos |
| `card` | `0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1)` | Cards padrão, list items |
| `elevated` | `0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1)` | Modais, bottom sheets, dropdowns |
| `modal` | `0 25px 50px -12px rgb(0 0 0 / 0.25)` | Modal full-screen, drawers |

---

## Estados de Botão (Tailwind-ready)

| Estado | Aparência (Light) | Aparência (Dark) |
|--------|-------------------|------------------|
| `default` | `bg-primary text-white` | `bg-primary text-white` |
| `hover` | `bg-primary-hover` | `bg-primary-hover` |
| `focus` | `ring-2 ring-primary/50` | `ring-2 ring-primary/50` |
| `active` | `bg-primary-hover scale-[0.98]` | `bg-primary-hover scale-[0.98]` |
| `disabled` | `bg-disabled text-disabled-text cursor-not-allowed` | `bg-disabled text-disabled-text cursor-not-allowed` |
| `loading` | `relative animate-pulse` + spinner | `relative animate-pulse` + spinner |

**Variantes:**
- `secondary`: `bg-surface border border-border text-text` / hover `bg-gray-100` (dark: `bg-gray-800`)
- `ghost`: `text-primary` / hover `bg-primary/10`
- `danger`: `bg-danger text-white` / hover `bg-danger-hover`
- `success`: `bg-success text-white` / hover `bg-success-hover`

---

## Breakpoints (Mobile-First)

| Token | Largura mínima | Dispositivo alvo |
|-------|----------------|------------------|
| `sm` | `640px` | Celular grande / pequeno tablet |
| `md` | `768px` | Tablet retrato |
| `lg` | `1024px` | Tablet paisagem / notebook pequeno |
| `xl` | `1280px` | Desktop |
| `2xl` | `1536px` | Desktop largo |

> **Regra:** Toda tela nasce mobile (`< sm`). Use `sm:`, `md:`, `lg:` para expandir layout (grid, flex-direction, padding).

---

## Identidade PWA (para `manifest.webmanifest`)

| Campo | Valor |
|-------|-------|
| `short_name` | `Caronas` |
| `name` | `Caronas UTFPR` |
| `theme_color` | `#0066CC` |
| `background_color` | `#F8FAFC` |
| `display` | `standalone` |
| `orientation` | `portrait-primary` |
| `scope` | `/` |
| `start_url` | `/?source=pwa` |
| `icons` | `icons/icon-192.png` (192×192), `icons/icon-512.png` (512×512) — máscara `purpose: any maskable` |
| Comportamento offline | Tela "Você está offline" com botão "Tentar novamente"; Minhas Caronas e último sino visíveis em cache |

---

## Componentes-chave (para Mapa de Componentes no Figma)

| Componente Angular | Token(s) principais | Descrição |
|--------------------|---------------------|-----------|
| `<app-header>` | `surface`, `border`, `text`, `primary` | Topo fixo: título, sino, avatar |
| `<app-bottom-nav>` / `<app-sidebar>` | `surface`, `border`, `primary`, `text-muted` | Navegação principal (3 abas + perfil) |
| `<app-offer-card>` | `surface`, `border`, `text`, `success`/`danger`, `primary` | Card de oferta na busca e gestão |
| `<app-ride-card>` | `surface`, `border`, `text`, `primary` | Card em Minhas Caronas (com contato) |
| `<app-notification-item>` | `surface`, `text`, `text-muted`, `primary` | Linha no dropdown do sino |
| `<app-step-form>` | `surface`, `border`, `primary`, `text` | Wizard criar oferta (steps) |
| `<app-bairro-select>` | `surface`, `border`, `text`, `primary` | Dropdown 23 bairros → 3 pontos |
| `<app-empty-state>` | `surface`, `text-muted`, `primary` | Ilustração + texto + CTA |
| `<app-toast>` | `success`/`danger`/`warning`, `text-white` | Feedback global |
| `<app-modal>` / `<app-bottom-sheet>` | `surface`, `shadow-modal`, `primary` | Confirmações, formulários |

---

## Protótipo (Stitch/Figma)

**Link:** [inserir link público do Stitch/Figma após gerar]
**Telas cobertas:**
1. Login UTFApps
2. Home / Dashboard (estado vazio + atalhos)
3. Criar Oferta (3 steps)
4. Buscar Caronas (abas Ida/Volta + filtro bairro)
5. Detalhe Oferta + Solicitação
6. Minhas Solicitações / Gestão (Motorista)
7. Minhas Caronas (Ativas + Histórico)
8. Central de Notificações (Sino)
**Responsividade:** Mobile (375px) + Desktop (1440px) para cada tela
**Navegação:** Protótipo clicável configurado