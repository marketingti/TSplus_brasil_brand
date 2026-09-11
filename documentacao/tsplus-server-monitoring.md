# TSplus Server Monitoring

> **Documentação completa TSplus** — 109 páginas

---


---
*Página 1*

Ativando sua licença
Server Monitoring inclui um Painel de Administração de Licenças.
Na tela inicial, você pode ver o status da sua Licença na barra de status na parte inferior. Por
exemplo, uma Licença de teste como visto abaixo:
Para ver o status e as informações da sua Licença, com seu ID de Computador e Nome do
Computador, clique no botão de Licença ou no status da licença na barra de status:

---
*Página 2*

Esta tela mostra detalhes sobre sua licença e oferece opções para ativação e atualizações:
Clique no botão “Ativar Licença” e depois clique no menu “Administração” > “Licença”.
Você encontrará sua chave de ativação permanente (XXXX-XXXX-XXXX-XXXX) na nossa
confirmação de pedido por e-mail.
Se você deseja ativar sua assinatura, insira sua chave de assinatura. (S-XXXX-XXXX-XXXX-
XXXX) .
Para obter sua Chave de Ativação, conecte-se ao nosso Portal de Licenciamento , insira seu
endereço de e-mail e seu número do pedido:

---
*Página 3*

Baixe o Guia do Usuário do Portal do Cliente para mais informações sobre como usá-lo.
Você poderá ver e copiar sua chave de ativação. Clique no botão “Ativar sua Licença” e insira-a:
Você pode ver o novo status da sua Licença voltando para os detalhes da sua licença:
Atualize seus dados de licença clicando em 'Atualizar sua licença' - isso sincronizará as
informações com nosso Portal de Licenciamento.
Obrigado por escolher Server Monitoring!
Exportar logs para suporte:

---
*Página 4*

Exporte logs para ajuda do suporte.
1. Ativar solução de problemas
2. Reproduza o problema
3. Exportar logs para ajuda

---
*Página 6*

Gerenciamento de Alertas
Você pode acessar a Gestão de Alertas clicando em Gestão título de Alertas seção na
página inicial:
Quando você instala um agente em um servidor para monitorar, o Server Monitoring criará
automaticamente alertas básicos para o servidor. Criar um novo site também criará alertas para
o site.

---
*Página 7*

Usando o botão “Adicionar novo Alerta”, você pode adicionar alertas ao seu sistema de Server
Monitoring.

---
*Página 8*

Para servidores , os alertas podem ser configurados para:
Processador
Memória
Uso de leitura/gravação de disco
Uso da rede (bytes enviados/recebidos)
Espaço em disco usado
Usuários Ativos
Duração do Tempo de Inatividade
Para sites da web alertas podem ser configuradas para Tempo de Resposta ou Duração de
Inatividade.
Por favor, selecione o tipo de alerta que deseja criar e o(s) servidor(es) ou site(s) que deseja
monitorar.
Então você pode definir os parâmetros do alerta:

---
*Página 9*

Você pode personalizar as configurações com seus próprios valores:

---
*Página 10*

Você pode adicionar vários endereços para os alertas serem enviados. Se este campo for
deixado em branco, os alertas ainda estarão visíveis no histórico de alertas do Server
Monitoring.
Você também pode editar ou excluir um alerta, clicando em Editar ou Remover botões.
Notificações
Uma vez que você tenha configurado um alerta em seu servidor ou site, o Server Monitoring
monitorará de perto a métrica escolhida e enviará um e-mail assim que o limite alvo for atingido
ou excedido. O Server Monitoring também enviará um e-mail quando essa métrica voltar ao
normal.
Você pode verificar alertas históricos clicando em Histórico título de Alertas seção na página
inicial.

---
*Página 11*

Você verá uma lista de alertas acionados, com o título do alerta, o servidor ou site monitorado, o
início do alerta e seu fim (se vazio, o alerta ainda está acionado).
Você pode excluir uma ou mais linhas de histórico clicando em Remover botão.
Voltar ao Topo

---
*Página 13*

Como os dados são salvos e posso acessá-
los a partir das minhas próprias aplicações?
No monitoramento de servidor, todos os seus dados são salvos em um formato aberto. Usamos
um banco de dados SQL Server para armazenar dados globais e específicos de servidores e
sites.
Se você tiver uma ferramenta instalada que possa ler arquivos de banco de dados do SQL
Server (por exemplo, SQL Server Management Studio, SQL Server Management Studio
Express, etc.), você pode acessar os dados a partir daí.
Mesmo que você possa acessar esses arquivos tanto em modo de leitura quanto de gravação,
recomendamos que você sempre use o modo de acesso somente leitura, a fim de evitar
qualquer conflito entre o Server Monitoring e suas próprias aplicações.
Não hesite em nos contatar se quiser saber mais sobre o desenvolvimento de suas próprias
aplicações usando dados de Server Monitoring.

