# Arquitetura de conteúdo da homepage

## Fonte de verdade

O conteúdo abaixo foi extraído da tela desktop aprovada no Google Stitch:

- projeto: `14810906810027389425`;
- tela desktop aprovada: `a4de20ddce1048fa90e379486c547d1b`;
- tela mobile aprovada: `aec06b32af274dda84cdfab889adcf00`.

O texto está documentado em inglês porque essa é a versão principal aprovada no
Stitch. A versão em português deve manter a mesma estratégia, ordem e intenção,
com tradução editorial própria — não tradução palavra por palavra quando isso
prejudicar clareza.

O conteúdo do site atual continua sendo a fonte para fatos, URLs e histórico.
As pendências factuais encontradas estão registradas ao final deste documento.

## Posicionamento central

- Independent Software Studio;
- operação founder-led;
- custom web applications;
- internal systems e internal tools;
- business automation;
- especialização em Python/Django;
- comunicação direta com o desenvolvedor que projeta e constrói o software;
- tecnologia como meio para resolver problemas operacionais.

## Ordem da página

1. Header e navegação
2. Hero / value proposition
3. Selected Work
4. Capabilities
5. Studio Philosophy
6. Process
7. Foundation
8. About
9. Final CTA
10. Footer

---

## 1. Header e navegação

### Objetivo

Identificar imediatamente Pedro Campos como um Independent Software Studio e
oferecer acesso rápido às principais provas e ao contato.

### Wordmark

`Pedro Campos / Independent Software Studio`

### Navegação

- `Work` → `#work`
- `Capabilities` → `#capabilities`
- `Approach` → `#philosophy`
- `About` → `#about`
- `Foundation` → `#foundation`

### CTA

- label: `Start a conversation`
- destino: `mailto:pcampos119104@gmail.com`

### Conteúdo adicional

- seletor de idioma `PT`;
- na versão inglesa, deve apontar para `/pt/`;
- na versão portuguesa, deve apontar para `/`.

### Intenção comercial

Fixar o novo posicionamento antes de qualquer detalhe técnico e manter contato e
prova de trabalho acessíveis durante toda a navegação.

---

## 2. Hero / value proposition

### Objetivo

Começar pelo funcionamento do negócio do cliente e estabelecer a vantagem da
entrega direta por um desenvolvedor sênior.

### Eyebrow

`Independent software studio · São Paulo / Remote`

### Headline

`Software built around how your business actually works.`

### Supporting copy

> Custom web applications, internal tools, and automation designed and built
> directly by a senior Python/Django developer. No account managers, no
> handoffs—direct senior execution from first conversation to production.

### CTAs

1. `Discuss your project` → `mailto:pcampos119104@gmail.com`
2. `See selected work` → `#work`

### Conteúdo que deve aparecer

- nota: `Direct communication from first conversation to production.`;
- painel `Core Practice Index` com quatro frentes:
  1. `Scheduled Workflows` — scheduled workflows, report generation e email
     delivery pipelines;
  2. `Relational Data Modeling` — PostgreSQL schemas e business logic;
  3. `Server-Driven Web` — Django templates com HTMX;
  4. `REST APIs & Tooling` — Python backends, automated tests e Docker;
- rodapé do painel: `Location & Delivery / São Paulo · Remote Engagements`.

### Intenção comercial

Mostrar, no primeiro viewport, que a oferta combina entendimento operacional,
execução técnica sênior e relacionamento direto. A tecnologia sustenta a
promessa, mas não lidera a mensagem.

---

## 3. Selected Work

### Objetivo

Demonstrar capacidade por meio de software real e específico, organizado pelo
problema operacional, pelas capacidades construídas e pela arquitetura usada.

### Section label

`01 / Selected Work`

### Headline

`Bespoke software designed to solve specific operational friction.`

### Supporting copy

Não há parágrafo adicional. O Stitch mostra o metadata label
`Selected Engagements 2023–2025`, que precisa de validação antes da publicação.

### CTA

