![1° Sprint](https://github.com/user-attachments/assets/046b1b08-9234-4650-8107-80ab3cec102c)

<br>

<p align="center">
    <a href="#objetivos"> Objetivos da Sprint </a> &nbsp |&nbsp &nbsp
    <a href="#entregas"> Entregas </a> &nbsp |&nbsp &nbsp
    <a href="#metricas"> Métricas do Time </a>  &nbsp |&nbsp &nbsp  
    <a href="#backlog"> Backlog da Sprint </a>  &nbsp |&nbsp &nbsp  
    <a href="#links"> Links úteis </a>
</p>

No início do desenvolvimento da aplicação de controle de ponto eletrônico, a primeira sprint focou no MVP (Produto Mínimo Viável), priorizando as funcionalidades mais essenciais. A equipe concentrou seus esforços na marcação de ponto, que é a base do sistema. Entre as funcionalidades desenvolvidas, destacam-se o cadastro da empresa e setores, cadastro de colaboradores e jornadas, registro de ponto, histórico de pontos, solicitações de ajustes de ponto e cálculo automático de horas extras.

<span id="objetivos">

# 🎯 Objetivos da Sprint
Os requisitos funcionais atendidos nesta sprint foram:

- ✔️ **RFN 01. Cadastro de Empresas:** <br /> O sistema permite cadastrar uma empresa juntamente com os setores que a compõem. <br /> <br /> 
- ✔️ **RFN 02. Cadastro de Colaboradores:** <br />  O sistema permite cadastrar funcionários com diferentes níveis de permissão, vinculando-os à sua jornada de trabalho no momento do cadastro. <br /> <br /> 
- ✔️ **RFN 03. egistro e Ajustes no Ponto:** <br />  O sistema permite registrar os horários de entrada, saída e intervalos dos funcionários, mantendo um histórico acessível ao colaborador. O sistema também permite realizar solicitações de ajustes de ponto. <br /> <br /> 
- ✔️ **RFN 04. Horas Extras e Banco de Horas:** <br />  O sistema tem o registro automático das horas extras realizadas pelo colaborador. <br /> <br /> 

<br> 

<span id="entregas">

# 📲 Entregas
Durante esta sprint, o time entregou artefatos SCRUM validados, como o Backlog do Produto, o Backlog das Sprints e as User Stories, com a participação direta do P.O. e comunicação constante com o cliente. Para entender e alinhar as expectativas do cliente, foi criado um protótipo inicial no Figma, que ajudou a definir a identidade visual e o design do sistema. Esse protótipo foi validado com o cliente e traduzido em uma aplicação React, integrando as funcionalidades acordadas para esta sprint.

### RF 01: Cadastro da Empresa
O cadastro da empresa ocorre no ínicio, com o preenchimento de informações essenciais como nome, razão social, CNPJ e CEP, o que permite preencher automaticamente o endereço da empresa. No segundo passo, é possível cadastrar todos os setores da empresa, estruturando a organização hierárquica.

### RF 02: Cadastro de Colaboradores
O sistema permite o cadastro de novos colaboradores, onde cada um recebe um e-mail de primeiro acesso após a conclusão do cadastro. As informações incluem nome, CPF, e-mail, data de nascimento, código de registro, tipo de contrato (CLT ou Estágio), data de contratação, cargo, nível de acesso e o setor ao qual o colaborador pertence.

No segundo passo, a jornada de trabalho do colaborador pode ser configurada, especificando carga horária e dias trabalhados. Caso a jornada seja flexível, não é necessário definir os horários de entrada, saída e almoço, mas, caso contrário, essas informações devem ser detalhadas.

### RF 03: Registro e Ajustes no Ponto
Funcionários e gestores podem registrar os pontos de trabalho ao longo do dia, incluindo horários de entrada, início de almoço, fim de almoço e saída. Caso ocorra algum erro ou esquecimento ao bater o ponto, é possível solicitar um ajuste, acompanhado de uma justificativa. Gestores ou administradores têm a capacidade de aprovar ou rejeitar essas solicitações de ajuste. Se o ajuste for aceito, o ponto é alterado automaticamente. Caso contrário, o gestor pode enviar uma devolutiva explicando a recusa.

### RF 04: Horas Extras e Banco de Horas
As horas extras são automaticamente calculadas pelo sistema. Na tela de "Meus Pontos", o colaborador pode visualizar a quantidade de horas trabalhadas, incluindo horas extras. O sistema também registra todos os pontos batidos, garantindo transparência e controle sobre o tempo trabalhado, além de facilitar a gestão de horas extras e banco de horas.

<br />

<span id="metricas">

# 📈 Métricas do Time
A sprint foi composta por 9 user stories e 27 subtasks. Embora o gráfico de burndown mostre que o trabalho foi concentrado no final, a realidade é que o time começou a trabalhar antes da sprint, realizando atividades como a criação do mockup, definição de DoR e DoD, elaboração do Backlog da Sprint, e configuração das branches de backend e frontend.

O gráfico de burndown mostra a evolução do trabalho ao longo da sprint. A linha horizontal representa o tempo, ou seja, as datas da sprint, enquanto a linha vertical indica os pontos de história que representam o esforço total planejado para a sprint. A linha cinza mostra a taxa de progresso ideal, indicando como o trabalho deveria ser realizado de maneira constante ao longo dos dias. Já a linha vermelha indica o trabalho realizado, que no gráfico reflete a conclusão das User Stories 100% finalizadas. O pico no gráfico ocorre quando as User Stories são concluídas, explicando a aparente concentração de trabalho no final da sprint. Na prática, a maior parte das subtasks já estava concluída antes das últimas entregas.

<br />
    
<div align="center">
<img src="https://github.com/user-attachments/assets/d1f6e4c8-addd-42d2-b012-2d50f9801472" alt="Gráfico Burndown" />
</div>

<br>

<span id="backlog">

# 📃 Backlog da Sprint

| **RFN** | **Rank** | **Prioridade** | **User Story** | **Estimativa** | **Sprint** | **Critérios de Aceitação** |
|---------|----------|----------------|----------------|----------------|------------|---------------------------|
| 01      | 1        | Alta           | Como administrador, quero cadastrar minha empresa, para configurar minhas informações e começar a gerenciar os pontos e colaboradores | 3              | 1          | - Na tela de Login, ao clicar no botão "É novo aqui? Cadastre sua empresa!", o usuário será direcionado para a tela de cadastro da empresa. <br> - A tela de cadastro deve conter os campos obrigatórios: Nome, Razão Social, CNPJ e CEP. <br> - Os campos CNPJ e CEP devem possuir máscaras de formatação. <br> - Não deve permitir o registro duas empresas com o mesmo CNPJ <br> - Após preencher os campos e salvar o cadastro, o usuário será redirecionado para a tela de definição de setores da empresa |
| 02      | 2        | Alta           | Como administrador, quero cadastrar e gerenciar os setores da minha empresa para organizar as equipes de trabalho | 3              | 1          | - Após preencher as informações da empresa, o usuário será redirecionado para a tela de cadastro de setores <br> - Ao digitar o nome no campo e clicar no botão "+", um novo setor poderá ser adicionado <br> - Todos os setores cadastrados serão listados abaixo do formulário de inserção <br> - O sistema não permitirá o cadastro de setores com nomes duplicados. <br> - O sistema não permitirá a adição de setores com nome vazio |
| 02      | 3        | Alta           | Como administrador, quero que meus cadastros tenham diferentes níveis de acesso, para garantir que cada usuário tenha permissões específicas conforme sua função | 21             | 1          | - O sistema deve permitir os níveis de acesso de administrador, gestor e funcionário <br> - O sistema deve bloquear usuários sem permissão de executar ações não autorizadas <br> - Apenas administradores podem alterar o nível de acesso do colaborador |
| 02      | 4        | Alta           | Como administrador, quero registrar meus colaboradores com seus dados, para fazer o gerenciamento de suas informações e atividades dentro do sistema | 21             | 1          | - Apenas administradores podem registrar novos colaboradores <br> - O cadastro terá os campos de nome completo, data de nascimento, CPF, e-mail, número de registro, setor, data de admissão <br> - Os campos de data de nascimento, CPF, e-mail e data de admissão deverão ter máscaras de formatação <br> - O sistema não deve permitir duas contas com o mesmo CPF ou e-mail |
| 02      | 5        | Média          | Como administrador, quero definir a jornada de trabalho, para que possa garantir o cumprimento das obrigações horários dos colaboradores | 5              | 1          | - Apenas administradores podem definir ou editar a jornada de trabalho dos colaboradores <br> - A definição da jornada trará os campos de horários de Entrada, Saída, Carga Horária e Dia da Semana <br> - Os horários de Entrada e Saída só serão mostrados se a opção for “Não” no campo de Horário Flexível? <br> - Todos os campos de horário deverão ter máscaras de formatação <br> - O Horário de Saída deve sempre ser maior que o Horário de Entrada, evitando registros inválidos |
| 03      | 6        | Alta           | Como funcionário e gestor, quero registrar meus horários de entrada, saída e tempo de almoço, para que minha jornada de trabalho seja contabilizada corretamente | 8              | 1          | - Todos os níveis de acesso, exceto o administrador da empresa, registram ponto <br> - Na tela de início, serão exibidos apenas dois botões por vez, alternando conforme o status: Entrada ➙ Saída, Ida Almoço ➙ Volta Almoço <br> - Cada status pode ser acionado apenas uma vez por dia, ficando bloqueado após o uso. <br> - Na mesma tela, serão exibidos os parâmetros de horas trabalhadas diárias e mensais, incluindo informações sobre horas extras |
| 04      | 7        | Alta           | Como funcionário e gestor, quero que minhas horas extras sejam automaticamente contabilizadas, para garantir o controle das horas trabalhadas a mais | 8              | 1          | - O sistema deverá automaticamente contabilizar as horas extras quando o tempo trabalhado passar da carga horária definida para aquele usuário <br> - Deverá ser indicado as horas diárias automáticas na tela inicial em “Carga diária” <br> - Deverá acumular as horas extras no card da tela inicial que indica o Banco de Horas do usuário |
| 03      | 8        | Média          | Como funcionário e gestor, quero acessar meu histórico de pontos, para poder acompanhar e ter controle detalhado das horas trabalhadas | 3              | 1          | - Na tela de Meus pontos, será exibido todo o histórico de pontos marcado por aquele funcionário, dividido por dias e mostrando horas extras, faltantes e adicional noturno <br> - Terá o filtro de período a fim de visualizar datas específicas |
| 03      | 9        | Média          | Como funcionário e gestor, quero realizar pedidos de ajustes de pontos, para que seja ajustado alterações que eu julgo necessárias | 8              | 1          | - Na tela Meus Pontos, haverá a opção Solicitar Ajuste, ao lado do horário correspondente, que abrirá uma tela de edição dos registros. Nela, será possível excluir, adicionar um novo ponto e inserir uma justificativa, que será enviada para aprovação do gestor do setor ou do administrador <br> - Na tela Solicitações, ao criar um novo pedido com o tipo “Ajuste de ponto”, será possível selecionar uma data e um horário já registrado, permitindo definir a alteração desejada. Além do campo obrigatório de justificativa |
| 03      | 10       | Média          | Como administrador e gestor, quero receber e aprovar pedidos de alteração de ponto, para serem modificados caso necessário | 3              | 1          | - Apenas administradores e gestores recebem pedidos de alteração de ponto <br> - Administradores recebem solicitações de todos, enquanto gestores recebem apenas de seus setores <br> - Na tela de solicitações, aparecerá todas as solicitações enviadas com a indicação “Ajuste de ponto” <br> - Ao escolher o pedido, as opções Aceitar e Recusar estarão disponíveis. O campo de justificativa estará sempre visível, sendo opcional |


<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 1ª sprint:
  - [Repositório front-end](https://github.com/SkyFlyTeam/BeeOnTime-frontend/releases/tag/v1.0)
  - [Repositório back-end](https://github.com/SkyFlyTeam/BeeOnTime-backend/releases/tag/v1.0)
<br>


