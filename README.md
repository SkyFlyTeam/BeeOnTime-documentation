![2° Sprint](https://github.com/user-attachments/assets/358d1391-4dcc-4a46-8219-8a2a84d925ae)

<br>

<p align="center">
    <a href="#objetivos"> Objetivos da Sprint </a> &nbsp |&nbsp &nbsp
    <a href="#entregas"> Entregas </a> &nbsp |&nbsp &nbsp
    <a href="#metricas"> Métricas do Time </a>  &nbsp |&nbsp &nbsp  
    <a href="#backlog"> Backlog da Sprint </a>  &nbsp |&nbsp &nbsp  
    <a href="#links"> Links úteis </a>
</p>

Nesta sprint, nosso foco principal foi o desenvolvimento de lógicas de backend e funcionalidades de frontend, voltadas para as solicitações de funcionários e gestores aos administradores. Agora, além de solicitar ajustes de ponto, os usuários também podem solicitar folgas, férias, horas extras, licença médica e justificar ausências. Implementamos ainda a visualização do banco de horas individual, permitindo o acompanhamento do histórico de compensações. Por fim, desenvolvemos as telas de edição de dados de perfil e dos funcionários.

<span id="objetivos">

# 🎯 Objetivos da Sprint
Os requisitos funcionais atendidos nesta sprint foram:

- ✔️ **RFN02. Cadastro de Colaboradores** <br /> O sistema permite cadastrar funcionários com diferentes níveis de permissão, vinculando-os à sua jornada de trabalho no momento do cadastro. <br /> <br /> 
- ✔️ **RFN04. Horas Extras e Banco de Horas:** <br />  O sistema permite a solicitação antecipada de horas extras ou o registro automático, sujeitos à aprovação do administrador, que define se serão pagas ou convertidas para o banco de horas.
 <br /> <br /> 
- ✔️ **RFN05. Justificativas de Ausências:** <br />  O sistema permite que funcionários registrem ausências, anexando justificativas e informando os dias de afastamento. O RH recebe e confirma o recebimento da solicitação.
 <br /> <br /> 

<br> 

<span id="entregas">

# 📲 Entregas

### RFN02. Cadastro de Colaboradores
O módulo de cadastro de colaboradores foi finalizado nesta sprint.
Agora, além do cadastro inicial da empresa, as telas de edição de perfil, edição de dados dos colaboradores e configuração da jornada de trabalho estão totalmente desenvolvidas, concluindo assim o requisito de cadastros.

### RFN04. Horas Extras e Banco de Horas:
O controle de horas foi ampliado e aprimorado.
Além da contabilização automática das horas extras, o sistema agora permite a solicitação prévia de realização de horas extras em dias planejados, com envio de justificativa.
A tela de Banco de Horas também foi finalizada, apresentando as seguintes informações:
- Total de horas trabalhadas
- Horas descontadas
- Horas abonadas
- Horas extras pagas
- Saldo acumulado

### RFN05. Justificativas de Ausências:
O sistema de justificativas foi implementado conforme a regra de negócio.
Agora, é possível:
- Enviar justificativas de ausência dentro do prazo de 48 horas após a falta.
- Solicitar afastamento para períodos futuros, como em casos de afastamento médico, com o envio da justificativa.

<br />

<span id="metricas">

# 📈 Métricas do Time
A sprint foi composta por 22 user stories e 37 subtasks. O gráfico de burndown mostra a evolução do trabalho ao longo da sprint. A linha horizontal representa o tempo, ou seja, as datas da sprint, enquanto a linha vertical indica os pontos de história que representam o esforço total planejado para a sprint. A linha cinza mostra a taxa de progresso ideal, indicando como o trabalho deveria ser realizado de maneira constante ao longo dos dias. Já a linha vermelha indica o trabalho realizado, que no gráfico reflete a conclusão das User Stories 100% finalizadas. O pico no gráfico ocorre quando as User Stories são concluídas.

<br />

<div align="center">
<img src="https://github.com/user-attachments/assets/9f422ddd-e622-474c-9295-66ae4ad78cdd" alt="Gráfico Burndown" />
</div>

<br>

<span id="backlog">

# 📃 Backlog da Sprint
| **RFN** | **Rank** | **Prioridade**      | **User Story**                                                                                                  | **Estimativa** | **Critérios de Aceitação**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|---------|----------|--------------------|----------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 4       | 11       | Média              | Como gestor, gostaria que na minha tela de solicitações fosse dividida entre as análises dos funcionários a fazer e meus pedidos, para facilitar a visualização e o gerenciamento das tarefas | 2              | - A listagem será dividida entre "Análises" e "Meus Pontos".<br>- Análises: exibe solicitações dos funcionários do setor.<br>- Meus Pontos: exibe solicitações feitas pelo gestor.<br>- Ordenação: mais recente para mais antigo em novas e analisadas.<br>- Tela responsiva.                                                                                                                                                                                                                                   |
| 4       | 12       | Média              | Como funcionário e gestor gostaria de solicitar horas extras para que seja liberado trabalhar a mais quando necessário | 3              | - Justificativa é campo obrigatório.<br>- Horas extras obrigatórias e em horas.<br>- Pode ser selecionado somente um dia.<br>- Solicitação deve ser feita com no mínimo 2 horas de antecedência, bloqueando antes disso.<br>- Exibir toast de confirmação de solicitação enviada.                                                                                                                                                                                                                                               |
| 4       | 13       | Média              | Como funcionário e gestor, gostaria de poder escolher entre as diferentes opções ao fazer a solicitação, para garantir que minha solicitação seja feita corretamente | 3              | - Botão criado como componente.<br>- Opções: Férias, Folga, Hora extra, Ajuste de ponto e Licença médica.<br>- Tela responsiva.                                                                                                                                                                                                                                                                                                                                                                                                        |
| 2       | 14       | Média              | Como administrador, gestor ou funcionário, quero poder editar minhas informações de cadastro para manter meus dados atualizados | 2              | - Todos os níveis podem editar seu próprio perfil.<br>- Nome: somente letras.<br>- E-mail: válido e único.<br>- Nível de acesso, Cargo, Departamento e Tipo de contrato inalteráveis.<br>- Senha altera ao salvar.<br>- Botão salvar aparece somente após edição.<br>- Após alteração exibir mensagem de confirmação.<br>- Tela responsiva.                                                                                                                                                                             |
| 4       | 15       | Média              | Como administrador e gestor, gostaria de ver um relatório mensal com todos os meus funcionários e seu banco de horas, para acompanhar as horas trabalhadas a mais | 3              | - Tela mostra banco de horas do mês atual.<br>- Administrador vê todos funcionários, gestor somente setor.<br>- Colunas: Total Horas Trabalhadas, Horas Contratuais, Descontos, Horas Abonadas, Horas Extras Pagas, Saldo Acumulado.<br>- Skeleton na página enquanto tabela não carrega.                                                                                                                                                                                                                                        |
| 4       | 16       | Média              | Como administrador e gestor gostaria de ter um modal para classificar horas extras solicitadas por um colaborador como pagas, para gerenciar e controlar essas horas de maneira eficiente | 5              | - Administrador aceita de todos usuários, gestor só seu setor.<br>- Abrange solicitações e horas extras contadas.<br>- Usa componentes modal e botões.<br>- Exibe colaborador, dia solicitado e total de horas.<br>- Origem: solicitação gestor/funcionário.<br>- Ao recusar não tem devolutiva.<br>- Utiliza ms-BancoHoras.<br>- Exibe toast de confirmação de solicitação recusada, classificada como banco de horas ou pagas.                                                                                                                           |
| 2       | 17       | Média              | Como administrador, quero editar as informações e a jornada dos usuários para mantê-las atualizadas           | 2              | - Apenas administrador pode editar usuário e jornada.<br>- Nome: somente letras.<br>- CPF com máscara e sem duplicidade.<br>- E-mail válido e único.<br>- Data nascimento: ano com até 4 dígitos.<br>- Número registro: só números e sem duplicidade.<br>- Tipo de contrato: Admin/Gestor CLT, Funcionário CLT ou Estagiário.<br>- Campos obrigatórios obrigam validação.<br>- Toggle status.<br>- Botão salvar aparece só após alteração.<br>- Exibe toast confirmação.<br>- Tela responsiva.<br>- Skeleton.<br>- Regras para horário flexível e obrigatoriedade dos campos.<br>- Validações e toasts similares para jornada. |
| 4       | 18       | Média              | Como funcionário e gestor, gostaria de ver um relatório mensal do meu banco de horas, para acompanhar as horas trabalhadas a mais | 5              | - Tela mostra datas do mês atual.<br>- Mesmas colunas e estrutura do relatório mensal geral.<br>- Skeleton enquanto tabela carrega.                                                                                                                                                                                                                                                                                                                                                             |
| 4       | 19       | Média              | Como funcionário e gestor, gostaria de ter um resumo do meu banco de horas na tela inicial, para visualizar rapidamente as horas trabalhadas a mais | 2              | - Primeira barra: relação horas trabalhadas vs carga horária total.<br>- Segunda barra: distribuição horas extras pagas/banco horas (se houver).<br>- Skeleton do componente enquanto não carregado.                                                                                                                                                                                                                                                                                          |
| 5       | 20       | Alta               | Como administrador e gestor, gostaria de receber justificativas de faltas dos colaboradores, para ter controle sobre as ausências | 3              | - Administrador recebe de todos, gestor só do setor.<br>- Devolutiva obrigatória em recusa.<br>- Toast de confirmação aprovada/recusada.                                                                                                                                                                                                                                                                                                                                                         |
| 4       | 21       | Alta               | Como administrador, gestor e funcionário, quero visualizar um relatório diário de banco de horas, para que eu possa acompanhar as horas extras trabalhadas | 3              | - Tela mostra banco de horas do mês atual.<br>- Acesso via relatório mensal e ação.<br>- Listagem ordenada do dia mais atual ao mais antigo.<br>- Mesmas colunas do relatório mensal.<br>- Skeleton na página.                                                                                                                                                                                                                                                                               |
| 5       | 22       | Alta               | Como administrador e gestor, gostaria que as faltas, folgas e férias fossem registradas nos dias correspondentes no histórico de pontos dos usuários, para facilitar a visualização e o acompanhamento das ausências | 3              | - Indicadores para ausências, ausências justificadas, folgas e férias.<br>- Skeleton enquanto tabela carrega.                                                                                                                                                                                                                                                                                                                                                                             |
| 5       | 23       | Alta               | Como funcionário e gestor, gostaria de enviar uma justificativa para afastamento médico, para que minha ausência seja devidamente validada | 5              | - Selecionar pelo menos um dia.<br>- Justificativa obrigatória.<br>- Prazo para envio: 48h após ausência, bloqueio depois.<br>- Toast confirmação envio.                                                                                                                                                                                                                                                                                                                                     |
| 5       | 24       | Alta               | Como funcionário e gestor, quero justificar minha falta para registrar corretamente o motivo da minha ausência   | 5              | - Opção para justificar ausência em dias sem ponto.<br>- Modal com dia e justificativa obrigatória.<br>- Erro se campo vazio.<br>- Falta não registrada em folgas.<br>- Toast confirmação envio.                                                                                                                                                                                                                                                                                             |
| 6       | 25       | Média              | Como funcionário e gestor, quero solicitar folgas para usufruir das minhas horas acumuladas no banco de horas   | 5              | - Exibir horas acumuladas no banco.<br>- Seleção de pelo menos um dia, que deve ser dia de trabalho.<br>- Mostrar horas totais consumidas.<br>- Justificativa obrigatória.<br>- Permitir solicitação mesmo sem banco horas (fica pendente se aprovada).<br>- Solicitação com 15 dias de antecedência, bloqueio antes disso.<br>- Toast confirmação envio.                                                                                                                                  |
| 6       | 26       | Média              | Como administrador e gestor, quero receber os pedidos de folga dos colaboradores para avaliá-los e aprová-los ou recusá-los conforme necessário | 3              | - Devolutiva obrigatória em caso de recusa.<br>- Toast confirmação aprovada/recusada.                                                                                                                                                                                                                                                                                                                                                                                                       |
| 6       | 27       | Média              | Como funcionário e gestor, quero solicitar férias para usufruir dos meus direitos de descanso anual garantidos por lei | 5              | - Férias permitidas em formatos: 30; 15+15; 20+10; 10+15+5.<br>- Seleção permitida conforme formato.<br>- Verificação de férias já tiradas ao abrir tela.<br>- Botão “Férias” desativado se sem tempo mínimo 1 ano ou pedido pendente.<br>- Solicitação com 60 dias de antecedência, bloqueio antes.<br>- Justificativa obrigatória.<br>- Toast confirmação criação.<br>- Sistema verifica aniversário de contratação para alerta de férias.<br>- Contagem de dias úteis feita no front.<br>- Registro no BD na tabela Folga com tipo “Férias”.                                    |
| 6       | 28       | Média              | Como administrador e gestor, quero receber os pedidos de férias dos colaboradores para avaliá-los e aprová-los ou recusá-los conforme planejamento | 3              | - Devolutiva obrigatória em caso de recusa.<br>- Toast confirmação aprovada/recusada.                                                                                                                                                                                                                                                                                                                                                                                                       |
| 4       | 29       | Média              | Como administrador e gestor gostaria de classificar horas extras solicitadas por um colaborador como banco de horas, para gerenciar e controlar essas horas de maneira eficiente | 5              | - Administrador aceita de todos, gestor só seu setor.<br>- Abrange solicitações e horas extras contadas.<br>- Usa componentes modal e botões.<br>- Exibe colaborador, dia e total de horas.<br>- Origem: solicitação gestor/funcionário.<br>- Ao recusar não tem devolutiva.<br>- Utiliza ms-BancoHoras.<br>- Toast confirmação solicitação recusada, banco de horas ou pagas.                                                                                                                                                 |
| 4       | 30       | Média              | Como administrador e gestor gostaria de recusar horas extras feitas ou solicitadas por um colaborador, para gerenciar essas horas de maneira eficiente | 1              | - Administrador aceita de todos, gestor só seu setor.<br>- Abrange solicitações e horas extras contadas.<br>- Usa componentes modal e botões.<br>- Exibe colaborador, dia e total de horas.<br>- Origem: solicitação gestor/funcionário.<br>- Ao recusar não tem devolutiva.<br>- Utiliza ms-BancoHoras.<br>- Toast confirmação solicitação recusada, banco de horas ou pagas.                                                                                                                                                 |
| 4       | 31       | Média              | Como administrador e gestor, gostaria de converter o banco de horas dos colaboradores em horas extras pagas para gerir o tempo de trabalho e compensações | 5              | - Após movimentação, exibe quantidade a mudar e confirma sim ou não.<br>- Exibe toast confirmação de alteração.                                                                                                                                                                                                                                                                                                                                                                            |


<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 2ª sprint:
  - [Repositório front-end](https://github.com/SkyFlyTeam/BeeOnTime-frontend/releases/tag/v2.0)
  - [Repositório back-end](https://github.com/SkyFlyTeam/BeeOnTime-backend/releases/tag/v2.0)
<br>


