# Especificação visual implementável

## Fonte de verdade e escopo

Esta especificação traduz para valores implementáveis o design aprovado no
Google Stitch:

- projeto: `14810906810027389425`;
- desktop: `5e306be84dcc4a9399533afb6e2962e0`;
- mobile: `9fd03e0befd54fa9ae462187f465091e`;
- design system: `Atelier Editorial — Petroleum & Amber`;
- asset do design system: `7822681292574026971`.

O design é light-only. As classes de dark mode presentes no HTML exportado pelo
Stitch não representam uma variante aprovada e não devem motivar um seletor de
tema nesta implementação.

## Princípios visuais

- aparência editorial e de boutique technical consultancy;
- tipografia como elemento visual principal;
- alto contraste e leitura confortável;
- whitespace generoso;
- estrutura expressa por grid e linhas de 1px;
- sombras apenas muito sutis para separar cards claros do fundo marfim;
- ausência de gradientes, glow, glassmorphism e estética de terminal;
- tecnologia apresentada com sobriedade, depois da narrativa comercial;
- cantos discretamente arredondados, sem aparência de pills.

## Estrutura da página

```text
body
├── sticky header
├── main
│   ├── hero / value proposition
│   ├── selected work
│   ├── capabilities
│   ├── studio philosophy
│   ├── process
│   ├── foundation
│   ├── about
│   └── final CTA
└── footer
    ├── brand, location and links
    └── language and copyright
```

Todas as seções, exceto o CTA final, usam uma base clara e uma borda inferior de
1px. `Studio Philosophy` usa uma superfície azulada suave. O CTA final usa fundo
azul-petróleo escuro em largura total.

## Container, grid e breakpoints

### Container principal

- `max-width: 1280px` (`max-w-7xl`);
- centralizado com `margin-inline: auto`;
- padding horizontal mobile: `20px`;
- padding horizontal a partir de `768px`: `48px`;
- altura do header: `64px`.

### Breakpoints

Usar os breakpoints padrão do Tailwind:

- `sm`: `640px`;
- `md`: `768px`;
- `lg`: `1024px`;
- `xl`: `1280px`.

### Grid desktop

- grid estrutural de 12 colunas quando necessário;
- gap principal: `48px`;
- hero: narrativa `8/12`, practice index `4/12`;
- cases: texto `6/12`, imagem e metadata `6/12`;
- about: retrato `4/12`, narrativa `8/12`;
- capabilities: `2` colunas;
- studio philosophy: `3` colunas;
- process: `4` colunas;
- foundation: `3` colunas.

### Grid intermediário

Entre `768px` e `1023px`:

- capabilities: `2` colunas;
- process: `2` colunas;
- foundation: `2` colunas;
- proof strip: `4` colunas;
- hero, cases e about permanecem empilhados até `1024px`.

### Grid mobile

Abaixo de `768px`:

- conteúdo principal em uma coluna;
- cards e etapas empilhados;
- metadata dos cases e proof strip em `2` colunas;
- CTAs principais empilhados e ocupando a largura disponível;
- screenshots de case em proporção `16:10`;
- retrato em proporção `4:5`.

A captura mobile do Stitch tem `780px` físicos e representa aproximadamente um
viewport CSS de `390px` em densidade 2x.

## Escala de espaçamento

| Token | Valor | Uso principal |
| --- | ---: | --- |
| `space-xs` | `4px` | micro gaps, ícone/texto |
| `space-sm` | `8px` | labels, gaps compactos |
| `space-md` | `16px` | padding interno padrão e separadores |
| `space-lg` | `24px` | cards, botões e gaps de grid |
| `space-xl` | `48px` | seções mobile e headers de seção |
| `space-2xl` | `80px` | seções desktop e distância entre cases |
| `margin-mobile` | `20px` | margem lateral mobile |
| `margin` | `48px` | margem lateral desktop |

### Regras de seção

