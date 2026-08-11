# TSplus Remote Access — Apresentação Comercial
## Conteúdo final (v2 — tom institucional/consultivo) + Prompt para Claude Design

Fonte dos números institucionais: página oficial
https://tsplusbrasil.com.br/institucionais/remote-access (consultada em 27/07/2026).

Estrutura: 7 slides principais + 1 apêndice técnico (fora da contagem/narrativa de venda).

---

## CONTEÚDO FINAL DOS SLIDES

### Slide 01 — Capa
TSPLUS BRASIL
Remote Access

### Slide 02 — Cenário de mercado
**Um cenário conhecido em TI**

Equipes de tecnologia enfrentam hoje uma dupla exigência: manter sistemas críticos funcionando com segurança, e viabilizar acesso remoto sem inflar o orçamento com licenciamento complexo.

Soluções tradicionais como Citrix e Microsoft RDS resolvem a parte técnica, mas costumam elevar o custo total de propriedade com CALs, infraestrutura dedicada e renovações anuais obrigatórias. É nesse contexto que o TSplus Remote Access se posiciona como alternativa.

### Slide 03 — Nossa Missão
**Nossa Missão**

Desde 2007, seguimos um único princípio: tornar aplicativos e dados do mundo simples de acessar, em qualquer lugar, a qualquer momento, por qualquer dispositivo ou rede.

Isso se traduz em um ecossistema pensado pra cobrir toda a jornada de TI da sua empresa: o Remote Access entrega seus sistemas com segurança, o Remote Support leva assistência técnica até onde seu time estiver, o Advanced Security blinda seus servidores contra ataques, e o Server Monitoring acompanha a saúde da sua infraestrutura em tempo real.

**Estatísticas:** 18 anos no mercado · 500 mil+ clientes · 4.8/5 avaliação Sourceforge · 80% economia média

### Slide 04 — TSplus Remote Access vs. Citrix e Microsoft RDS
Os três resolvem o mesmo problema central: publicar desktops e aplicações Windows para acesso remoto. A diferença está em como cada um chega lá.

**Sem plugins ou clientes específicos** — funciona em qualquer navegador (Chrome, Firefox, Safari), enquanto soluções tradicionais geralmente exigem instalação de cliente próprio.

**Sem CALs do Windows Server** — o modelo de licenciamento do RDS costuma exigir CAL por usuário; o TSplus não.

**Implantação em menos de um dia** — comparado a projetos de Citrix, que costumam levar semanas.

**Licenças simultâneas irrestritas** — sem cobrança adicional por usuário conectado.

**Portal web com a identidade da sua empresa** — personalização completa, sem depender de equipe de design.

> ⚠️ Não incluí números de TCO (ex: R$ 80.000 vs economia em 3 anos) porque essa peça específica é de marketing de redes sociais, não uma fonte institucional auditada. Se você tiver o estudo de TCO original, me passa que eu incorporo com mais força nesse slide.

### Slide 05 — Benefícios centrais
**Menos risco para o seu negócio** — Conexões protegidas por criptografia TLS/SSL, com Advanced Security e 2FA disponíveis para quem precisa de uma camada extra de controle.

**Aproveite o que você já construiu** — Leve sistemas Windows legados para a web sem reescrever uma linha de código, prolongando o valor do que sua empresa já investiu.

**Previsibilidade no orçamento de TI** — Licença vitalícia: você paga uma vez e usa para sempre, sem surpresa em renovação obrigatória.

### Slide 06 — Vantagens técnicas
**Sua operação não para** — Load balancing distribui usuários entre servidores automaticamente, com fallback pronto caso um servidor falhe.

**Sua equipe acessa de onde estiver** — Qualquer navegador, qualquer sistema operacional, sem instalar nada.

**Sua marca, sua cara** — Portal personalizável com cores, nome e identidade da sua empresa.

**Sem dor de cabeça com impressão** — Impressão remota universal, sem configurar driver específico.

**Controle centralizado** — Um único portal Gateway para gerenciar acesso a múltiplos servidores e usuários.

### Slide 07 — Fechamento institucional
A TSplus está presente globalmente, mas o atendimento que chega até você é local: suporte técnico no Brasil, de segunda a sexta, das 8h às 18h.

Sem cartão de crédito. Instalação em minutos. Suporte técnico no Brasil.

**Guilherme Filippo**
Diretor Regional Brasil
guilherme@tsplusbrasil.com.br
www.tsplusbrasil.com.br

**CTA:** Teste grátis por 15 dias

### Apêndice — Versão / Instalação
*(fora da narrativa de venda — puxar apenas se o cliente pedir detalhe técnico ao vivo)*

**Remote Access — Versão e Instalação**

Os setups apresentados aqui estão na última versão disponível até a data desta demonstração.

Setup-ConnectionClient.exe → versão do cliente, instalado no usuário
Setup-TSplus.exe → versão do servidor