---
*Página 14*

Como usar um banco de dados externo?
Você pode usar um banco de dados localizado em um servidor diferente daquele onde o Server
Monitoring está instalado. A instância do SQL Server deve já estar instalada na máquina de
destino, e você deve ter privilégios administrativos sobre ela.
Os passos são os seguintes:
1. Configurar o banco de dados externo
2. Configurar o Monitor de Servidor para usar o banco de dados externo
Configurar o banco de dados externo
No Gerenciador de Configuração do SQL Server, para a instância correspondente, o TCP/IP
deve estar habilitado.
NOTAS: Certifique-se de que seu servidor seja acessível através de TCP porta 49237 caso
contrário, você pode precisar criar um novo regra de entrada no firewall.
No SQL Server Management Studio, crie um novo login para Monitoramento de Servidor.

---
*Página 15*

Selecionar autenticação do SQL Server , em seguida, especifique o nome de usuário e
senha Certifique-se de manter essas credenciais, elas serão necessárias durante a
configuração do Server Monitoring.

---
*Página 16*

O login deve ter pelo menos o público função do servidor. Além disso, atribua a dbcreator
papel se o banco de dados ainda não foi criado.

---
*Página 17*

Na aba de segurança, certifique-se de que a autenticação esteja configurada para permitir
ambos. SQL Server e Autenticação do Windows .
Configurar Monitoramento de Servidor
Configurar o Monitoramento do Servidor depende de uma instalação existente já estar presente.
Se o Server Monitoring ainda não estiver instalado

---
*Página 18*

Siga o procedimento de instalação padrão , exceto que no Nome da Instância campo, você
deve fornecer as informações de conexão (nome da instância e porta) para a instância remota
do SQL Server.
Por exemplo, se você estiver instalando TSplus-SM em uma máquina virtual e quiser usar um
banco de dados hospedado em DV , entrar dv.tsplus.net,49237\SQLExpress ou
54.36.189.128,49237\SQLExpress
(é uma vírgula, entre o endereço do servidor e a porta, e não um dois-pontos)
Se o Server Monitoring já estiver instalado
Se o Server Monitoring já estiver instalado, basta atualizar o NomeDaInstância chave de
registro em: Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Digital River\ServerMonitoring
Você também pode atualizar o NomeDoBancoDeDados se você quiser usar um nome de
banco de dados diferente do padrão.
Finalmente, reiniciar o serviço de dados do TSplus-ServerMonitoring para que a instalação
do banco de dados possa ser feita (criação das tabelas e outros objetos).

---
*Página 19*

Instalação
Executar o programa de configuração do Server Monitoring e depois siga os passos de
instalação .
Nota: O Windows solicitará que você execute a configuração como Administrador.
Clique em "Próximo".

---
*Página 20*

Escolha se deseja a instalação recomendada ou a instalação avançada.
Se você escolher a instalação avançada, terá algumas opções de configuração extras:
A opção Avançada permite que você:

---
*Página 21*

Use configurações de proxy personalizadas.
Baixe o instalador sem executá-lo, o que não instala o Server Monitoring.
Você pode escolher instalar o Server Monitoring em um local personalizado.

---
*Página 22*

Server Monitoring usa um banco de dados SQL Server para armazenar todos os dados
provenientes dos seus servidores monitorados.
Você pode usar a Instância Padrão do SQL Server, ou escolha outra instância se você já tiver o
SQL Server instalado .

---
*Página 23*

Por favor, clique em "Eu concordo" para aceitar o contrato de licença.
A configuração agora fará o download de todos os pré-requisitos.

---
*Página 24*

Por favor, seja paciente Pode levar alguns minutos para instalar completamente o software e
seus pré-requisitos.
NOTA: Você pode ser solicitado a reiniciar seu computador antes de usar Server Monitoring.
Agora você pode abrir o Server Monitoring clicando no atalho criado na sua área de trabalho.
Você será recebido pela tela inicial do Console de Administração:

---
*Página 25*

A avaliação gratuita do Server Monitoring é uma licença completa de 15 dias.

---
*Página 26*