- padding vertical mobile: `48px`;
- padding vertical a partir de `768px`: `80px`;
- cabeçalho de seção: `padding-bottom: 24px`;
- distância após cabeçalho de seção: `48px`;
- espaço entre os dois cases: `80px`;
- gap comum entre cards independentes: `24px`.

## Tipografia

### Família

- primária: `Geist, sans-serif`;
- pesos carregados: `300`, `400`, `500`, `600`, `700`;
- não usar fonte monoespaçada;
- labels técnicos continuam em Geist, uppercase e com tracking amplo.

### Escala tipográfica

| Papel | Desktop | Mobile | Peso | Line-height | Letter-spacing |
| --- | ---: | ---: | ---: | ---: | ---: |
| Display / hero / CTA | `64px` | `38px` | `400` | `72px` / `44px` | `-0.03em` / `-0.02em` |
| Heading de seção | `40px` | `28px` | `500` | `48px` / `34px` | `-0.025em` / `-0.015em` |
| Heading médio | `24px` | `24px` | `500` | `32px` | `-0.015em` |
| Heading pequeno/card | `18px` | `18px` | `600` | `24px` | `-0.01em` |
| Body grande | `17px` | `17px` | `400` | `28px` | `-0.005em` |
| Body padrão | `15px` | `15px` | `400` | `24px` | `0` |
| Body pequeno | `13px` | `13px` | `400` | `20px` | `0.005em` |
| Label caps | `11px` | `11px` | `500` | `16px` | `0.08em` |

### Uso

- H1 e headline do CTA final: Display;
- H2 de seção: Heading de seção;
- títulos de cases e lead do About: Heading médio;
- títulos de cards: Heading pequeno;
- parágrafo principal do hero e About: Body grande;
- descrições de capabilities e princípios: Body padrão;
- listas técnicas e etapas do processo: Body pequeno;
- índices, eyebrows, metadata e navegação: Label caps ou `12px` uppercase
  com `letter-spacing: 0.08em`.

### Comprimento de linha

- H1: `max-width: 896px`;
- supporting copy do hero e CTA: `max-width: 672px`;
- lead de seções: entre `768px` e `896px`;
- body editorial: preferir `60–72ch` quando não limitado pelo grid.

## Cores

### Tokens usados diretamente

| Token | Hex | Uso |
| --- | --- | --- |
| `surface` / `background` | `#F7F3EA` | fundo principal |
| `surface-lowest` | `#FFFFFF` | cards e painéis |
| `surface-low` | `#EAF1EF` | áreas secundárias e hover |
| `surface-container` | `#DDE8E5` | superfície intermediária |
| `surface-high` | `#D8E5E2` | superfície elevada sem sombra |
| `surface-highest` | `#CBD8D4` | bordas e divisórias claras |
| `primary` | `#102f35` | headline, botão primário e CTA final |
| `on-surface` | `#102F35` | texto principal |
| `on-surface-variant` | `#4b6064` | body secundário |
| `outline` | `#70898a` | metadata e bordas escuras |
| `outline-variant` | `#B6C8C4` | ícones e separadores secundários |
| `secondary` | `#925B08` | destaque âmbar acessível para labels e links |
| `secondary-container` | `#F7E9C7` | destaque âmbar suave e hover sobre fundo escuro |
| `secondary-fixed-dim` | `#E7C57C` | variação âmbar intermediária |
| `primary-fixed-dim` | `#D5E0DD` | copy no CTA escuro |
| `inverse-surface` | `#2E5960` | divisor interno no CTA escuro |
| `primary-container` | `#0B333C` | fallback escuro, não um tema separado |

### Aplicação

- usar o azul-petróleo como cor estrutural dominante e manter a maior parte da
  página em superfícies marfim ou azuladas suaves;
- reservar `#925B08` para eyebrows, estados ativos, ícones pequenos e hover;
- não criar gradientes nem grandes blocos âmbar saturados;
- seleção de texto: fundo `#F7E9C7`, texto `#4a2c00`;
- validar contraste WCAG AA para qualquer combinação diferente das aprovadas.

