# TSplus Brasil — Variações de Posicionamento dos Criativos

> Documento de orientação para diversificar a composição dos criativos (Feed, Capa de Carrossel, estrutura interna de Carrossel) e evitar repetição de layout entre peças. Aplica-se a todas as redes onde a TSplus Brasil publica hoje: Instagram (Feed, Stories, Carrossel), LinkedIn, Google Meu Negócio, e demais formatos de conteúdo visual da marca.
>
> Segue as diretrizes já estabelecidas no repositório (`design-tokens.json`, `DESIGN_AGENTES_tsplus.pdf`): paleta escura #242424 com glow laranja #ff9106, tipografia Red Hat Display, CTA sempre consultivo, blacklist de elementos proibidos.

---

## 1. Diagnóstico do padrão atual

Analisando as peças em produção hoje (ex.: "500 mil clientes globais", "ERP desktop acessível via browser", "Saiu do Citrix?"), o padrão se repete em 100% dos casos:

- Personagem sempre à **direita**, corpo cortado, olhando para fora do quadro ou de braços cruzados.
- Bloco de texto sempre à **esquerda**, mesma hierarquia (rótulo pequeno → headline em 2-3 linhas → parágrafo de apoio → CTA laranja).
- CTA sempre no mesmo ponto (abaixo do parágrafo, alinhado à esquerda).
- Fundo sempre escuro, sem nenhuma peça em fundo claro.

Isso cria consistência de marca, mas gera fadiga visual quando várias peças aparecem em sequência (feed do Instagram, carrossel, anúncios em rotação). O objetivo deste documento é introduzir variação controlada — sem perder identidade de marca.

---

## 2. Princípios que não mudam (independem da variação)

- Paleta: fundo escuro #242424 (com gradiente pro preto) **ou** fundo claro (ver seção 5.1, novo — a validar), laranja #ff9106 só como glow/destaque (nunca como preenchimento chapado), branco #ffffff.
- Tipografia Red Hat Display; rótulos em uppercase com tracking aberto.
- CTA sempre consultivo ("Fale com um especialista", "Solicite uma demonstração", "Modernize seus sistemas legados") — nunca "Compre agora".
- Fotos de personagem em preto e branco/dessaturadas só quando usadas como plano de fundo (10–15% opacidade); quando o personagem é o sujeito principal da foto, mantém cor.
- Blacklist continua valendo em toda variação: hacker de capuz cartoon, monitor CRT, selos de desconto/Black Friday, fundo laranja chapado.
- Nunca citar concorrentes nomeados nas peças (usar o ângulo de ataque descrito em `base-concorrentes.md` sem citar o nome).

---

## 3. Variações de posicionamento — Feed (peça única)

Quatro composições para alternar entre publicações de feed. Nenhuma delas substitui as outras — são um repertório para rodar em rotação.

### Variação A — Personagem à direita (atual, manter como uma das opções)
- Grid 55/45 (texto/visual), como já documentado.
- Texto alinhado à esquerda, personagem ocupa a faixa direita, corpo cortado.
- CTA abaixo do parágrafo, alinhado à esquerda.
- Uso recomendado: peças de prova social e institucionais (estatísticas, "sobre a marca").

### Variação B — Personagem à esquerda (espelhada)
- Inverte o grid: 45/55 (visual/texto).
- Texto alinhado à direita, personagem na faixa esquerda.
- CTA abaixo do parágrafo, alinhado à direita.
- Uso recomendado: peças de caso de uso e comparação/migração — o espelhamento sinaliza visualmente "virada de chave" (ex.: campanhas "Saiu do Citrix?").

### Variação C — Personagem ao fundo, texto centralizado
- Personagem em plano geral, desfocado ou em baixa opacidade (15–25%), ocupando o fundo inteiro do quadro.
- Texto centralizado sobre um scrim escuro (gradiente radial ou painel semitransparente) para garantir contraste.
- CTA centralizado, logo abaixo do parágrafo.
- Uso recomendado: peças de campanha/data comemorativa, ou quando o personagem não é o foco central da mensagem (ex.: anúncio de funcionalidade específica).

### Variação D — Sem personagem humano (tipográfica/gráfica)
- Composição 100% gráfica: número/dado em destaque (headline grande), elemento visual abstrato de apoio (glow técnico, malha de dados, ícone de cadeado/nuvem/servidor conforme o produto).
- Texto ocupa até 70% do quadro, alinhamento livre (esquerda ou centralizado).
- CTA sempre presente, mesmo sem personagem.
- Uso recomendado: **Two-Factor Authentication** (único produto sem personagem na ficha atual — ver `ficha-personagens.md`), estatísticas isoladas, ou para dar respiro visual entre peças com personagem.

---

## 4. Variações de capa — Carrossel

A capa precisa parar o scroll em 1–2 segundos. Recomendo 4 variações, para rotacionar por tema de campanha:

1. **Capa-dado**: número grande (ex.: "500 mil clientes") + personagem à direita — igual à Variação A do feed, mas com menos texto de apoio (a capa não carrega parágrafo longo).
2. **Capa-pergunta**: headline em forma de pergunta ("Saiu do Citrix?", "Seu RDP está exposto?") + personagem à esquerda olhando para o texto (não para fora do quadro) — cria tensão narrativa que "puxa" para o slide 2.
3. **Capa-manchete sem personagem**: manchete tipográfica grande centralizada sobre fundo com glow laranja forte, sem foto — indicada quando o carrossel é sobre um produto sem persona fixa (2FA) ou conteúdo mais técnico/educativo (ex. SEO, changelog).
4. **Capa-selo**: rótulo de formato ("Guia", "Checklist", "Comparativo") em destaque + ícone/elemento gráfico do produto, personagem pequeno em segundo plano ou ausente — indicada para conteúdo educativo/how-to.