O monitoramento do servidor indica que o
consumo de CPU está mais alto do que o
esperado. O que posso fazer?
1. Verifique se há atualizações
Por favor, verifique regularmente se há atualizações, pois a maioria delas oferece melhorias de
desempenho. Recomendamos que você aplique as atualizações do Server Monitoring fora do
horário de trabalho, pois a atualização pode realizar operações em segundo plano de longa
duração no banco de dados.
A versão mais recente do Server Monitoring está sempre disponível aqui: link direto .
2. Aplicar configuração recomendada
Um banco de dados sempre utilizará todos os recursos de computação disponíveis para concluir
as solicitações o mais rápido possível. Portanto, é recomendável planejar os recursos para o
seu servidor de Server Monitoring de acordo com seu uso.
Por favor, encontre abaixo nossas recomendações com base no número de servidores
monitorados:
Servidores monitorados CPU Memória (RAM)
1-2 2 8
3-4 4 16
5+ 8 32
Instalar o Server Monitoring em um disco do tipo SSD é recomendado para melhor
desempenho.
Além disso, pode ser necessário alocar espaço em disco adicional para o seu Servidor de
Monitoramento, dependendo do número de servidores e sites monitorados, e da quantidade de
dados coletados e armazenados no banco de dados SQL Server.

---
*Página 27*

Finalmente, observe que geralmente é uma boa ideia executar um aplicativo de monitoramento,
como Server Monitoring, em um servidor dedicado. Isso impede que outros aplicativos reduzam
os recursos disponíveis.
3. Entre em contato com o nosso suporte ao cliente
Se todas as recomendações acima não fornecerem uma experiência aceitável com Server
Monitoring, não hesite em entrar em contato com nosso suporte ao cliente em https://
terminalserviceplus.freshdesk.com Ficaremos felizes em ajudar a solucionar problemas com a
sua instalação do Server Monitoring.
Para facilitar nosso suporte técnico e reproduzir seu problema, podemos solicitar uma
exportação do seu banco de dados.
Para fazer isso, abra um prompt de comando elevado, digite o seguinte comando:
sqlcmd -S [Seu Nome de Instância do SQL Server] -Q “BACKUP DATABASE [ServerMonitoring]
TO DISK = N’ServerMonitoring_Support.bak’ WITH NOFORMAT, NOINIT, NAME = ‘demodb-
full’, SKIP, NOREWIND, NOUNLOAD, STATS = 10”
Uma vez que a exportação tenha terminado, por favor, envie-nos o arquivo localizado em C:
\Program Files (x86)\Microsoft SQL
Server[YourVersionOfSQLServer]\MSSQL\Backup\ServerMonitoring_Support.bak .

---
*Página 28*

Pré-requisitos
Simulador de Arquitetura
Configure sua arquitetura online para ajudá-lo a escolher nosso software e complementos.
TSplus Architecture Simulator
Requisitos de Hardware
Requisitos de Processador e Memória com base no número de servidores monitorados:
Servidores monitorados Núcleos de CPU Memória (RAM)
1-2 2 8
3-4 4 16
5+ 8 32

---
*Página 29*

NOTAS:
Instalar o Server Monitoring em um disco SSD é recomendado para melhor desempenho.
Certifique-se de alocar espaço em disco suficiente no servidor que hospeda o Console de
Administração. A quantidade de dados coletados e o tamanho do banco de dados SQL
dependerão de quantos servidores estão sendo monitorados.
As melhores práticas indicam que é ideal executar o Server Monitoring em um servidor
dedicado. Isso impede que outros aplicativos reduzam os recursos disponíveis para sua
plataforma de monitoramento.
Sistema Operacional
Seu hardware deve usar um dos sistemas operacionais abaixo:
Windows 7 Pro
Windows 8/8.1 Pro
Windows 10 Pro
Windows 11 Pro
Windows Server 2008 SP2/Small Business Server SP2 ou 2008 R2 SP1
Windows Server 2012 ou 2012 R2
Windows Server 2016
Windows Server 2019
Windows Server 2022
Windows Servidor 2025
Ambas as arquiteturas de 32 e 64 bits são suportadas.
Os agentes (servidores que são monitorados) podem ser sistemas operacionais Linux ou
Windows. Os agentes Linux foram testados até agora nas distribuições Ubuntu e Debian. Se
você tiver um servidor com outra distribuição e encontrar problemas para instalar o agente, entre
em contato conosco.
Rede
Apenas uma porta de rede é necessária: porta 7778, que não é uma porta oficialmente
registrada e, portanto, não está atribuída a serviços específicos.

---
*Página 31*

