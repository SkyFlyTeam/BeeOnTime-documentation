# Documentação Projeto BeeOnTime

### Orientadores:

- P2: Gerson da Penha 
- M2: Eduardo Sakaue

<br>

<span id="sobre">

# 🔎 Sobre o projeto

O BeeOnTime é um sistema de controle de ponto eletrônico para que as empresas possam gerenciar de forma mais eficaz suas equipes quanto a escalas/jornadas de trabalho, ausências programadas, horas extras, banco de horas, férias e etc.

<br> 

<span id="backlog">

# Backlog do Produto

### Requisitos Funcionais
RFN01. Cadastro de Empresas: O sistema permite cadastrar uma empresa, permitindo a seleção da localidade para que os feriados regionais sejam automaticamente configurados no calendário da empresa.

RFN02. Cadastro de Colaboradores: O sistema permite cadastrar funcionários com diferentes níveis de permissão, vinculando-os à sua jornada de trabalho no momento do cadastro.

RFN03. Registro e Ajustes no Ponto: O sistema permite registrar automaticamente os horários de entrada, saída e intervalos dos funcionários, mantendo um histórico acessível ao colaborador. O sistema também permite solicitações de ajustes de ponto, limitadas a três por funcionário, seguindo a política interna.

RFN04. Horas Extras e Banco de Horas: O sistema permite a solicitação antecipada de horas extras ou o registro automático, sujeitos à aprovação do administrador, que define se serão pagas ou convertidas para o banco de horas.

RFN05. Justificativas de Ausências: O sistema permite que funcionários registrem ausências, anexando justificativas e informando os dias de afastamento. O RH recebe e confirma o recebimento da solicitação.

RFN06. Controle de Férias e Folgas: O sistema permite o agendamento de férias e folgas pelos administradores e também permite solicitações pelos funcionários. Após a aprovação, o sistema registra automaticamente a ausência no calendário da empresa.

RFN07. Relatórios de Ponto: O sistema gera relatórios detalhados sobre registros de ponto, horas extras, banco de horas, ausências, atrasos e falhas em marcações, permitindo filtros por colaborador e período.

RFN08. Espelho de Ponto: O sistema gera o espelho de ponto detalhado de cada funcionário, permitindo a assinatura para validação formal e a disponibilização de uma cópia para conferência.

RFN09. Calendário da Empresa: O sistema permite definir os dias que serão folgas para todos os funcionários, permitindo a configuração de feriados facultativos conforme as regras da empresa.

RFN10. Notificações e Alertas: O sistema envia alertas aos funcionários e gestores sobre eventos importantes, como falhas no registro de ponto, necessidade de justificativa de ausência, solicitações pendentes de ajustes e atualizações no banco de horas.


### Requisitos Não Funcionais

RNF01 Desenvolver projetos de BD, utilizar as técnicas de armazenamento de tratamento de dados não estruturados. 

RNF02.Aplicar linguagens de programação back-end no desenvolvimento de aplicações e serviços web do tipo REST. 

RNF03.Empregar linguagens de POO e utilizar Padrões de Projetos no desenvolvimento de aplicações. 

RNF04.Linguagens Java, JavaScript e TypeScript. 

RNF05.Framework Spring MVC. 

RNF06.Framework React

RNF07.Manual do usuário

RNF08.Usabilidade: Interface intuitiva, fácil navegação e design responsivo adaptável a diferentes dispositivos.

RNF09.Guia de Instalação: Instruções claras para a instalação do sistema em diferentes ambientes.


<br>


## DoR (Definition of Ready) 

User Stories completas: Todos os requisitos descritos em User Stories planejadas para caber na sprint.

Tarefas detalhadas e atribuídas: Cada User Story deve ter ao menos uma task detalhada e atribuída a um responsável.

Critérios de aceitação definidos: Cada User Story deve ter critérios de aceitação bem estabelecidos.

Estimativas definidas: Todas as User Stories devem ter uma estimativa de esforço/tamanho feita pelo time

Wireframe/Mockup aprovados: O cliente deve ter validado e aprovado os protótipos visuais.

Modelo de dados finalizado: Estrutura de dados completamente definida e documentada.

Testes de aceitação definidos: Incluindo testes sugeridos pelo cliente e testes de aceitação.

Ambiente de desenvolvimento pronto: O time deve ter acesso a todos os ambientes, ferramentas e permissões necessárias.

<br>

## DoD (Definition of Done) 

Critérios de aceitação validados: Todos os critérios de aceitação foram atendidos e verificados com testes apropriados.

Execução de testes adequados: Testes unitários, de integração e de aceitação foram realizados para garantir a estabilidade e funcionamento correto da aplicação.

Código-fonte completo e padronizado: O código está 100% implementado, refatorado e segue as boas práticas e padrões de qualidade definidos.

Commits organizados e documentados: Os commits seguem a nomenclatura acordada, são claros, segmentados e possuem histórico bem documentado.

Guia de instalação detalhado: A documentação de instalação é clara e completa, permitindo que qualquer usuário ou desenvolvedor configure e execute a aplicação sem dificuldades.

Manual do usuário disponível: Um manual foi criado para orientar o cliente sobre o funcionamento da aplicação.


<br>

<span id="autores">

# 👥 Autores


|    Função     | Nome                                  |                                                                                                                                                      LinkedIn & GitHub                                                                                                                                                      |
| :-----------: | :------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|  Team Member  | Brenno Rosa Lyrio de Oliveira               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/brennolyrio/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/BrennoLyrio)   |
| Scrum Master  | André Salerno |      [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/andresalerno/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/andresalerno)     |
| Team Member   | Eric Lourenço Mendes da Silva      |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)]() [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/ericloumendes)        |
|  Team Member  | Gustavo Muraoka Silva                 |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/gustavo-muraoka-4256721ba/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/gustavomuraoka)        |
|  Product Owner  | Sarah Montuani Batagioti               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/sarahbatagioti/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/SarahBatagioti)   |
|  Team Member  | Karen de Cássia Gonçalves     |           [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/karen-cgonçalves) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/karengoncalves8)   |
|  Team Member  | Guilherme dos Santos Benedito               |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/guilherme-benedito/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/gui-benedito)   |
|  Team Member  | Arthur Johannes Rodrigues Peres y Peres              |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/ajperes/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/ajperes)   |

![image 6](https://github.com/andresalerno/projeto_api/assets/105525498/a7ca2b45-b638-4ae3-a1aa-d4b533acc6ab)