O design aprovado não apresenta CTA nos cases. Os repositórios existentes
continuam disponíveis como fonte, mas não devem ser adicionados visualmente sem
nova decisão de conteúdo.

### Case study: MDC

#### Identificação

- `CASE STUDY // MDC-01`
- `Internal Operations · Django Web Application`

#### Headline

`MDC — Member Database & Administration Platform`

#### Operational Problem

> The organization previously operated across disparate manual workflows and
> ad-hoc record keeping, creating administrative overhead, duplicate data entry,
> and inconsistent member follow-up.

#### Engineered Capabilities

1. Business rules and role-based permissions for member administration.
2. Authentication, user access control, and private file handling.
3. Scheduled background workflows for automated report generation and image
   rendering.
4. Reliable email notification delivery with error handling and status
   tracking.

#### System Architecture

`Python · Django · PostgreSQL · pytest · Docker · GitHub Actions CI/CD`

#### Metadata visual

- Database: `PostgreSQL`
- Status: `End-to-End Delivery`
- Workflows: `Scheduled Tasks`
- Testing: `pytest Suites`

#### URL existente no projeto

`https://github.com/pcampos119104/mdc`

### Case study: CDC

#### Identificação

- `CASE STUDY // CDC-02`
- `Content Architecture · Server-Driven Application`

#### Headline

`CDC — Recipe Management Application`

#### Operational Problem

> Recipe documentation, testing notes, and preparation instructions were
> dispersed across unorganized channels, creating operational friction and
> communication gaps across day-to-day culinary workflows.

#### Engineered Capabilities

1. Unified data model organizing recipe content and operational workflows in
   one place.
2. Server-driven reactive interface for rapid browsing, searching, and
   updating.
3. Authentication and access control for internal workflows.
4. Containerized local development environment with automated test suites and
   linting.

#### System Architecture

`Python · Django · HTMX · Alpine.js · Tailwind CSS · pytest · Ruff · Docker Compose`

#### Metadata visual

- UI Architecture: `HTMX & Alpine.js`
- Styling: `Tailwind CSS`
- Code Quality: `Ruff & pytest`
- Environment: `Docker Compose`

#### URLs existentes no projeto

- `https://github.com/pcampos119104/cdc`
- versão anterior: `https://github.com/pcampos119104/magapp`

### Intenção comercial

Converter projetos que antes pareciam itens de portfólio em evidência de
entendimento de negócio, modelagem de domínio, automação e entrega end-to-end.
Não usar métricas ou resultados não comprovados.

---

## 4. Capabilities

### Objetivo

Explicar o que o studio constrói em categorias reconhecíveis para compradores de
software, sem começar por uma lista de tecnologias.

### Section label

`02 / Capabilities`

### Headline

`Focused software engineering tailored to core business operations.`

### CTA

Não há CTA nesta seção.

### Conteúdo que deve aparecer

#### Custom Web Applications

> When off-the-shelf software forces compromise, bespoke web applications
> modeled around your operational workflows and data models. Built to endure
> with Python and Django without unnecessary front-end bloat.

Metadata: `Django Framework · Relational Data Modeling · Business Logic Architecture`

#### Internal Tools & Administration

> Purpose-built management portals, administrative consoles, and operational
> interfaces tailored to how your business actually runs every day.

Metadata: `Django Admin & Custom Portals · Access Control · Reporting Queries`

#### Scheduled Workflows & Processing

> Automating repetitive business workflows, data extraction, report generation,
> and transactional email with reliable Python automation and error handling.

Metadata: `Scheduled Tasks · Document & Report Generation · Delivery Pipelines`

#### Backend Systems & REST APIs

> Structured relational database architecture, robust REST endpoints, and
> service integration built for clarity, testability, and operational stability.

Metadata: `PostgreSQL Modeling · Django REST Framework · RESTful Endpoints`

### Intenção comercial

Ajudar o visitante a reconhecer o próprio problema dentro de uma capacidade do
studio e mostrar que a oferta cobre sistemas completos, não apenas tarefas de
programação.