Em todas: indicador de carrossel (setas ou "1/6") no canto, para deixar claro que há mais slides.

---

## 5. Variações de estrutura interna do Carrossel (slides 2 em diante)

Cinco estruturas de slide para intercalar dentro de um mesmo carrossel, evitando repetir a mesma composição em todos os slides internos.

### 5.1 Nota sobre alternância de cor (fundo escuro ↔ fundo claro)

Hoje o repositório só documenta o tema escuro para a TSplus. Para permitir a alternância que você pediu (ex.: slide 2 escuro → slide 3 claro), proponho o seguinte **tema claro complementar** — a validar com você antes de virar padrão oficial:

- Fundo: branco ou off-white (#F7F7F5)
- Texto: grafite escuro (#242424) — a mesma cor do fundo escuro, só invertida
- Laranja #ff9106 mantém a mesma função de destaque/CTA (não muda entre temas)
- Como as fotos dos personagens (ficha de personagens) foram geradas com fundo escuro (datacenter, sala de servidores), em slides de fundo claro recomendo **não** usar a foto em full-bleed — usar o personagem recortado (só a figura, sem o fundo original) sobre o fundo claro, ou reservar o fundo claro para slides sem personagem (dado, citação, comparação).

### 5.2 As cinco estruturas

**Estrutura 1 — Slide de dado/estatística**
- Fundo escuro. Número grande centralizado ou à esquerda. Personagem cortado no canto inferior direito (só ombro/rosto, não corpo inteiro). Rótulo pequeno no topo indicando a fonte do dado.

**Estrutura 2 — Slide de benefício/feature**
- Fundo claro. Ícone do recurso (não foto) + texto curto (1 frase) alinhado à esquerda ou centralizado. Sem personagem. Bom para listar módulos de produto (ex.: os recursos do Advanced Security) em slides separados.

**Estrutura 3 — Slide comparativo (split screen)**
- Metade escura ("Sem TSplus") + metade clara ("Com TSplus"), lado a lado ou empilhadas. Ícones ou frases curtas de cada lado. Sem citar concorrente nomeado do lado "sem".

**Estrutura 4 — Slide de citação/prova social**
- Fundo escuro com textura sutil (malha técnica, glow lateral). Aspas grandes em laranja. Personagem ao fundo, bem desfocado e em baixa opacidade (a mesma lógica de "background photo" já documentada). Texto centralizado verticalmente.

**Estrutura 5 — Slide de CTA final**
- Fundo escuro com glow laranja mais intenso que os slides anteriores (sinaliza "fim do carrossel, hora de agir"). Botão de CTA centralizado, grande. Personagem de corpo inteiro (se o produto tiver ficha) ou ausente (2FA) — braços abertos/postura convidativa em vez de braços cruzados, para variar da pose padrão de capa.

### 5.3 Sequência sugerida (exemplo de 6 slides)

| Slide | Estrutura | Fundo |
|---|---|---|
| 1 (capa) | Capa-pergunta ou capa-dado | Escuro |
| 2 | Estrutura 1 — dado/estatística | Escuro |
| 3 | Estrutura 2 — benefício/feature | Claro |
| 4 | Estrutura 3 — comparativo | Split escuro/claro |
| 5 | Estrutura 4 — citação | Escuro |
| 6 | Estrutura 5 — CTA final | Escuro (glow intenso) |

A alternância não precisa ser rígida — o importante é não repetir a mesma estrutura em dois slides consecutivos, e usar o fundo claro como respiro visual a cada 2–3 slides.

---

## 6. Aplicação por canal

- **Instagram Feed:** Variações A–D da seção 3, formato 4:5 ou 1:1.
- **Instagram Carrossel:** Capas da seção 4 + estruturas internas da seção 5, formato 4:5.
- **Instagram Stories:** grid já documentado (top20/center40/base40); aplicar Variação C (personagem ao fundo) ou D (tipográfica) com mais frequência, já que Stories tem menos espaço para grid 55/45.
- **LinkedIn:** priorizar Variação A ou B (personagem + texto), tom mais institucional/dado de mercado; banner horizontal usa grid 50/50 já documentado para os outros brands do grupo — replicar proporção para TSplus quando for peça de banner.
- **Google Meu Negócio:** priorizar Variação D (tipográfica, direto ao ponto) ou capa-selo — pouco espaço para texto longo, imagem precisa comunicar em 1 olhada.

---

## 7. Checklist antes de publicar uma peça

- [ ] A composição escolhida é diferente da última peça publicada no mesmo canal?
- [ ] Se o carrossel tem mais de 4 slides, há pelo menos uma troca de fundo (escuro↔claro)?
- [ ] O personagem usado tem ficha correspondente ao produto (`ficha-personagens.md`)? Se for 2FA, usar Variação D/estrutura sem personagem.
- [ ] O CTA é consultivo, nunca "compre agora"?
- [ ] Nenhum concorrente é citado pelo nome na peça?
- [ ] A paleta e a tipografia seguem `design-tokens.json`?

---

*Documento inicial — as variações de posicionamento serão refinadas conforme referências visuais adicionais forem enviadas pela gestora de marketing.*