## Bordas, radius e elevação

- borda padrão: `1px solid #CBD8D4`;
- borda escura no CTA: `1px solid #70898a`;
- cards podem usar somente uma sombra de baixa opacidade (`0 1px 2px`);
- cards, painéis, imagens e grids externos: `border-radius: 8px`;
- botões: `border-radius: 6px`;
- badges compactos: `border-radius: 4px`;
- status dot do hero: `8px × 8px` e `border-radius: 9999px`.

## Navegação

### Desktop e tablet (`>= 768px`)

- header sticky em `top: 0`, `z-index: 50`;
- fundo `#F7F3EA` e borda inferior de 1px;
- altura `64px`;
- wordmark à esquerda;
- links centrais em `11px`, uppercase;
- link ativo `Work` com underline/borda inferior de 1px;
- seletor de idioma e CTA outlined à direita.

### Mobile (`< 768px`)

- links de âncora ficam ocultos;
- wordmark reduzido para `16px`;
- descriptor `Independent Software Studio` fica oculto abaixo de `640px`;
- permanecem `PT` e um CTA compacto `Start a conversation`;
- o design aprovado não contém menu drawer ou hamburger.

O seletor de idioma deve ser um link real, não um botão inerte.

## Botões e links

### Botão primário claro

- background: `#102f35`;
- texto: `#FFFFFF`;
- font-size: `15px`;
- padding: `12px 24px`;
- border-radius: `6px`;
- hover: background `#925B08`;
- transição: `color/background 150ms`;
- ícone de seta: `16px`, deslocamento horizontal de `2px` no hover.

### Botão outlined

- fundo transparente;
- borda: `1px solid #102f35`;
- texto: `#102f35`;
- padding desktop: `8px 16px`;
- hover: background `#EAF1EF`;
- border-radius: `6px`.

### Botão do CTA escuro

- background: `#FFFFFF`;
- texto: `#102f35`;
- padding: `14px 24px`;
- hover: background `#F7E9C7`.

### Links editoriais

- underline de `1px`;
- `text-underline-offset: 4px`;
- cor padrão conforme contexto;
- hover em `#925B08` sobre fundo claro;
- transição: `150ms`.

### Focus

O Stitch não define focus visual explicitamente. A implementação deve adicionar:

```css
outline: 2px solid #925b08;
outline-offset: 2px;
```

Aplicar em links, botões e qualquer controle via `:focus-visible`. Não remover o
outline nativo sem substituição equivalente.

Em mobile, controles interativos devem ter área mínima de `44px × 44px`, mesmo
quando o desenho visual interno for mais compacto.

## Cards e padrões de conteúdo

### Practice index

- painel branco com borda de 1px;
- header interno com `24px` de padding;
- linhas com `16px` de padding;
- linhas separadas por divisórias de 1px;
- hover da linha: `#EAF1EF` em `150ms`;
- ícone `18px` alinhado ao topo/direita.

### Case study

- container branco com borda de 1px;
- desktop: split `50/50`;
- coluna narrativa: `48px` de padding em `>=768px`, `24px` abaixo;
- coluna visual: fundo `#EAF1EF`, padding `24px`;
- screenshot desktop: `width: 100%`, `height: 288px`, `object-fit: cover`;
- screenshot mobile: `aspect-ratio: 16 / 10`;
- metadata: 4 colunas no desktop, 2 no mobile;
- radius externo de `8px` e sombra de separação quase imperceptível.

### Capability grid

- 2 colunas em `>=768px`, 1 coluna abaixo;
- grid desenhado por bordas compartilhadas;
- padding por item: `24px` mobile e `48px` a partir de `768px`;
- hover: fundo de `#FFFFFF` para `#EAF1EF` em `150ms`.

### Principle cards