Comece com o Monitoramento de Servidor
Passo 1: Instalando o Server Monitoring no seu
computador
Instalar o Server Monitoring é um processo fácil.
Basta baixar o instalador (Setup-TSplus-ServerMonitoring.exe) de nosso site e siga os passos
detalhados aqui .
Os arquivos são descompactados e copiados para as seguintes pastas:
C:\Program Files\TSplus-ServerMonitoring (sistemas de 32 bits)
C:\Program Files\ServerMonitoringAgent (sistemas de 32 bits)
C:\Program Files (x86)\TSplus-ServerMonitoring (sistemas de 64 bits)
C:\Program Files (x86)\ServerMonitoringAgent (sistemas de 64 bits).
A avaliação gratuita é totalmente funcional com uma licença de 15 dias.
Após a instalação, haverá um novo atalho na sua Área de Trabalho:

---
*Página 32*

Passo 2: Verificando sua Instalação
A instalação do Server Monitoring vem em 2 partes :
O Console de Administração de Monitoramento de Servidor - A principal interface de
Monitoramento de Servidor, onde um administrador pode visualizar informações e criar
relatórios sobre a saúde e a atividade do servidor.
O Agente de Monitoramento do Servidor - Um pequeno programa instalado em cada servidor
monitorado. O Agente coleta dados críticos e os envia para o Console de Administração de
Monitoramento do Servidor.
Quando o Console de Administração do Server Monitoring é instalado, o Agente também é. Isso
significa que, ao abrir o Server Monitoring pela primeira vez, você verá imediatamente a
máquina local listada como um Servidor Monitorado na tela inicial.
Para abrir o Console de Administração, clique no atalho da área de trabalho do Server
Monitoring. Você será recebido por uma tela inicial que se parece com isso:

---
*Página 33*

Você pode ver um servidor configurado (o servidor onde você instalou Server Monitoring) e um
site configurado ( www.example.com ).
Próximos passos
Para mais detalhes sobre Server Monitoring, por favor, leia o documentação online completa .
Não hesite em contate-nos se você tiver perguntas ou feedback sobre Server Monitoring e/ou
este guia de início rápido.

---
*Página 34*

Como fazer: adicionar filtros em um relatório
personalizado
Você pode adicionar um ou vários filtros aos dados em um relatório. Por exemplo, no relatório
de "Uso de Aplicativos", você pode querer filtrar pelo nome do aplicativo. Vamos filtrar os
aplicativos cujo nome começa com "Microsoft".
Primeiro, selecione os filtros do relatório:
Então, uma janela é aberta com a lista de filtros atuais. Você sempre terá um filtro com nomes
de servidores ou nomes de sites, é obrigatório, por favor, ignore-o (você pode removê-lo, mas
então ele será adicionado novamente automaticamente).
Clique no botão ”+” para adicionar um filtro.

---
*Página 35*

Escolha o campo no qual deseja aplicar o filtro (neste caso, o nome do processo), e depois o
operador de filtro e o valor:
Em seguida, clique em "OK", salve o relatório personalizado e acesse-o para ver os resultados
filtrados:

---
*Página 37*

Como: Alterar o tipo de gráfico de um
relatório personalizado
Você pode alterar o tipo de gráfico exibido em um relatório:
Primeiro, selecione o gráfico que deseja alterar, em seguida clique em o configurações botão,
e clique em Executar designer :
Em seguida, clique no botão “Alterar tipo”:

---
*Página 38*

Escolha o novo tipo:
Clique em OK e veja as modificações aplicadas:

---
*Página 39*

Você também pode, neste formulário, personalizar o conteúdo do gráfico (título, legenda,
anotações etc.)

---
*Página 40*

Como: Alterar cores de um relatório
personalizado
Se você quiser mudar as cores das séries em um gráfico:
Selecione o gráfico que você deseja alterar, em seguida clique em o configurações botão, e
clique em Paletas :
Então escolha uma paleta existente ou crie a sua própria:

---
*Página 41*

Clique em OK e veja as modificações aplicadas:

---
*Página 42*

Você também pode personalizar o conteúdo do datagrid (cores, bordas, fontes, etc.) Basta
selecionar a(s) célula(s) que deseja modificar e alterar as propriedades que deseja.

---
*Página 44*

Como: Alterar o logotipo de um relatório
personalizado
Para mudar o logotipo de um relatório personalizado, você pode clicar no logotipo atual e, em
seguida, clicar no configurações botão, e mude o Fonte da Imagem campo:
Então, salve e veja as modificações aplicadas:

---
*Página 46*

