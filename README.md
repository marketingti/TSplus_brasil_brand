# TSplus Brasil — Brand & Design System

Repositório de referência da identidade visual e de conteúdo da **TSplus Brasil**, subsidiária oficial da TSplus (acesso remoto, virtualização, segurança cibernética e monitoramento de servidores).

Este repositório serve como fonte para o **sistema de design no Claude Design**, garantindo que qualquer apresentação comercial, post de rede social, landing page ou material de vendas siga o mesmo padrão visual e de voz de marca.

## Estrutura

```
tsplus-brasil-brand/
├── 01-diretrizes/              → Guia oficial de arte e design (fundação de tudo)
├── 02-identidade-visual/        → Logos, paleta de cores, tipografia e regras de apresentação (tokens)
│   └── logos/                   → Variações do logotipo (a preencher)
├── 03-referencias-aprovadas/    → Peças reais já publicadas, aprovadas, no padrão atual
│   ├── dark-theme/              → Security, Monitoring, Remote Access
│   └── light-theme/             → Remote Support, Software Houses, mobilidade
├── 04-institucional/            → Quem somos, missão, visão, valores, produtos
├── 05-apresentacoes/            → Apresentações comerciais (aprovadas, em andamento e antigas)
│   └── originais-antigas/       → PDFs das apresentações antigas (material-fonte)
└── 06-fontes/                   → Arquivos de fonte Red Hat Display (a preencher)
```

## Status das 5 apresentações comerciais (ecossistema completo)

| Produto | Status | Arquivo de conteúdo/prompt |
|---|---|---|
| Remote Access | ✅ Aprovada — é a referência visual definitiva | `remote-access-conteudo-e-prompt.md`, `remote-access-APROVADA.pdf` |
| Remote Support | Conteúdo e prompt prontos | `remote-support-conteudo-e-prompt.md` |
| Server Monitoring | Conteúdo e prompt de correção prontos | `server-monitoring-conteudo-e-prompt.md`, `prompt-correcao-server-monitoring.md` |
| Advanced Security | Conteúdo e prompt (geração do zero) prontos | `advanced-security-conteudo-e-prompt.md` |
| Two-Factor Authentication | Conteúdo pronto + correção de composição visual solicitada | `two-factor-conteudo-e-prompt.md`, `prompt-correcao-two-factor.md` |

Outros prompts de apoio:
- `prompt-referencia-imagens-jpeg.md` — como usar imagens JPEG da apresentação aprovada como referência visual no Claude Design
- `prompt-exportar-canva.md` — como pedir pro Claude Design exportar um projeto pro Canva
- `template-mestre-apresentacao.md` — **documento central de regras**, leia antes de gerar qualquer apresentação nova

## Regras inegociáveis de marca e de apresentação (resumo rápido)

- Fonte única: **Red Hat Display**
- Grid: **55% texto / 45% visual** (50/50 em banners horizontais)
- Tema Dark (`#242424`) → Security, Monitoring, Remote Access
- Tema Light (branco/cinza claro) → Support, mobilidade, Software Houses
- Laranja `#ff9106`: glow difuso no dark, sólido em ícones/botões no light — **nunca fundo chapado**
- CTA sempre consultivo: "Fale com um consultor", "Teste grátis por 15 dias" — nunca "Compre agora"
- Logo: canto superior direito (ou topo-centro em Stories)
- Rodapé: `tsplusbrasil.com.br`
- Proibido: hacker cartunizado, monitor CRT, selos de desconto/Black Friday

### Regras específicas de apresentações comerciais (ver `template-mestre-apresentacao.md` para detalhes)
- Apenas **Capa, Nossa Missão e Perto de Você** são idênticos em todas as apresentações
- Os outros 4 slides têm **identidade visual própria por produto** — nunca repetir a mesma composição (tabela, cards numerados, bullets+pizza) de uma apresentação pra outra
- **Sem slide de Versão/Instalação** em nenhuma apresentação comercial
- **"80% de economia média"** é estatística institucional exclusiva do slide de Nossa Missão — não repetir em outros slides
- Sempre **reservar espaço para imagens** (bloco neutro) em vez de gerar fotos realistas
- Evitar concorrentes nomeados sem fonte oficial confirmada — preferir comparação "Antes vs. Depois" quando não houver comparação publicada pela TSplus

Ver `01-diretrizes/DESIGN_AGENTES_tsplus.pdf` para o guia visual completo e `04-institucional/resumo-institucional.md` para dados institucionais (incluindo a divergência de "anos no mercado" entre páginas do site, ainda não resolvida).
