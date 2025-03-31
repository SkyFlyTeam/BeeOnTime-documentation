![1° Sprint](https://github.com/user-attachments/assets/046b1b08-9234-4650-8107-80ab3cec102c)

<br>

<p align="center">
    <a href="#objetivos"> Objetivos da Sprint </a> &nbsp |&nbsp &nbsp
    <a href="#entregas"> Entregas </a> &nbsp |&nbsp &nbsp
    <a href="#metricas"> Métricas do Time </a>  &nbsp |&nbsp &nbsp  
    <a href="#links"> Links úteis </a>
</p>

No início do desenvolvimento da aplicação de controle de ponto eletrônico, a primeira sprint focou no MVP (Produto Mínimo Viável), priorizando as funcionalidades mais essenciais. A equipe concentrou seus esforços na marcação de ponto, que é a base do sistema. Entre as funcionalidades desenvolvidas, destacam-se o cadastro da empresa e setores, cadastro de colaboradores e jornadas, registro de ponto, histórico de pontos, solicitações de ajustes de ponto e cálculo automático de horas extras.

<span id="objetivos">

# 🎯 Objetivos da Sprint
Os requisitos funcionais atendidos nesta sprint foram:

- ✔️ RF 01: Cadastro da empresa
- ✔️ RF 02: Cadastro de colaboradores
- ✔️ RF 03: Registro e ajustes no ponto
- ✔️ RF 04: Cálculo de horas extras e banco de horas

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

<span id="links">

# 🔗 Links úteis

- Tags geradas em cada repositório que simbolizam o fim da 1ª sprint:
  - [Repositório front-end]()
  - [Repositório back-end]()
- [Modelo lógico do Banco de Dados](https://drive.google.com/file/d/1sXmtWTzleYs18p3dwqE7RUNxmmhGuBpb/view?usp=sharing)
- [Backlog da 1°Sprint]()
<br>