---

## 5. Studio Philosophy

### Objetivo

Explicar por que uma operação independente pode reduzir perda de contexto,
handoffs e complexidade desnecessária.

### Section label

`03 / Studio Philosophy`

### Headline

`Why work with an independent studio?`

### Supporting copy

> Software projects fail when intent is lost between sales teams, account
> managers, and junior developers. As an independent studio, the person who
> scopes your requirements is the person who writes the code.

### CTA

Não há CTA nesta seção.

### Conteúdo que deve aparecer

1. **Direct Senior Ownership** — contato direto com um desenvolvedor com
   experiência desde 2013 e tradução dos requisitos em arquitetura sem
   intermediários.
2. **Pragmatic, Maintainable Scope** — soluções em tecnologias comprovadas,
   principalmente Python/Django, sem stack inflada.
3. **Focused Increments, Faster Clarity** — software funcional em incrementos
   focados, visibilidade e feedback sobre funcionalidades reais.

### Intenção comercial

Transformar a escala founder-led em diferencial de responsabilidade, clareza e
continuidade, sem fingir uma equipe ou estrutura de agência.

---

## 6. Process

### Objetivo

Reduzir incerteza sobre a contratação mostrando um caminho simples entre
problema operacional e software em produção.

### Section label

`04 / Process`

### Headline

`A disciplined, four-step path from operational bottleneck to production.`

### CTA

Não há CTA nesta seção.

### Conteúdo que deve aparecer

1. **Understand the operation** — entender o fluxo cotidiano, gargalos e o que
   sucesso significa em termos de negócio. Phase: `Operational Audit`.
2. **Define the right scope** — priorizar funcionalidades de maior impacto e
   definir dados e arquitetura. Phase: `Data Modeling & Architecture`.
3. **Build in focused increments** — entregar software funcional em incrementos,
   com testes e feedback direto. Phase: `Incremental Sprints`.
4. **Deployment and ongoing support** — deployment pragmático, documentação
   operacional e manutenção. Phase: `Deployment & Maintenance`.

### Intenção comercial

Mostrar método e previsibilidade sem prometer cadência, prazo ou garantia que
não tenham sido acordados para um projeto específico.

---

## 7. Foundation

### Objetivo

Apresentar a especialização técnica depois que o visitante já compreendeu valor,
trabalhos, capacidades e processo.

### Section label

`05 / Foundation`

### Headline

`Technology follows the problem, not current industry hype.`

### Supporting copy

`I prioritize proven, battle-tested software engineering tools with long-term ecosystem stability.`

### CTA

Não há CTA nesta seção.

### Conteúdo que deve aparecer

1. **Python & Django** — Python, Django, Django REST Framework, REST APIs e
   Wagtail quando apropriado.
2. **Relational Persistence** — PostgreSQL, normalização, reporting queries e
   schema migrations.
3. **Server-Driven Frontend** — Django templates, HTMX, Alpine.js, Tailwind CSS
   e HTML semântico.
4. **Automated Testing & Linting** — automated tests, pytest, Ruff e ambientes
   reproduzíveis.
5. **Workflows & Automation** — Git, GitHub Actions, CI/CD, build/test checks e
   automação por scripts.
6. **Infrastructure & Environments** — Docker, Docker Compose, Linux e
   deployment pragmático.

### Intenção comercial

Reforçar especialização e manutenibilidade sem transformar a homepage em uma
lista de skills ou currículo técnico.

---

## 8. About

### Objetivo

Dar rosto e credibilidade à operação depois que a oferta já foi estabelecida.

### Section label

`06 / About`

### Headline

`Founder & Senior Software Engineer`

### Supporting copy

> I am Pedro Campos, a senior software engineer based in São Paulo, Brazil, with
> a background in software development since 2013 and 5+ years of professional
> Python experience.

