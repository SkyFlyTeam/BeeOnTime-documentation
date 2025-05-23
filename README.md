![3° Sprint](https://github.com/user-attachments/assets/f2a750b5-2745-45b3-abb9-31c738f576ad)

<br>

<p align="center">
    <a href="#objetivos"> Objetivos da Sprint </a> &nbsp |&nbsp &nbsp
    <a href="#entregas"> Entregas </a> &nbsp |&nbsp &nbsp
    <a href="#metricas"> Métricas do Time </a>  &nbsp |&nbsp &nbsp  
    <a href="#backlog"> Backlog da Sprint </a>  &nbsp |&nbsp &nbsp  
    <a href="#links"> Links úteis </a>
</p>

Durante esta sprint, nosso principal foco foi o desenvolvimento de relatórios voltados para a análise de marcações de ponto pelos administradores e gestores. Esses relatórios permitem identificar ausências, falhas nas marcações e o comportamento de registro ao longo do dia.

Também implementamos um calendário que exibe um resumo diário dos diferentes tipos de faltas, além de permitir a gestão de feriados e a concessão de folgas coletivas.

Por fim, implementamos o espelho de ponto, sendo possível gerar um arquivo PDF do documento e realizar a assinatura do mesmo ao confirmar seus dados de cadastro.

<span id="objetivos">

# 🎯 Objetivos da Sprint
Os requisitos funcionais atendidos nesta sprint foram:

- ✔️ **RFN06. Controle de Férias e Folgas:** <br /> O sistema permite o agendamento de férias e folgas pelos administradores e também permite solicitações pelos funcionários. Após a aprovação, o sistema registra automaticamente a ausência no calendário da empresa. <br /> <br />
- ✔️ **RFN07. Relatórios de Ponto:** <br />   O sistema gera relatórios detalhados sobre registros de ponto, horas extras, banco de horas, ausências, atrasos e falhas em marcações, permitindo filtros por colaborador e período. <br /> <br />
- ✔️ **RFN08. Espelho de Ponto:** <br /> O sistema gera o espelho de ponto detalhado de cada funcionário, permitindo a assinatura para validação formal e a disponibilização de uma cópia para conferência. <br /> <br />
- ✔️ **RFN09. Calendário da Empresa:** <br /> O sistema permite definir os dias que serão folgas para todos os funcionários, permitindo a configuração de feriados facultativos conforme as regras da empresa. <br /> <br />
- ✔️ **RFN10. Notificações e Alertas:** <br /> O sistema envia alertas aos funcionários e gestores sobre eventos importantes, como falhas no registro de ponto, necessidade de justificativa de ausência, solicitações pendentes de ajustes e atualizações no banco de horas. <br /> <br />
- ✔️ **RFN11. Filtros de Pesquisa e Visualização:** <br /> O sistema disponibiliza filtros de pesquisa e visualização em suas telas, permitindo a personalização das informações exibidas. Os filtros devem possibilitar a seleção de dados específicos, como período, colaborador, status, tipo de evento (ausência, atraso, horas extras, etc.) e outras variáveis relevantes, para facilitar a análise e o gerenciamento das informações <br /> <br />

<br> 

<span id="entregas">

# 📲 Entregas

### RFN06. Controle de Férias e Folgas:
O sistema de solicitações de férias e folgas foi finalizado.<br />
Entre as funcionalidades entregues:
- Solicitação de folgas utilizando o banco de horas ou com desconto de horas.
- Marcação de datas para folgas, com necessidade de aprovação do gestor/administrador.
- Solicitação de férias nos formatos permitidos (30 dias, 15 + 15 dias, 20 + 10 dias ou 10 + 15 + 5 dias), também com aprovação requerida.

### RFN07. Relatórios de Ponto:
Com o objetivo de oferecer maior visibilidade e controle sobre a jornada dos colaboradores, foram desenvolvidos relatórios que centralizam e facilitam a análise de dados de ponto em toda a empresa. Esses relatórios auxiliam gestores e administradores na identificação de padrões de comportamento, ausências e falhas no registro de ponto. <br />
- **Relatório de Pontos Diários:** apresenta a lista de colaboradores com seus respectivos status (Presente, Ausente, em Férias ou em Folga), incluindo a data prevista de retorno. Também exibe os horários de ponto registrados ao longo do dia.
- **Relatório de Ausências:** traz um gráfico de pizza com a distribuição percentual e quantitativa dos tipos de ausência (folgas, licenças médicas, férias, ausências justificadas e não justificadas). Ao lado, uma tabela detalha os colaboradores que apresentaram ausências, com os respectivos tipos e quantidades.
- **Relatório de Falhas em Marcações:** disponibiliza gráficos comparativos entre marcações pontuais e com atraso, além de um gráfico sobre solicitações de ajuste em relação aos pontos registrados corretamente. Inclui também uma tabela com os casos de atraso, informando o horário previsto, o horário real de marcação e o tempo de atraso.

### RFN08. Espelho de Ponto:
Foi implementada a funcionalidade de visualização e assinatura do espelho de ponto mensal. Agora, os colaboradores têm acesso à lista de espelhos já assinados, com indicação daqueles que ainda estão com a assinatura pendente. <br />
Ao iniciar o processo de assinatura, é possível visualizar o PDF contendo todos os registros de ponto do mês, o total de horas trabalhadas e o saldo acumulado no banco de horas. Para validar a assinatura, é necessário confirmar o CPF e a senha da conta. <br />
Além disso, o PDF assinado pode ser baixado para fins de registro e consulta.

### RFN09. Calendário da Empresa:
Foi desenvolvido um calendário corporativo que oferece uma visão da presença dos colaboradores ao longo do mês. A interface exibe, em cada dia, a quantidade de colaboradores em férias, em folga ou ausentes, com os totais destacados diretamente abaixo da data. <br />
Ao selecionar um dia específico, é possível visualizar a lista detalhada dos colaboradores vinculados a cada uma dessas situações. <br />
Além disso, o calendário permite a configuração de feriados, com a opção de definir se a empresa irá operar normalmente ou não nessas datas. Também é possível conceder folgas coletivas de forma prática e centralizada por meio da própria interface do calendário.

### RFN10. Notificações e Alertas:
Foi implementado um sistema de notificações automáticas para manter todos os perfis de usuários informados sobre eventos relevantes relacionados à gestão de ponto e ausências. As notificações foram desenvolvidas com base nas principais necessidades de funcionários, gestores e administradores, garantindo mais agilidade no acompanhamento e tomada de decisões. <br />
As principais notificações implementadas são:
- **Justificativas de ausência pendentes:** funcionários e gestores recebem alertas quando há justificativas que ainda não foram enviadas, como lembrete para regularização.
- **Solicitações aprovadas ou reprovadas:** funcionários e gestores são notificados sempre que uma solicitação (como ajuste de ponto, justificativa, etc.) for aprovada ou rejeitada, facilitando o acompanhamento.
- **Esquecimento de marcação de ponto:** caso o colaborador esqueça de registrar o ponto, uma notificação é enviada como lembrete.
- **Definição de folgas:** sempre que uma folga for atribuída, funcionários e gestores recebem um aviso, garantindo que todos estejam cientes de alterações na escala.
- **Solicitações pendentes:** administradores e gestores recebem alertas sobre novas solicitações pendentes de análise, ajudando a manter o fluxo de aprovações em dia.
- **Justificativas de falta recebidas:** sempre que um colaborador enviar uma justificativa, administradores e gestores são notificados para que possam acompanhar e tomar as medidas necessárias.

### RFN11. Filtros de Pesquisa e Visualização:
Foram implementados filtros em todas as telas do sistema, permitindo ao usuário ajustar a visualização conforme suas necessidades e facilitando o acesso rápido às informações relevantes. <br />
Os critérios de filtragem variam de acordo com cada tela, incluindo opções como setor, status do colaborador, tipo de contrato, nível de permissão, período, entre outros. Além disso, campos de busca foram adicionados nas tabelas para agilizar a localização de dados específicos.

<br />

<span id="metricas">

# 📈 Métricas do Time
A sprint foi composta por 29 user stories e 43 subtasks.O gráfico de burndown mostra a evolução do trabalho ao longo da sprint. A linha horizontal representa o tempo, ou seja, as datas da sprint, enquanto a linha vertical indica os pontos de história que representam o esforço total planejado para a sprint. A linha cinza mostra a taxa de progresso ideal, indicando como o trabalho deveria ser realizado de maneira constante ao longo dos dias. Já a linha vermelha indica o trabalho realizado, que no gráfico reflete a conclusão das User Stories 100% finalizadas. O pico no gráfico ocorre quando as User Stories são concluídas.

<br />
    
<div align="center">
<img src="" alt="Gráfico Burndown" />
</div>

<br>

<span id="backlog">

# 📃 Backlog da Sprint

| **RFN** | **Rank** | **Prioridade** | **User Story** | **Estimativa** | **Critérios de Aceitação** |
|---------|----------|----------------|----------------|----------------|----------------------------|
| 7 | 32 | médio | Como administrador e gestor, gostaria de visualizar um relatório com os pontos diários registrados pelos colaboradores, para que eu possa acompanhar a presença | 5 | - Administrador vê de todos e gestor só vê do seu setor<br>- Coluna de Status mostra quando os funcionários estão Presentes, Ausentes, Férias, Folga ou Licença médica<br>- Quando colaborador está de Folga, Férias ou Licença médica, mostrar retorno previsto abaixo da tag do status<br>- Quando não houver dado, mostrar “-”<br>- Barra de pesquisa que puxa nomes dos colaboradores<br>- Filtros de colunas<br>- Paginação<br>- Tela responsiva |
| 7 | 33 | médio | Como administrador e gestor, gostaria de visualizar um gráfico com o relatório de ausências, para acompanhar e monitorar a frequência do time | 5 | - Administrador vê de todos e gestor só do seu setor<br>- Mostrar quantidade e porcentagem das ausências:<br>&nbsp;&nbsp;- Folgas<br>&nbsp;&nbsp;- Férias<br>&nbsp;&nbsp;- Licenças médicas<br>&nbsp;&nbsp;- Ausências sem justificativas<br>&nbsp;&nbsp;- Ausências justificadas<br>- Filtro de data define período, padrão últimos 90 dias<br>- Mostrar svg quando não tiver dados<br>- Tela responsiva |
| 7 | 34 | médio | Como administrador e gestor, gostaria de visualizar uma tabela com o relatório de ausências, para acompanhar e monitorar a frequência do time | 5 | - Administrador vê de todos e gestor só do seu setor<br>- Por padrão mostrar total de ausências por colaborador<br>- Ao clicar em seção do gráfico (ex: Folga), tabela atualiza dinamicamente filtrando a categoria<br>- Coluna “Ausências Totais” renomeada conforme categoria selecionada (ex: "Folgas Totais")<br>- Filtro de data define período<br>- Paginação<br>- Tela responsiva |
| 7 | 35 | médio | Como administrador e gestor, gostaria de visualizar uma tabela com os atrasos dos colaboradores, para que eu possa identificar e analisar falhas de marcações | 5 | - Administrador vê de todos e gestor só do seu setor<br>- Filtro de data define período<br>- Jornada flexível: horário esperado é o último horário do dia considerando carga horária e limite até 21h59 (considerar intervalo)<br>- Tolerância de 10 minutos de atraso<br>- Quando não houver dados, tabela some e fica só gráfico 100% ou svg sem dados<br>- Filtro de colunas<br>- Paginação<br>- Tela responsiva |
| 7 | 36 | médio | Como administrador e gestor, gostaria de visualizar um gráfico com os atrasos dos colaboradores, para que eu possa analisar falhas de marcações | 3 | - Administrador vê de todos e gestor só do seu setor<br>- Mostrar comparação entre atrasos e marcações pontuais<br>- Filtro de data define período<br>- Mostrar quantidade e porcentagem<br>- Mostrar svg quando não tiver dados<br>- Tela responsiva |
| 7 | 37 | médio | Como administrador e gestor, gostaria de visualizar um gráfico com a contagem de solicitação de ajuste, para que eu possa identificar e analisar falhas de marcações | 3 | - Administrador vê de todos e gestor só do seu setor<br>- Mostrar comparação entre solicitações de ajuste de ponto e marcações corretas<br>- Filtro de data define período<br>- Mostrar quantidade e porcentagem<br>- Mostrar svg quando não tiver dados<br>- Tela responsiva |
| 8 | 38 | alto | Como administrador, funcionário e gestor, gostaria de gerar os espelhos de ponto mensais, para controlar e ter registros das horas trabalhadas | 5 | - Listar no formato “MÊS/ANO”<br>- Espelho do mês atual indisponível até encerramento do mês<br>- Indicar espelho assinado, pendente ou indisponível<br>- Seguir modelo para gerar PDF<br>- Visualizar PDF gerado e assinado<br>- Zoom para visualização<br>- Opção de baixar arquivo<br>- Tela responsiva |
| 8 | 39 | alto | Como funcionário e gestor, gostaria de assinar os espelhos de ponto mensais, para controlar e ter registros das horas trabalhadas | 5 | - Ao selecionar espelho, abrir modal para visualizar com opções de assinar e baixar<br>- Mostrar PDF do mês correspondente<br>- Zoom para visualização<br>- Modal de assinatura pede verificação de CPF e senha<br>- Mostrar confirmação de assinatura<br>- Após assinado, botão “Assinar” não aparece |
| 9 | 40 | baixo | Como administrador, gostaria de definir os feriados que minha empresa irá participar, para controlar os dias de folga obrigatórios e facultativos | 5 | - Acesso restrito a administradores<br>- Indicar feriado no calendário com flag vermelha<br>- Modal “Definir feriados” com lista para seleção<br>- Buscar feriados estaduais e municipais via CEP da empresa<br>- Indicar feriados facultativos<br>- Tela responsiva |
| 9 | 41 | baixo | Como administrador e gestor, gostaria de definir os novos dias de folga, para controlar os dias trabalhados | 3 | - No calendário, mostrar tooltip “Definir dia de folga” nos dias trabalhados<br>- Ao clicar, abrir seleção do dia para folga com justificativa<br>- Tela responsiva |
| 9 | 42 | baixo | Como administrador, gostaria de definir folgas gerais na empresa para controlar os dias trabalhados | 5 | - Acesso restrito a administradores (restante só visualização)<br>- Indicar folga geral no calendário com flag roxa<br>- Tooltip “Definir dia de folga” a partir do dia atual<br>- Modal para definir dia com lista e filtro por setor e busca por nome<br>- Mostrar quantos colaboradores selecionados<br>- Tela responsiva |
| 9 | 43 | baixo | Como administrador e gestor, gostaria de ver um resumo das ausências no calendário da empresa, para controlar a quantidade de faltas | 5 | - Administrador vê todos, gestor só seu setor<br>- Em dias passados, mostrar resumo de férias, folgas, ausências (incluindo licenças e faltas) e feriados<br>- Resumo mensal com soma de feriados, ausências, férias e folgas<br>- Legenda do calendário<br>- Ao selecionar dia passado, abrir resumo com pessoas em férias, folga e ausentes<br>- Tela responsiva |
| 9 | 44 | baixo | Como funcionário e gestor, gostaria de visualizar um calendário com a minha jornada de trabalho, para que eu possa controlar os dias trabalhados | 3 | - Mostrar dias de folga, férias, ausências (faltas e licenças médicas) e feriados<br>- Mostrar resumo do mês com quantidade de feriados, faltas e folgas<br>- Tela responsiva |
| 9 | 45 | baixo | Como funcionário e gestor, gostaria de ter um resumo dos feriados, para planejar minhas demandas | 3 | - Mostrar feriados definidos pela empresa<br>- Atualizar conforme edição<br>- Mostrar sempre próximos 6 feriados<br>- Tela responsiva |
| 10 | 46 | baixo | Como funcionário e gestor, gostaria de receber uma notificação sobre justificativas de ausência pendentes, para que eu seja lembrado de enviá-las | 5 | - Notificação enviada ao registrar falta<br>- Enviar 24h e 30 min antes do limite de 48h para envio<br>- Mensagem com prazo para envio e link para Tela Meus Pontos<br>- Filtros de “Solicitações” e “Minhas pendências” para funcionários<br>- Filtros “Solicitações” e “Minhas análises” para gestores<br>- Filtros “Solicitações” e “Justificativas” para admins |
| 10 | 47 | baixo | Como funcionário e gestor, gostaria de receber uma notificação quando uma solicitação for aprovada ou reprovada, para manter o controle de pedidos | 2 | - Notificação enviada ao aprovar ou reprovar<br>- Mensagens indicando aprovador e tipo da solicitação<br>- Link para modal da solicitação |
| 10 | 48 | baixo | Como funcionário e gestor, gostaria de receber uma notificação quando esquecer de bater meu ponto, para que eu seja lembrado de marcar | 2 | - Notificação enviada assim que atraso (limite 10 min)<br>- Mensagem de aviso e link para Tela Meus Pontos |
| 10 | 49 | baixo | Como funcionário e gestor, gostaria de receber uma notificação sempre que uma folga for definida, para que eu saiba quando minha escala for alterada | 2 | - Notificação enviada quando dia de folga/trabalho for definido<br>- Mensagem indicando quem definiu e data<br>- Link para tela Calendário |
| 10 | 50 | baixo | Como administrador e gestor, gostaria de receber uma notificação quando uma solicitação estiver pendente, para que eu seja lembrado de verificar | 2 | - Notificação enviada na criação da solicitação<br>- Alertas aos 2, 7 e 14 dias de pendência<br>- Mensagens com detalhes e link para solicitação |
| 10 | 51 | baixo | Como administrador e gestor, gostaria de receber uma notificação quando um funcionário enviar uma justificativa de falta, para que eu possa acompanhar e tomar as ações necessárias | 2 | - Notificação enviada na submissão da justificativa<br>- Mensagem com detalhes e link para solicitação |
| 7 | 52 | médio | Como funcionário e gestor, gostaria de ver um resumo diário dos pontos batidos, para que eu possa monitorar minha jornada de trabalho de modo rápido | 3 | - Mostrar os dois últimos dias<br>- Mostrar até quatro pontos batidos com ícones diferenciados<br>- Mostrar somente os pontos disponíveis se não tiver os 4<br>- Tela responsiva |
| 11 | 53 | médio | Como administrador e gestor, gostaria que a tela de pontos diários tenha filtro na tabela, para que eu possa facilitar a visualização e análise das informações | 3 | - Filtro de Status: Presente, Ausente, Férias, Folga e Licença médica<br>- Filtro de Tipo Contratação: CLT e Estagiário<br>- Filtro de Setor (somente administrador)<br>- Filtro de Permissão: Administrador, Gestor, Funcionário (somente administrador)<br>- Campo de busca por nome ou código de registro |
| 11 | 54 | médio | Como administrador, gestor e funcionário, gostaria que a tela de banco de horas tenha filtro na tabela, para que eu possa facilitar a visualização e análise das informações | 3 | - Filtro de Tipo Contratação: CLT e Estagiário<br>- Filtro de Setor (somente administrador)<br>- Filtro de Permissão (somente administrador)<br>- Filtro de Status: Ativo/Inativo (padrão Ativo)<br>- Filtro de período de tempo (De até)<br>- Campo de busca por nome ou código |
| 11 | 55 | médio | Como administrador e gestor, gostaria que a tela de relatório de ausências tenha filtro na tabela e gráfico, para que eu possa facilitar a visualização e análise das informações | 2 | - Filtro de Tipo Contratação: CLT e Estagiário<br>- Filtro de Setor (somente administrador)<br>- Filtro de Permissão (somente administrador)<br>- Filtro de Status: Ativo/Inativo (padrão Ativo) |
| 11 | 56 | médio | Como administrador e gestor, gostaria que a tela de relatório de falha em marcações tenha filtro na tabela e gráfico, para que eu possa facilitar a visualização e análise das informações | 2 | - Filtro de Tipo Contratação: CLT e Estagiário<br>- Filtro de Setor (somente administrador)<br>- Filtro de Permissão (somente administrador)<br>- Filtro de Status: Ativo/Inativo (padrão Ativo) |
| 11 | 57 | médio | Como administrador e gestor, gostaria que a tela de colaboradores tenha filtro na tabela, para que eu possa facilitar a visualização e análise das informações | 2 | - Filtro de Tipo Contratação: CLT e Estagiário<br>- Filtro de Setor (somente administrador)<br>- Filtro de Permissão (somente administrador)<br>- Filtro de Status: Ativo/Inativo (padrão Ativo)<br>- Campo de busca por nome ou código<br>- Tela Histórico de Pontos com filtro de período |
| 11 | 58 | médio | Como administrador, gestor e funcionário, gostaria que a tela de solicitações tenha filtro na listagem, para que eu possa facilitar a visualização e análise das informações | 2 | - Filtros para administrador/gestor: Tipo Contratação, Setor, Permissão<br>- Filtros para todos: Tipo de Solicitação, Status (Aprovado/Reprovado) |
| 11 | 59 | médio | Como administrador e gestor, gostaria que a tela de calendário tenha filtro, para que eu possa facilitar a visualização e análise das informações | 2 | - Filtros: Tipo Contratação, Setor, Permissão<br>- Filtro de Tipo de Ausência (Folga, Férias, Ausência, Feriado)<br>- Modal Definir dia de folga: filtro de setor e busca por nome |
| 11 | 60 | médio | Como funcionário e gestor, gostaria que a tela de meus pontos tenha filtro na tabela, para que eu possa facilitar a visualização e análise das informações | 1 | - Filtro de período de tempo (De até) |




<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 3ª sprint:
  - [Repositório front-end](https://github.com/SkyFlyTeam/BeeOnTime-frontend/releases/tag/v3.0)
  - [Repositório back-end](https://github.com/SkyFlyTeam/BeeOnTime-backend/releases/tag/v3.0)
<br>