- 3 colunas em `>=768px`, 1 coluna abaixo;
- gap `24px`;
- padding `24px`;
- header e footer internos separados por borda de 1px;
- altura igual dentro da mesma linha via flex.

### Process steps

- 4 colunas em `>=1024px`, 2 em `>=768px`, 1 abaixo;
- células contíguas com bordas compartilhadas;
- padding `24px`;
- label da fase no rodapé da célula.

### Foundation cards

- 3 colunas em `>=1024px`, 2 em `>=768px`, 1 abaixo;
- gap `24px`;
- padding `24px`;
- listas em `13px/20px`;
- sem logos de tecnologia.

### Proof strip

- 4 colunas em `>=768px`, 2 abaixo;
- bordas compartilhadas;
- padding `16px`;
- valor em `18px/24px`;
- label e descrição em uppercase pequeno.

## Ícones

- estilo visual: outline, geométrico e discreto;
- tamanhos aprovados: `14px`, `16px` e `18px`;
- usos: seta externa, seta de CTA, check, engenharia, velocidade, dataset,
  layers, API e email;
- ícones decorativos devem usar `aria-hidden="true"`;
- botões icon-only precisam de `aria-label`;
- Material Symbols Outlined é a fonte usada no protótipo, mas a implementação
  pode reutilizar SVGs inline/localmente para evitar uma nova dependência, desde
  que mantenha forma, peso e tamanho equivalentes.

## Imagens

### Retrato

- proporção: `4:5`;
- `object-fit: cover`;
- grayscale;
- contraste visual equivalente a `contrast(1.25)`;
- borda externa e borda da imagem de 1px;
- padding do frame: `8px`;
- metadata inferior com nome e localização.

O Stitch usa um retrato gerado como placeholder. A implementação deve usar
`img/perfil_social_bw.webp`, com crop equivalente, salvo se um novo retrato real
for aprovado.

### Cases

O Stitch usa imagens conceituais geradas para MDC e CDC. Elas não são assets de
produção e não devem ser hotlinked. Antes da implementação final, produzir
screenshots reais e sanitizados dos projetos, mantendo:

- enquadramento horizontal `16:10` no mobile;
- altura de `288px` no desktop;
- aparência neutra;
- borda de 1px;
- nenhum dado privado ou identificável.

### Assets atuais

- `img/perfil_social_bw.webp`: candidato para o retrato;
- `img/og-image.jpg`: deve ser revisado para o novo posicionamento;
- `img/skills.png`: não faz parte do design aprovado;
- `img/favicon.ico`: preservar até existir substituição aprovada.

## Comportamento responsivo detalhado

### Desktop

- hero em 8/4 colunas;
- cases em split horizontal;
- maior uso de whitespace vertical (`80px`);
- grids de 2, 3 ou 4 colunas conforme a seção;
- navegação completa visível.

### Mobile

- ordem do conteúdo permanece idêntica;
- hero narrativo antes do practice index;
- CTAs empilhados;
- cases: texto antes da imagem e metadata;
- capabilities, principles, process e foundation em uma coluna;
- metadata e proof strip em duas colunas;
- About: retrato antes da narrativa;
- CTA final: botão principal centralizado no próprio controle;
- footer em coluna, com links quebrando linha;
- padding lateral `20px` e vertical de seção `48px`.

### Diferenças específicas entre os exports aprovados

- no export desktop, o CTA do header fica oculto abaixo de `640px`;
- no export mobile, existe uma variante compacta do mesmo CTA visível em telas
  pequenas;
- para implementação, prevalece a tela mobile aprovada: mostrar o CTA compacto.

## Estados de interação

- duração padrão: `150ms`;
- easing: usar `ease`/padrão do Tailwind;
- cards interativos: mudança de fundo, sem movimento vertical;
- links: mudança para `#925B08`;
- botão primário: azul-petróleo → âmbar escuro;
- botão claro no CTA: branco → âmbar claro;
- seta do CTA: deslocamento de `2px` no eixo X;
- nenhuma sombra, escala ou glow no hover;
- respeitar `prefers-reduced-motion: reduce` e remover deslocamentos/transições
  não essenciais.