Como: Alterar a visibilidade de algumas
informações no relatório personalizado
Você pode estar interessado apenas em alguns indicadores em um relatório. Você pode ocultar
os outros clicando nos campos correspondentes e, em seguida, no Propriedades de
comportamento , você pode marcar o Coluna Visível caixa de seleção:
Então, no Visão do Designer , você verá os campos desativados:

---
*Página 47*

E no Visualização de prévia , você verá os campos ocultos:

---
*Página 49*

Como usar banco de dados existente para
relatórios personalizados:
Quando você personaliza um relatório existente ou cria um novo, você usará dados de
monitoramento que estão armazenados no banco de dados que você construiu durante a
configuração, e que são alimentados regularmente pelos dados de todos os servidores e sites
que você monitora.
Você pode ver 2 tipos de dados que você pode usar:
tabelas, que são dados "puros" à medida que chegam dos servidores que você monitora

---
*Página 50*

procedimentos armazenados, que são um agregado de muitas tabelas, que foram feitos para
a necessidade de um relatório ou um painel de controle

---
*Página 51*

Você pode usar um ou outro, de acordo com suas necessidades. Se você está acostumado com
o SQL Server Management Studio, pode até criar seus próprios procedimentos armazenados e
usá-los em seus relatórios personalizados.

---
*Página 52*

Personalizar Relatórios (Usuários
Avançados)
Com o Server Monitoring, você tem vários relatórios padrão que nossa equipe forneceu como
modelos. No entanto, em certos casos, você pode querer um relatório específico que não é
fornecido pela nossa equipe.
Se você acha que outros clientes além de você podem estar interessados neste relatório, entre
em contato com nossa equipe de suporte e tentaremos adicioná-lo à lista de relatórios padrão,
se for elegível.
Se for uma alteração muito específica que você precisa, pode ser interessante personalizar um
relatório existente ou até mesmo criar um novo (para usuários avançados).
Para personalizar um relatório existente: primeiro selecione um relatório (site ou servidor)
clicando em um bloco de Servidor, depois escolhendo um relatório no menu à esquerda.
Em seguida, clique em o Personalizar botão:

---
*Página 53*

Um designer de relatórios aparecerá:
Quando você fez todas as modificações que desejava, clique em Salvar botão, e dê um nome
amigável ao seu relatório personalizado:

---
*Página 54*

Seu relatório personalizado estará disponível no menu à esquerda, e você pode selecioná-lo
para visualizá-lo.

---
*Página 55*

Aqui estão alguns exemplos de modificações fáceis que você pode fazer em um relatório:
Alterar um logotipo
Mudar cores
Alterar tipo de gráfico
Filtre seus dados
Alterar visibilidade das informações
Aqui está como você pode usar os dados existentes no banco de dados de Server Monitoring:
Use dados do banco de dados

---
*Página 57*

Exportar e Imprimir Relatórios
Primeiro, selecione um relatório (site ou servidor) clicando em um bloco de Servidor e, em
seguida, escolhendo um tipo de relatório no menu à esquerda.
Escolha os parâmetros que melhor lhe convêm, em seguida clique em Exportar/Imprimir
botão:

---
*Página 58*

Uma ferramenta de visualização aparecerá:
Dentro do menu e da barra de ferramentas, você tem inúmeras ações possíveis:
Pesquisar dentro do relatório

---
*Página 59*

Salve o documento como está (no formato .prnx, isso não será útil na maioria dos casos)
Imprimir ou imprimir rapidamente o documento
Configuração da página (margens, orientação, etc.)
Escolha uma cor de fundo
Insira uma marca d'água (texto ou imagem)
Exporte o documento em vários formatos (PDF, HTML, MHT, RTF, DocX, XLS, XLSX, CSV,
arquivo de texto, arquivo de imagem)
Envie o documento por e-mail em vários formatos (PDF, MHT, RTF, DocX, XLS, XLSX, CSV,
arquivo de texto, arquivo de imagem)
Ao exportar em algum formato, por exemplo Excel, você pode escolher algumas opções:
Então você precisa escolher onde salvar o arquivo e se gostaria de abri-lo após salvar.

---
*Página 60*

Agora você tem um arquivo Excel que pode editar à vontade!

---
*Página 62*

Agendamento de envio de relatórios por e-
mail
Primeiro, selecione um relatório (site ou servidor) clicando em um bloco de Servidor e, em
seguida, escolhendo um tipo de relatório no menu à esquerda.
Clique em o Agendar envio de e-mails botão:

---
*Página 63*

Uma nova forma aparecerá:

---
*Página 64*