> ⚠️ Confirmar com Jonathan a versão vigente antes de usar (o slide original tinha data de referência 23/02, que pode estar desatualizada).

---

## PROMPT PARA O CLAUDE DESIGN

Cole o texto abaixo no Claude Design, dentro do projeto/organização onde o sistema de marca `tsplus-brasil-brand` já estiver vinculado:

```
Crie uma apresentação comercial para a TSplus Brasil, produto Remote
Access, usando o sistema de marca da organização (design system já
vinculado a partir do repositório tsplus-brasil-brand).

Público-alvo: gestores de TI, analistas de infraestrutura e software
houses avaliando alternativas ao Citrix, Microsoft RDS ou VPN
tradicional.

Tom: institucional e corporativo, com viés consultivo. Evite qualquer
tom de página de vendas com gatilho agressivo — a comunicação deve
soar como um relatório de mercado conduzido por especialistas, não
como um anúncio. Nada de urgência artificial, contadores regressivos
ou linguagem de "oferta".

Tema visual: dark theme, seguindo a regra do design system (dark para
Security/Monitoring/Remote Access, light para Support/mobilidade).

Estrutura: 7 slides principais + 1 slide de apêndice técnico (marcado
visualmente como separado da narrativa principal, ex: numeração "A1"
ou etiqueta "Apêndice").

Slide 1 — Capa
"TSPLUS BRASIL" / "Remote Access"

Slide 2 — Cenário de mercado
Texto institucional sobre a dupla exigência de segurança e custo que
equipes de TI enfrentam hoje, posicionando o TSplus Remote Access como
resposta a esse cenário — sem citar concorrentes de forma direta aqui
(a comparação direta vem no slide 4).

Slide 3 — Nossa Missão
Texto sobre a missão da TSplus desde 2007, citando os 4 produtos do
ecossistema (Remote Access, Remote Support, Advanced Security, Server
Monitoring). 4 estatísticas em destaque: 18 anos no mercado, 500 mil+
clientes, 4.8/5 avaliação Sourceforge, 80% economia média.

Slide 4 — Comparativo direto: TSplus Remote Access vs. Citrix vs.
Microsoft RDS
Apresentar como tabela ou 5 blocos de diferencial, tom factual e
educado, sem menosprezar os concorrentes: sem plugins/clientes
específicos, sem CALs do Windows Server, implantação em menos de um
dia, licenças simultâneas irrestritas, portal web personalizável.

Slide 5 — Benefícios centrais (3 cards)
Menos risco para o negócio (segurança), aproveitamento do que já foi
construído (sistemas legados), previsibilidade de orçamento (licença
vitalícia) — cada um com ícone e texto focado no resultado para o
comprador, não na feature em si.

Slide 6 — Vantagens técnicas (5 cards)
Load Balancing, Acesso via Web, Portal Web Personalizável, Impressora
Universal, Portal Gateway — cada um reescrito com foco no benefício
prático para quem gerencia TI (continuidade, mobilidade, identidade de
marca, praticidade, controle centralizado).

Slide 7 — Fechamento institucional
Suporte técnico local no Brasil (segunda a sexta, 8h às 18h), reforços
de baixa fricção (sem cartão de crédito, instalação em minutos),
contato do Diretor Regional Brasil Guilherme Filippo, CTA final "Teste
grátis por 15 dias".

Apêndice — Versão / Instalação
Bloco técnico simples com nome dos instaladores (Setup-ConnectionClient.exe
para o cliente, Setup-TSplus.exe para o servidor) e nota de que a
versão deve ser confirmada antes do uso ao vivo.

Use as referências aprovadas da pasta 03-referencias-aprovadas/dark-theme
do design system como guia de estilo visual (glow laranja difuso, cards
translúcidos, tipografia Red Hat Display, grid 55/45) — mas mantenha a
composição mais sóbria e institucional do que uma peça de rede social,
já que este é um material de apresentação comercial, não um post.

Para fotos ou ilustrações realistas (ex: pessoa trabalhando, ambiente
de escritório), não gere — vou anexar imagens já prontas em seguida.
Por enquanto, use placeholders neutros ou os padrões gráficos (grid
pontilhado, glow, ícones) do sistema de marca.

Texto completo de cada slide (copy final aprovado):
[colar aqui o conteúdo da seção "CONTEÚDO FINAL DOS SLIDES" acima]
```

**Nota:** o prompt reforça explicitamente o tom institucional/consultivo (sem gatilho de vendas agressivo) porque essa é a linha mais fácil de o Claude Design "escorregar" — modelos de IA tendem a puxar pro tom de landing page quando veem estrutura de benefícios/CTA. Se o resultado vier com qualquer termo tipo "oferta imperdível" ou contagem regressiva, é só pedir pra ele reescrever mais sóbrio, citando esse mesmo ponto.