> I run this independent studio to offer business leaders a direct, senior
> technical partner for critical software initiatives. Having worked remotely
> with US-based companies, I understand that software succeeds through clear
> operational communication, pragmatic architecture, and disciplined
> follow-through—not agency bureaucracy.

> When you engage this studio, you work directly with me from requirements
> through implementation, automated testing, deployment, and ongoing
> maintenance.

### CTA

Não há CTA nesta seção.

### Conteúdo que deve aparecer

- retrato de Pedro;
- localização: `São Paulo, BR`;
- proof strip:
  - Background: `Since 2013 / Software Delivery`;
  - Specialty: `5+ Years / Professional Python`;
  - Collaboration: `Remote / US-Based Companies`;
  - Engagement: `End-to-End / Direct Execution`.

### Intenção comercial

Confirmar que o relacionamento é pessoal, sênior e end-to-end, sem deslocar a
homepage para uma narrativa de currículo.

---

## 9. Final CTA

### Objetivo

Converter visitantes que reconheceram um problema operacional e já viram prova,
capacidade, método e experiência.

### Eyebrow

`INITIATE CONVERSATION // STUDIO INQUIRY`

### Headline

`Have an operational process that software could make simpler?`

### Supporting copy

> Tell me about your current workflow, where friction lives, and what you want
> to automate. Direct conversation, without sales handoffs.

### CTAs

1. `Discuss your project` → `mailto:pcampos119104@gmail.com`
2. `pcampos119104@gmail.com` → `mailto:pcampos119104@gmail.com`

### Conteúdo adicional

`Direct conversation, without sales handoffs.`

### Intenção comercial

Fazer um convite específico e de baixo atrito, coerente com a promessa de
comunicação direta e sem linguagem genérica de vendas.

---

## 10. Footer

### Objetivo

Encerrar a página com identificação, localização, rotas essenciais, canais reais
e idioma.

### Conteúdo que deve aparecer

- `Pedro Campos / Independent Software Studio`;
- `São Paulo, Brazil · Available for Remote Engagements`;
- Selected Work, Capabilities e Approach;
- `pcampos119104@gmail.com`;
- LinkedIn: `https://linkedin.com/in/pcampos119104`;
- GitHub: `https://github.com/pcampos119104`;
- idiomas EN e PT;
- `© 2026 Pedro Campos. All rights reserved. Built with precision.`

### CTA

O email funciona como CTA secundário. Links sociais são apoio de confiança.

### Intenção comercial

Manter a operação verificável e fácil de contatar sem adicionar uma última
camada promocional.

## Pendências factuais antes da implementação do conteúdo definitivo

O design aprovado contém textos que não estão comprovados literalmente pelo
site atual. Eles permanecem documentados por fidelidade ao Stitch, mas precisam
de validação:

1. `Selected Engagements 2023–2025`: o site atual não atribui esse intervalo aos
   dois projetos e apresenta MDC como trabalho iniciado em setembro de 2025.
2. O problema do MDC menciona duplicate data entry e inconsistent member
   follow-up; o site atual confirma processos manuais, mas não essas duas
   consequências específicas.
3. O problema do CDC menciona documentação dispersa, testing notes e gaps de
   comunicação; o site atual apenas confirma que o sistema organiza conteúdo e
   fluxos de receitas em um lugar.
4. `Incremental Sprints` e `Rapid cycles` não aparecem como método formal no
   conteúdo atual.
5. `Tested & Documented` deve ser entendido como princípio de trabalho; o site
   atual confirma testes e práticas de documentação em contextos específicos,
   não uma certificação geral.
6. O Stitch usa URLs genéricas para LinkedIn e GitHub. A implementação deve usar
   as URLs reais registradas acima.
7. O Stitch mostra o seletor `PT` como botão sem destino. A implementação deve
   preservar as rotas atuais `/` e `/pt/`.
8. `REGISTER REF // 2026.01` funciona como detalhe editorial no hero, mas não
   corresponde a uma versão pública ou data comprovável do studio. Confirmar se
   o label permanece decorativo ou se deve ser omitido antes da publicação.
