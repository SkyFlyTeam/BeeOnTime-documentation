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
- ✔️ **RFN06. Controle de Férias e Folgas:** <br />  O sistema permite o agendamento de férias e folgas pelos administradores e também permite solicitações pelos funcionários. Após a aprovação, o sistema registra automaticamente a ausência no calendário da empresa. <br /> <br />

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

### RFN06. Controle de Férias e Folgas:
O sistema de solicitações de férias e folgas foi finalizado.
Entre as funcionalidades entregues:
- Solicitação de folgas utilizando o banco de horas ou com desconto de horas.
- Marcação de datas para folgas, com necessidade de aprovação do gestor/administrador.
- Solicitação de férias nos formatos permitidos (30 dias, 15 + 15 dias, 20 + 10 dias ou 10 + 15 + 5 dias), também com aprovação requerida.

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

| **RFN** | **Rank** | **Prioridade** | **User Story** | **Estimativa** | **Sprint** | **Critérios de Aceitação** |
|---------|----------|----------------|----------------|----------------|------------|---------------------------|
| 02      | 11        | Média           | Como administrador, quero editar as informações e a jornada dos usuários para mantê-las atualizadas | 2              | 2          | Editar **Colaborador:**<br>-Apenas administrador pode editar usuário e jornada.<br>-Nome: somente letras.<br>-CPF: deve ter máscara e não permitir duplicidade.<br>-E-mail: deve ser válido e único.<br>-Data de nascimento: ano com até 4 dígitos.<br>-Número de registro: somente números e não duplicado.<br>-Caso o nível de acesso seja Admin ou Gestor o Tipo de Contrato fica como CLT, caso seja funcionário, pode ser CLT ou Estagiário.<br>-Não permitir salvar com campos obrigatórios vazios. Exibir erro de campo obrigatório.<br>-Toggle no botão de status.<br>-Botão de salvar só aparece após alteração.<br>-Exibir um toast de confirmação de alteração.<br>-A tela precisa ser responsiva.<br>-Adicionar Skeleton<br><br>**Editar Jornada:**<br>-Se horário flexível for "Sim", campos de entrada e saída desaparecem; se "Não", ambos são obrigatórios.<br>-Horário de saída não pode ser antes do de entrada.<br>-Pelo menos um dia da semana deve ser selecionado.<br>-Não permitir salvar com campos obrigatórios vazios. Exibir erro de campo obrigatório.<br>-Botão de salvar só aparece após edição de campo.<br>-Exibir um toast de confirmação de alteração.<br>-A tela precisa ser responsiva.<br>-Adicionar Skeleton <br> |
| 02      | 12        | Média           | Como administrador, gestor ou funcionário, quero poder editar minhas informações de cadastro para manter meus dados atualizados | 2              | 2          | -Todos os níveis de acesso podem editar seu próprio perfil.<br>- Nome: somente letras.<br>- E-mail: válido e único.<br>- Nível de acesso, Cargo, Departamento e Tipo de contrato: inalteráveis<br>- Senha: altera ao salvar.<br>- Botão de salvar aparece somente após edição.<br>- Após a alteração exibir uma mensagem de confirmação<br>- A tela precisa ser responsiva.<br> |
| 04      | 13        | Baixa           | Como funcionário e gestor, gostaria de poder escolher entre as diferentes opções ao fazer a solicitação, para garantir que minha solicitação seja feita corretamente | 3             | 2          | - O botão deverá ser criado como componente<br>- Deverá ter as opções de Férias, Folga, Hora extra, Ajuste de ponto e Licença médica<br>- Precisa ser responsivo.<br> |
| 02      | 14        | Baixa           | Como gestor, gostaria que na minha tela de solicitações fosse dividida entre as análises dos funcionários a fazer e meus pedidos, para facilitar a visualização e o gerenciamento das tarefas | 2             | 2          | -A listagem será dividida entre "Análises" e "Meus Pontos":<br> -Análises: exibe as solicitações dos funcionários do setor.<br> - Meus Pontos: exibe as solicitações feitas pelo gestor.<br>- A ordem de listagem será:<br> -Mais recente para o mais antigo para novas solicitações.<br>- Mais recente para o mais antigo para solicitações já analisadas.<br>- A tela precisa ser responsiva.<br> |
|05|15| Alta |||||
||||||||
||||||||
||||||||
||||||||
||||||||


<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 2ª sprint:
  - [Repositório front-end](https://github.com/SkyFlyTeam/BeeOnTime-frontend/releases/tag/v2.0)
  - [Repositório back-end](https://github.com/SkyFlyTeam/BeeOnTime-backend/releases/tag/v2.0)
<br>