Apenas preencha os seguintes campos:
1. O tipo de arquivo de saída (PDF, Excel ou HTML).
2. A data da primeira exportação.
3. A frequência de exportação (a cada hora / 4 horas / 8 horas / 12 horas / dia / semana / mês).
4. O(s) endereço(s) de e-mail para enviar o relatório. Por favor, separa vários endereços de e-
mail com uma vírgula.
5. Os servidores/sites da web envolvidos no relatório.
6. O período de tempo para o relatório (última hora / últimas 4 horas / últimas 8 horas / últimas
12 horas / hoje / ontem / últimos 7 dias / últimos 30 dias / últimos 90 dias / últimos 180 dias).
Clique em Validar para salvar o cronograma.
Para editar o cronograma, clique novamente em o Agendar envio de e-mails botão.
Os recursos de envio de e-mails do Relatório do Servidor e Agenda estão desacoplados: Os
critérios de filtro definidos na página do relatório se aplicam apenas à exportação e não à
entrega de e-mails agendada.

---
*Página 65*

Recursos em tempo real do servidor
Para ter acesso a recursos em tempo real para servidores, clique no bloco “Em tempo real” na
seção Servidores:
Desempenho
Isso exibe uma visão geral do desempenho do seu servidor (CPU, Memória, Gravação em disco
e Leitura em disco) nos últimos 10 minutos:

---
*Página 66*

Uso do processo
Ao clicar em “Processar uso” no menu à esquerda, você verá uma tabela mostrando os
processos atualmente utilizados no servidor selecionado e alguns indicadores-chave:

---
*Página 67*

Você pode filtrar por servidor.
Largura de banda
Ao clicar em "Largura de banda" no menu à esquerda, você verá uma tabela mostrando o uso
da largura de banda (para cima e para baixo) do servidor selecionado:

---
*Página 68*

Usuários
Ao clicar em "Usuários" no menu à esquerda, você verá uma tabela e um gráfico mostrando os
usuários atualmente conectados ao servidor selecionado:

---
*Página 70*

Relatório de uso de aplicativo por servidor e
usuário
Este relatório está disponível clicando em Servidores > Relatórios azulejo, depois no Uso de
aplicativos por servidor e usuário link do menu à esquerda
O Relatório de uso de aplicativo por servidor e usuário exibe o uso do aplicativo por
usuário para o(s) servidor(es) especificado(s) e período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 71*

Relatório de Uso de Aplicação por Servidor
Este relatório está disponível clicando em Servidores > Relatórios , então em Uso de
aplicativos por servidor no menu à esquerda.
O Relatório de uso de aplicativo por servidor exibe o uso da aplicação para o(s)
servidor(es) especificado(s) e período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 72*

Relatório de Desempenho Médio do Servidor
Este relatório está disponível clicando em Servidores > Relatórios , então em Desempenho
médio no menu à esquerda.
O Relatório de desempenho médio do servidor exibe o desempenho médio (CPU, Memória
e uso de Disco) para o(s) servidor(es) e período de tempo especificado(s).
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 73*

Relatório de Sessões Concorrentes do
Servidor
Este relatório está disponível clicando em Servidores > Relatórios , então em Sessões
concorrentes por hora no menu à esquerda.
O Relatório de sessões simultâneas do servidor exibe o número de sessões simultâneas
para o(s) servidor(es) especificado(s) e período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 74*

Recursos do Relatório do Servidor
Para ter acesso aos recursos de relatórios, clique no bloco "Relatórios" na seção Servidores:
Você verá esta tela:

---
*Página 75*

Você pode ver 5 áreas diferentes:
1. Relatórios padrão Esta é uma lista de relatórios padrão, fornecidos por padrão com a
instalação do Server Monitoring. Você pode clicar em qualquer um deles para ver o relatório.
2. Relatórios personalizados Aqui você pode adicionar seus próprios relatórios, adicionando
novas colunas ao relatório, imagens personalizadas etc. A lista de relatórios é exibida aqui.
Você pode clicar em qualquer um deles para ver o relatório.
3. Ações em relatórios Aqui você pode exportar/imprimir relatórios, personalizá-los, agendar o
envio por e-mail ou excluí-los, se forem relatórios personalizados.
4. Filtros Você pode filtrar os relatórios por servidor e por data.
5. Prévia do relatório Você pode visualizar o relatório atualmente selecionado.
Os recursos de envio de e-mails do Relatório do Servidor e Agenda estão desacoplados: Os
critérios de filtro definidos na página do relatório se aplicam apenas à exportação e não à
entrega de e-mails agendada.

---
*Página 76*

Relatório de Uso da Rede
Este relatório está disponível clicando em Servidores > Relatórios , então em Uso da Rede
no menu à esquerda.
O Relatório de Uso da Rede exibe o uso da rede para o(s) servidor(es) especificado(s) e
período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 77*