## Componentes reutilizáveis

Os nomes abaixo descrevem padrões, não exigem framework JavaScript:

- `SiteHeader`
- `Wordmark`
- `LanguageSwitch`
- `SectionContainer`
- `SectionHeader`
- `IndexLabel`
- `PrimaryButton`
- `OutlineButton`
- `EditorialLink`
- `PracticeIndex`
- `PracticeIndexRow`
- `CaseStudy`
- `CaseMetadataGrid`
- `CapabilityCell`
- `PrincipleCard`
- `ProcessStep`
- `FoundationCard`
- `PortraitBlock`
- `ProofStat`
- `FinalCTA`
- `SiteFooter`

Cada padrão deve manter a mesma escala tipográfica, bordas, spacing e estados em
inglês e português. A mudança de idioma não deve alterar a ordem das seções.

## Acessibilidade

- manter HTML semântico: `header`, `nav`, `main`, `section`, `article`, `footer`;
- um único `h1` por página;
- headings em ordem lógica;
- adicionar `aria-labelledby` às seções quando útil;
- preservar `lang="en"` e `lang="pt-BR"` nas páginas correspondentes;
- alt text deve descrever o conteúdo real da imagem, não o prompt do Stitch;
- links externos com `rel="noopener noreferrer"`;
- indicadores de foco conforme especificado;
- área interativa mínima de 44px no mobile;
- não depender apenas da cor para indicar estado ativo;
- usar `aria-hidden="true"` em ícones decorativos.

## URLs e integrações que devem ser preservadas

- analytics: Google tag `G-Z6QQHCDGT0`;
- canonical EN: `https://www.pcampos.com.br/`;
- canonical PT-BR: `https://www.pcampos.com.br/pt/`;
- email: `mailto:contato@pcampos.com.br`;
- LinkedIn: `https://linkedin.com/in/pcampos119104`;
- GitHub: `https://github.com/pcampos119104`;
- MDC: `https://github.com/pcampos119104/mdc`;
- CDC: `https://github.com/pcampos119104/cdc`;
- sitemap e alternate languages existentes;
- structured data deve ser revisado para representar studio founder-led sem
  perder a entidade `Person` de Pedro.

## Inconsistências e decisões pendentes

1. **Imagens dos cases:** o Stitch usa imagens geradas; o repositório não possui
   screenshots reais de MDC e CDC.
2. **Retrato:** o Stitch usa um retrato gerado diferente de
   `img/perfil_social_bw.webp`.
3. **Links sociais:** o export do Stitch aponta para homepages genéricas; usar as
   URLs reais listadas acima.
4. **Idioma:** o controle do Stitch não navega; usar `/` e `/pt/`.
5. **Navegação mobile:** não existe menu para as âncoras, apenas idioma e CTA.
   Isso é fiel ao aprovado, mas reduz a navegação interna.
6. **Touch target do header:** o CTA compacto do protótipo é visualmente menor
   que 44px; a implementação deve aumentar a área clicável.
7. **Focus:** não foi desenhado no Stitch; esta especificação adiciona o estado
   necessário para acessibilidade.
8. **Conteúdo factual:** datas e descrições de problemas dos cases têm pendências
   listadas em `CONTENT.md`.
9. **Paleta interna do Stitch:** o novo design system usa azul-petróleo como cor
   estrutural e âmbar como destaque, conforme os tokens documentados acima.
10. **Dark mode:** existem classes dark no export, mas nenhuma versão dark foi
    aprovada; não faz parte do escopo.
11. **Favicon:** o asset existente está em `img/favicon.ico`, enquanto os HTMLs
    atuais referenciam `favicon.ico` na raiz. O caminho deve ser corrigido na
    futura implementação, sem alterar o asset nesta etapa.
