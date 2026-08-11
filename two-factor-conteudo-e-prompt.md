# TSplus Two-Factor Authentication — Apresentação Comercial
## Conteúdo final + Prompt de geração (do zero) para Claude Design

Fonte: página oficial https://tsplusbrasil.com.br/institucionais/two-factor-authentication
(consultada em 31/07/2026), adaptando também o conteúdo bruto da apresentação
antiga (05 - TWO FACTOR - ok.pdf), com copy melhorado e tom mais institucional.

> ⚠️ Nota sobre estatísticas: essa é a única página oficial que ainda mostra
> **16 anos no mercado** — as páginas de Remote Support, Server Monitoring e
> Advanced Security já mostram 18/19+. Ou seja, o "16 anos" da apresentação
> antiga não estava desatualizado por causa do deck — é a própria página do
> 2FA que ainda não foi atualizada no site. Usei 16 anos aqui por ser o dado
> oficial vigente desta página específica, mas vale sinalizar pra Guilherme/
> Alex que essa página parece estar defasada em relação às outras.

> ⚠️ Sem concorrentes nomeados nem estatística de "% de economia" específica
> do 2FA na página oficial — por isso a comparação usa o formato "Antes vs.
> Depois", e os gráficos usam dados estruturais reais do produto (não
> percentuais inventados).

---

## CONTEÚDO FINAL DOS SLIDES

### Slide 01 — Capa 🔒 PADRONIZADO
TWO FACTOR AUTHENTICATION

Adicione uma camada extra de proteção ao seu portal web. Sem hardware extra, sem complicação, sem brecha.

### Slide 02 — Cenário de mercado 🎨 IDENTIDADE PRÓPRIA
**CENÁRIO DE MERCADO**

Um cenário conhecido em TI.

Confiar apenas em nome de usuário e senha para proteger o acesso corporativo deixou de ser suficiente. Ataques deixaram de ser genéricos: hoje o malware é desenhado sob medida para atingir empresas e indivíduos específicos, com barreira de entrada cada vez menor para o invasor.

**Composição sugerida (diferente do Advanced Security):** em vez de texto + gráfico, use uma **linha do tempo horizontal** de 2 pontos mostrando a evolução da ameaça: "Ontem — vírus genéricos, ataques em massa" → "Hoje — malware sob medida, mirando empresas específicas". Elementos gráficos minimalistas (ícone de vírus disperso vs. ícone de alvo/mira), sem tabela e sem gráfico de pizza.

### Slide 03 — Nossa Missão 🔒 PADRONIZADO
*(Este slide deve ser idêntico ao slide de referência de Remote Access, mudando apenas a etiqueta "ESTE PRODUTO" para "Two-Factor Authentication". Se você enviar este slide já pronto separadamente, use a versão enviada no lugar desta.)*

**DESDE 2007**

Nossa missão.

Seguimos um único princípio: tornar aplicativos e dados do mundo simples de acessar, em qualquer lugar, a qualquer momento, por qualquer dispositivo ou rede.

Um ecossistema que cobre toda a jornada de TI:

- **Remote Access** — Entrega seus sistemas com segurança.
- **Remote Support** — Assistência onde seu time estiver.
- **Advanced Security** — Blinda seus servidores contra ataques.
- **Server Monitoring** — Saúde da infraestrutura em tempo real.
- **Two-Factor Authentication (2FA)** — Senhas dinâmicas e autenticação multifator para proteger seu portal web. *(ESTE PRODUTO)*

**Estatísticas:** 16 anos no mercado · 500 mil+ clientes no mundo · 4.8/5 avaliação Sourceforge · 80% de economia média

### Slide 04 — Como funciona o TSplus 2FA 🎨 IDENTIDADE PRÓPRIA
**COMO FUNCIONA**

Duas etapas. Uma camada real de proteção.

**Composição sugerida (diferente do Advanced Security — sem tabela):** fluxo visual horizontal de 3 passos, com ícone e uma frase curta em cada:
1. **Senha** — O usuário digita usuário e senha, como sempre fez.
2. **Código dinâmico** — O app autenticador no celular gera um código, renovado a cada 30 segundos.
3. **Acesso liberado** — Só entra quem tiver as duas coisas: a senha e o dispositivo.

Abaixo do fluxo, uma frase de reforço: "Mesmo que a senha vaze, o código sozinho não abre a porta — e o código sozinho, sem a senha, também não."

### Slide 05 — O que muda para o negócio 🎨 IDENTIDADE PRÓPRIA
**O QUE MUDA PARA O NEGÓCIO**

**Composição sugerida (diferente do Advanced Security — sem cards numerados verticais):** 3 números em destaque, estilo "stat callout" lado a lado (como um placar), cada um com o número grande e uma frase curta embaixo, sem ícone de escudo repetido:

- **30 segundos** — é o tempo de vida de cada código gerado, o suficiente para impedir reuso de senha vazada.
- **Zero** — hardware adicional necessário: funciona no celular que o colaborador já usa.
- **Poucos cliques** — para habilitar, adicionar usuários ou redefinir credenciais, direto pelo AdminTool.

### Slide 06 — Gestão no dia a dia 🎨 IDENTIDADE PRÓPRIA
**GESTÃO NO DIA A DIA**

**Composição sugerida (diferente do Advanced Security — sem bullets + pizza):** ilustração central de um smartphone com tela de código de verificação (mockup simples), rodeado por 3 ícones de apps compatíveis (Authy, Google Authenticator, Microsoft Authenticator) conectados ao aparelho por linhas finas. Ao lado ou abaixo, 2 blocos curtos de texto:

- **Funciona offline** — Códigos gerados no próprio dispositivo, mesmo sem conexão à internet.
- **Bloqueio inteligente** — Conexões RDP diretas são negadas para usuários com 2FA habilitado, fechando essa porta de entrada.

### Slide 07 — Perto de Você 🔒 PADRONIZADO
**SUPORTE LOCAL**

Perto de você.

A TSplus está presente globalmente, mas o atendimento que chega até você é local: suporte técnico no Brasil, de segunda a sexta, das 8h às 18h.

Cada região tem sua própria cultura, exigência de negócios, idioma e espírito. Nossos diretores garantem que a TSplus esteja fornecendo todos os dias e em todos os lugares a mesma qualidade e profissionalismo.

**Guilherme Filippo**
Diretor Regional Brasil
guilherme@tsplusbrasil.com.br
www.tsplusbrasil.com.br
Segunda a sexta, 8h às 18h (BRT)

**CTA:** Teste grátis por 15 dias / Fale com um consultor

---

## PROMPT DE GERAÇÃO PARA O CLAUDE DESIGN
### (do zero — para usar junto com as 7 imagens JPEG da apresentação de Remote Access como referência)

```
As imagens anexadas, nesta ordem, são os slides de uma apresentação
comercial da TSplus Brasil (produto Remote Access) já aprovada pela
diretoria. Elas são a referência de identidade de marca — extraia dela
as cores, tipografia, ícones, tratamento de foto e o tom geral de
comunicação.

Gere uma apresentação nova (do zero) para o produto Two-Factor
Authentication, seguindo esta regra de padronização:

Os slides de mesma posição das imagens 1 (Capa), 3 (Nossa Missão) e 7
(Perto de você) devem ser reproduzidos de forma IDÊNTICA ao que está
nessas imagens — mesmo layout, mesma tipografia, mesmo texto
institucional. Mudam apenas: o nome do produto na capa, a etiqueta
"ESTE PRODUTO" no slide de missão (movida para "Two-Factor
Authentication"), e o número de "anos no mercado" (16, conforme a
página oficial deste produto).

Não crie nenhum slide de "Versão/Instalação" — não deve existir em
nenhum lugar da apresentação.

Se eu enviar o slide de Nossa Missão já pronto separadamente, use a
versão que eu enviar no lugar do que está descrito no conteúdo abaixo.

Os slides de mesma posição das imagens 2 (Cenário de mercado), 4
(Comparativo), 5 (O que muda para o negócio) e 6 (Gestão no dia a dia)
devem manter a identidade de marca (cores, tipografia, tom), mas ter uma
COMPOSIÇÃO VISUAL PRÓPRIA — diferente não só das imagens de referência do
Remote Access, mas também das outras apresentações já geradas (Remote
Support, Server Monitoring, Advanced Security), que usaram tabela
"Antes vs Depois", cards numerados verticais e bullets com gráfico de
pizza. Para o 2FA, use as composições específicas indicadas no conteúdo
abaixo: linha do tempo horizontal, fluxo de 3 passos, números em
destaque estilo placar, e ilustração de smartphone com apps ao redor.
Evite repetir o formato de tabela comparativa ou de cards numerados
verticais usado nas apresentações anteriores.

Em todos os slides que tiverem (ou deveriam ter) tratamento fotográfico,
deixe uma área reservada claramente demarcada no lugar da imagem — um
bloco de fundo neutro, sem gerar fotografia ou ilustração realista. Isso
me permite substituir por uma foto própria depois.

Tom: institucional e corporativo, com viés consultivo — sem gatilho de
venda agressivo, urgência artificial ou linguagem de oferta.

Texto completo de cada slide para Two-Factor Authentication:
[colar aqui o conteúdo da seção "CONTEÚDO FINAL DOS SLIDES" acima]
```