Relatório de Presença do Usuário
Este relatório está disponível clicando em Servidores > Relatórios , então em Participação
do Usuário no menu à esquerda.
O Relatório de Presença do Usuário exibe a presença do usuário para o(s) servidor(es)
especificado(s) e período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 78*

Relatório de presença do usuário
Este relatório está disponível clicando em Servidores > Relatórios , então em Presença do
usuário no menu à esquerda
O Relatório de Presença do Usuário exibe a presença do usuário para o(s) servidor(es)
especificado(s) e período de tempo.
Os dados podem ser filtrados por nome do servidor e intervalo de datas.

---
*Página 79*

Gerenciamento de Servidor
Você pode visualizar, editar e remover servidores monitorados a partir da tela inicial.
Para editar um servidor, passe o mouse sobre o bloco correspondente e clique no ícone de
edição:
Uma caixa de diálogo aparecerá. Aqui você pode editar:
O alias do servidor
A URL do Servidor
O nome do host do servidor e o endereço IP.
A porta RDP do servidor. Por padrão, é 3389
Clique em validar para salvar suas alterações.

---
*Página 80*

Para remover um servidor clique em o X ícone ao passar o mouse sobre o bloco do servidor
que você deseja remover. Você será solicitado a confirmar sua escolha. NOTA: deletar um
servidor excluirá todos os dados associados a este servidor: desempenho, atividade do usuário,
alertas, etc…
Adicionar um novo servidor clique no bloco “Adicionar novo servidor” na página inicial:

---
*Página 81*

Server Monitoring apresentará as opções para adicionar um servidor Windows:
Você tem duas maneiras diferentes de adicionar um novo servidor Windows para monitorar:
Faça login no servidor que você gostaria de monitorar e navegue até: http://
YourMonitoringServerUrl:7778/download/Setup-Agent.exe
você também pode baixar diretamente o agente e enviá-lo para o servidor que você gostaria
de monitorar.

---
*Página 82*

Você pode agora iniciar o arquivo Setup-Agent.exe e instalá-lo.
Aceite a licença e clique em próximo

---
*Página 83*

Aqui você pode alterar a localização dos arquivos instalados.

---
*Página 84*

Insira a URL do servidor principal onde o Server Monitoring está instalado. Não altere o número
da porta (7778). Em seguida, clique em próximo. A instalação do Agente leva apenas um
momento.
O servidor que você acabou de adicionar aparecerá em sua lista de servidores monitorados em
breve. Não se preocupe se o novo servidor aparecer offline.

---
*Página 85*

Após alguns momentos de coleta de dados no novo servidor, ele aparecerá ativo e online no
Server Monitoring.
Você também pode monitorar um servidor Linux:

---
*Página 86*

Conforme indicado, você só precisa:
inicie um Terminal no servidor Linux que você deseja monitorar
copie o comando e execute-o no Terminal
Então, seu novo servidor Linux deve aparecer:

---
*Página 87*

Voltar ao Topo

---
*Página 88*

Configurações
Você pode gerenciar as configurações de Server Monitoring clicando no bloco “Configurações
Gerais”:
As configurações a seguir serão exibidas:

---
*Página 89*

Você pode configurar um servidor SMTP para poder enviar e-mails automáticos (para
relatórios e alertas)
Você pode definir um assunto e corpo personalizados para o envio de relatórios por e-mail.
Use o botão “Testar Configurações SMTP” para ter certeza de que suas informações SMTP
estão corretas.
Para mais informações sobre alertas, vá aqui
Para mais informações sobre o envio de relatórios por e-mail, vá aqui

---
*Página 90*

Desinstalar
Se você deseja desinstalar o Server Monitoring, pode fazê-lo seguindo os passos abaixo:
1.
Vá para Aplicativo e configurações , e procure por Server Monitoring.
2.
Desinstale ambos TSplus ServerMonitoring e Agente de Monitoramento de Servidor .
3. TSplus ServerMonitoring usa um SQL Server banco de dados para armazenar seus dados.
Durante a desinstalação do Server Monitoring, instâncias e bancos de dados do SQL Server
são não excluído, porque você pode querer manter seus dados, e você também pode usar
instâncias do SQL Server para outros fins. Se não for o caso, e você quiser desinstale
também as instâncias e bancos de dados do SQL Server , você pode fazer isso
pesquisando o Microsoft SQL Server e desinstalando o seguinte:

---
*Página 92*

