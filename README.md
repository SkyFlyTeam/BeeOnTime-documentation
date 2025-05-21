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

| **RFN** | **Rank** | **Prioridade** | **User Story** | **Estimativa** | **Sprint** | **Critérios de Aceitação** |
|---------|----------|----------------|----------------|----------------|------------|---------------------------|


<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 3ª sprint:
  - [Repositório front-end](https://github.com/SkyFlyTeam/BeeOnTime-frontend/releases/tag/v3.0)
  - [Repositório back-end](https://github.com/SkyFlyTeam/BeeOnTime-backend/releases/tag/v3.0)
<br>