Atualizando o Monitoramento do Servidor
Confira nossas correções e melhorias clicando em Registro de alterações
Executar o programa de lançamento de atualização do Server Monitoring, disponível aqui e
siga os passos de instalação .
NOTA: O Windows solicitará que você instale a atualização como Administrador.
Clique em "Próximo".

---
*Página 93*

Escolha o método de instalação apropriado para sua implantação.
Clique em "Eu concordo" para aceitar o contrato de licença.

---
*Página 94*

A atualização está agora completa. Você pode começar a usar a versão mais recente do Server
Monitoring.
NOTA: Dependendo do conteúdo do pacote de atualização, pode ser solicitado que você
reinicie seu servidor.

---
*Página 95*

Recursos em tempo real do site
Para ter acesso a recursos em tempo real para sites, clique no bloco “Em tempo real” na seção
Websites:
VISÃO GERAL
Isto exibe uma visão geral do tempo de atividade do seu site nos últimos 30 dias:

---
*Página 96*

Desempenho
Ao clicar em "Desempenho" no menu à esquerda, você verá um gráfico de pizza mostrando o
tempo de atividade/inatividade do site selecionado e alguns indicadores-chave:

---
*Página 97*

Você pode filtrar os resultados por:
Nome do site:
Intervalo de tempo :

---
*Página 99*

Relatório de Disponibilidade do Site
Este relatório está disponível clicando em Sites > Relatórios tile, em seguida clique em
Disponibilidade no menu à esquerda.
O Relatório de Disponibilidade do Site exibe o tempo de atividade em porcentagem para o
site e período de tempo especificados.
Os dados podem ser filtrados pelo nome do site e intervalo de datas.

---
*Página 100*

Recursos do Relatório do Site
Para acessar o recurso de relatórios para sites monitorados, clique no bloco "Relatórios" na
seção Websites:
Você verá esta tela:

---
*Página 101*

Você pode ver 5 áreas diferentes:
1. Relatórios padrão Esta é uma lista de relatórios padrão fornecidos por padrão com a
instalação do Server Monitoring. Você pode clicar em qualquer um deles para ver o relatório.
2. Relatórios personalizados Aqui você pode criar seus próprios relatórios, adicionando
novas colunas ao relatório, imagens personalizadas etc. A lista de relatórios é exibida aqui e
você pode clicar em qualquer um deles para ver o relatório.
3. Ações em relatórios Você pode exportar/imprimir relatórios, personalizá-los, agendar o
envio por e-mail ou excluí-los.
4. Filtros Aqui você pode filtrar os relatórios por site e por data.
5. Prévia do relatório Visualizar o relatório atualmente selecionado.
Para saber mais sobre os relatórios de Server Monitoring, por favor, leia esta documentação .
NOTA: O procedimento é o mesmo para relatórios de servidor e relatórios de site.

---
*Página 102*

Códigos de tempo de resposta do site
Relatório
Este relatório está disponível clicando em Sites > Relatórios azulejo, depois no Tempo de
resposta link do menu à esquerda
O Relatório de tempo de resposta do site exibe o tempo de resposta máximo, médio e
mínimo em milissegundos para o site e período de tempo especificados.
Os dados podem ser filtrados pelo nome do site e intervalo de datas.

---
*Página 104*

Relatório de Códigos de Resposta do Site
Este relatório está disponível clicando em o Sites > Relatórios tile, em seguida clicando
Resposta no menu à esquerda
O Relatório de Resposta do Site exibe os códigos de resposta para o site especificado e o
período de tempo.
Os dados podem ser filtrados pelo nome do site e intervalo de datas.

---
*Página 105*

Gestão de Site
O Tela inicial exibe a lista de sites monitorados. É também onde você adicionar um novo
site monitorar, editar ou remover sites da plataforma de monitoramento.
Para adicionar um novo site para monitorar, clique em Adicionar novo site .
Na caixa de diálogo que aparece, insira o nome amigável para o site e sua URL.

---
*Página 106*

Clique em Validar para continuar. Você verá o novo site aparecer na lista de sites monitorados:
Após um curto momento, o novo site será analisado e aparecerá verde (responsivo) ou
vermelho (não responsivo):

---
*Página 107*

Para editar um site existente, passe o mouse sobre o bloco do site e clique no botão Editar:
Você também pode excluir um site existente: basta passar o mouse sobre o bloco do site e
clicar no botão Excluir.

---
*Página 108*

NOTA: Isso excluirá quaisquer dados associados a este site (alertas, tempo de resposta, etc.)
Você também pode ir ao site, clicando no terceiro botão:

---
*Página 109*

Voltar ao Topo