# WorkSpace

## 1. Resumo
O cowork space e um local de trabalho compartilhado, onde empresas, CNPJ’s MEI, freelancer’s, start-up’s, advogados, etc... utilizam de forma esporádica ou continua dependendo das suas necessidades, seja para uma rápida reunião com um cliente, até um local fixo até gerar uma estabilidade para alugar ou construir local próprio de uma start-up


## 2. Visão
O Problema: A gestão de um coworking space e uma grande responsabilidade e complicada, tanto pela quantidade de coisas a se gerir, quanto pela quantidade de clientes que se pode existir, são muitos espaços para se cuidar de contrato de locação a longo prazo como também a curto prazo, muitos materiais alugados, assim podendo ocorrer conflitos de agendamentos, aluguel de recursos já esgotados, alem da possível demora causada pela burocracia de agendamentos, assim podendo causar insatisfação do cliente 

Nossa Visão: o COS: Cow Orc Space busca simplificar a gestão da grande gama de produtos, assim como facilitar a gestão dos recursos do work space, dando a possibilidade dos próprios inquilinos fazerem o aluguel de seus espaços e dos recursos disponibilizado pelo local, assim fazendo que cada cliente possa usufruir dos recursos adequados as necessidades deles. 


## 3. Público-Alvo
Profissionais autônomos e freelancers que utilizam coworking.

Pequenas e médias empresas que alugam salas esporadicamente.

Gestores de coworking que precisam de controle de uso dos espaços.

Equipes remotas que precisam de reuniões presenciais pontuais.


## 4. Escopo
Incluso
- Cadastro e autenticação de usuários (clientes, gerente, funcionários).
- Reserva de salas (esporádica ou fixa).
- Gestão de salas e contratos pelo gerente.
- Requisição de recursos e serviços adicionais.
- Gestão de estoque de recursos (funcionários + gerente).
- Relatórios mensais para gestão financeira e operacional.
- Portal único com redirecionamento para área específica de cada perfil.

Não Incluso (fora do escopo inicial)
- Integração direta com meios de pagamento externos (ex.: PayPal, Stripe).
- Automação física de portas, catracas e sensores.
- Aplicativo mobile nativo.


## 5. Personas
### Persona 1:  O cliente esporádico 

Nome: Carlos, o Advogado.  

Perfil:  
  Profissional que aceita serviços em diversas cidades, ele tem um cliente e precisa rapidamente e de forma simplificada um espaço para fazer suas reuniões naquela cidade. 

Objetivos:  
- Ter um local a qual procurar uma área de trabalho. 
- Alugar de forma simples, rápida, autônoma e simplificada sem enfrentar burocracia de contrato de aluguel e riscos de sobreposição de agenda. 
- Gestão de gastos simplificados e acessível. 

Dores (Frustrações):  

- Demora na resposta do dono do work space. 
- Burocracia no aluguel de um ambiente. 
- Incerteza sobre problemas de sobreposição de agenda. 


### Persona 2:  O cliente fixo 

Nome: André, O dono de start-up.  

Perfil:  
  Pessoa dona de ideia inovadora, quer começar uma empresa e precisa de um local de estadia da empresa até a consolidação da base da empresa, precisa de um espaço para permanecer por um grande tempo. 

Objetivos:  
- Ter um local para consolidar sua empresa, tendo um aluguel mensal. 
- Poder alugar recursos e solicitar serviços do work space 
- Poder acompanhar o gasto de aluguel do work space e dos objetos de auxílio a serem alugados. 
- Poder gerenciar acesso dos seus funcionários dentro do work space. 

Dores (Frustrações):  
- Não ter um contrato maleável, para caso de mudança para espaço próprio. 
- Não poder moldar o seu espaço de trabalho de acordo com suas necessidades. 
- Risco de multa em caso de quebra de contrato de aluguel. 
 

### Persona 3:  A gerente 

Nome: Monica, A gerente do work space.  

Perfil:  
  A gerente do work space, onde há um aglomerado de escritórios / espaços de trabalho com serviços próprios, a qual ela aluga para pessoas que necessitam de espaços de trabalhos com contratos de locação flexível, temporário a curto e longo prazo. 

Objetivos:  
- Poder divulgar seus espaços disponíveis para as pessoas a procura de work’s spaces. 
- Não precisar fazer contratos manuais com novos clientes. 
- Não precisar gerar cobranças manuais. 
- Ter mais facilidade na gestão de recursos de seu ambiente. 

Dores (Frustrações):  
- Perder muito tempo desenvolvendo contratos para cada cliente. 
- Não poder estar acompanhando a disponibilidade de recursos de forma remota. 
- Falta de controle total sobre consumos dentro de seu work space. 

### Persona 4:  O funcionário. 

Nome: Ângelo, trabalhador do work space.  

Perfil:  
  Contratado pelo gerente, para ajudar na organização, limpeza, e reposição de produtos do work space. 

Objetivos:  
- Poder acompanhar a falta de recursos para reposição (sabonete, papel higiénico nos banheiros, café na máquina de cafés, recursos em geral) 
- Acompanhar solicitações de limpeza de escritórios. 
- Monitorar entrada e saída de pessoas. 

Dores (Frustrações):  
- Não conseguir acompanhar a reposição de recursos em ambientes comuns. 
- Necessidade de ficar procurando o registo de cada pessoa para liberar acesso. 
- Ter de acompanhar pedidos manuais ou tag’s de porta para acompanhar pedidos de limpeza de escritório, podendo assim passar algo despercebido ficando sem prestar o serviço causando insatisfação do cliente. 

## 6. User Stories
### Acesso ao site

Como qualquer um dos usuários quero acessar o site e ser redirecionado para a área que preciso

Critérios de Aceite:
- Dado que sou um cliente, quero acesso ao agendamento/locação de espaço e posteriormente aos pedidos de serviço/recursos.
- Dado que sou um funcionário, quero acesso aos serviços requeridos e aos recursos.
- Dado que sou um gerente, quero acesso aos(as) agendamentos/locações, aos recursos e ao relatório mensal.


### Gerenciamneto de salas

Como gerente (Monica) quero conseguir manipular as salas no sistema.

Critérios de Aceite:
- Dado que estou na area de gerenciamento de salas que ver todas as salas cadastradas no sistema e se elas estão livres ou ocupadas.
- Dado que clique em uma das salas quero poder bloquear ela para realizar reformas na mesma.
- Dado que selecione uma opção de cadastro de sala quero que me seja fornecido um formulário para preencher as informações da sala.


### Aluguel esporádico de um work space. 

Como um cliente esporádico (Carlos) quero abrir o website, e procurar um escritório adequado para realizar minha reunião com meu cliente. 

Critérios de Aceite: 
- Dado que eu estou na tela de realizar agendamento, quando eu seleciono o escritório desejado, deve me ser mostrado os horários disponíveis e preços. 
- Dado que eu realizei a reserva deve-me ser fornecido o contrato de locação automaticamente, especificando a data com horário e preço da locação do espaço. 


### Aluguel fixo de um work space. 

Como um cliente fixo (André) quero abrir o website e através de uma janela separada para locações de longa duração quero escolher um local de trabalho para meu negócio que esta começando. 

Critérios de Aceite: 
- Dado que eu escolhi meu work space na tela de locação, quero realizar o cadastro de minha empresa no sistema. 
- Dado que minha locação foi realizada com sucesso, é esperado que aquela sala não apareça mais para locação em nem um local do sistema e o contrato apareça na tela.


### Pedidos de recursos e serviços

Como um cliente (André ou Carlos) quero poder abrir o site e poder requisitar recursos ou serviços para a sala alugada/alocada.

Critérios de Aceite:
- Dado que eu possua uma sala alugada/alocada, quero poder pedir recursos ou serviços disponiveis no site para minha sala.


### Adição de novos recursos ou serviço

Como gerente (Monica) quero conseguir adicionar recursos novos no sistema através do website.

Critérios de Aceite:
- Dado que estou na página de recursos quero ter uma aba para cadastrar novos produtos/serviços no sistema.
- Dado que eu selecione a aba quer preencher um formulário para cadastrar o produto/serviço.
- Dado o produto seja cadastrado com sucesso quero um alerta de produto/serviço adicionado com sucesso.


### Gerenciamento de recursos

Como funcionário (Ângelo) ou gerente (Monica) quero entrar na página de recursos e visualizar os recursos e/ou catalogar os recursos que foram recebidos.

Critérios de Aceite:
- Dado que entrei na página de recursos, quero visualizar todos os recursos cadastrados no sistema.
- Dado que filtrei os recurso por recursos em falta, quero ver quais recursos estão com problemas ou em falta.
- Dado que selecionei a opção de adição de recursos, quero conseguir realizar o cadastro de produtos no sistema através de um formulário com opções pré definidas.


### Visualização de relatorio mensal

Como gerente (Monica) quero poder visualizar o relatorio mensal da empresa.

Critérios de Aceite:
- Dado que acesso o site quero visualizar o relatorio mensal de salas usadas e serviços/recursos utilizados.


## 7. Casos de Uso
### Diagrama
<img width="1766" height="1710" alt="image" src="https://github.com/user-attachments/assets/73ec834c-988b-4904-85d3-29fb56b3a2c2" />

### Casos de Uso Identificados

Atores
- **Membro**: usuário que reserva salas e estações de trabalho.  
- **Gestor**: administrador do coworking, responsável pela gestão dos recursos.  

Casos de Uso do Membro
- Reserva sala
- Cancela reserva
- Edita reserva
- Login / Autenticação
- Visualiza disponibilidade
- Recebe notificação de reserva

Casos de Uso do Gestor
- Cadastra recursos
- Edita recurso
- Exclui recurso
- Visualiza todas as reservas
- Gera relatórios de utilização
- Gerencia membros

### Detalhamento do Caso de Uso — **Reserva sala**

**Nome:** Reserva sala  
**Ator Principal:** Membro  
**Stakeholders:** Membro, Gestor  
**Objetivo:** Permitir que o membro reserve uma sala ou estação em horário livre.  
**Trigger:** Membro seleciona recurso e inicia a solicitação de reserva.  

Pré-condições
- Membro autenticado.  
- Recurso ativo e disponível no sistema.  

Pós-condições
- **Sucesso:** Reserva confirmada e salva com status “ativa”; notificação enviada (quando habilitada).  
- **Falha:** Nenhuma alteração feita; mensagem de erro exibida.  

Fluxo Principal
1. O membro acessa o calendário de um recurso.  
2. Seleciona data, hora de início e término.  
3. O sistema **inclui** “Visualiza disponibilidade”.  
4. O sistema **inclui** “Impedir reserva em horário ocupado” para validar conflitos.  
5. O sistema confirma a criação da reserva.  
6. O sistema **estende** “Recebe notificação de reserva”, caso notificações estejam habilitadas.  

Fluxos Alternativos
- **FA1 — Intervalo inválido:** se término ≤ início, o sistema exibe erro e retorna ao passo 2.    
- **FA2 — Fora da política:** se a data exceder o limite configurado (ex.: até 30 dias à frente), o sistema rejeita e informa a política.  

Exceções
- **E1 — Conflito:** outro membro já reservou o mesmo horário → sistema bloqueia e sugere alternativas.  
- **E2 — Falha de comunicação:** reserva confirmada, mas notificação não entregue; sistema registra log.  
- **E3 — Condição de corrida:** duas reservas simultâneas → apenas a primeira confirmada é persistida.
- **E4 — Recurso inativo:** caso o recurso esteja inativo, o sistema bloqueia a ação.  

Regras de Negócio
- **RN1:** Não permitir sobreposição de horários em um mesmo recurso.  
- **RN2:** Definir duração mínima (30 min) e máxima (4h).  
- **RN3:** Reservas devem respeitar o horário de funcionamento do coworking.  
- **RN4:** Cada membro só pode criar, editar e cancelar suas próprias reservas.  
- **RN5:** Gestores têm acesso de visualização a todas as reservas.  

Critérios de Aceitação
- **CA1:** Dado que uma sala está livre entre 14:00–15:00, quando o membro reserva nesse intervalo, então o sistema confirma e exibe a reserva.  
- **CA2:** Dado que existe reserva entre 10:00–11:00, quando outro membro tenta reservar 10:30–11:00, então o sistema recusa e informa conflito.  
- **CA3:** Dado que notificações estão habilitadas, quando a reserva é confirmada, então o membro recebe notificação.  


## 8. Backlog com Priorização MoSCoW
### Must Have (Obrigatório)

- Acesso ao site com redirecionamento para área de cliente, gerente ou funcionário.
- Aluguel esporádico de salas (busca, escolha de horário, preço, contrato automático).
- Aluguel fixo de salas (com cadastro de empresa, bloqueio de sala e contrato).
- Gerenciamento de salas pelo gerente (cadastrar, bloquear para reforma, visualizar ocupação).
- Pedidos de recursos e serviços para clientes com salas alugadas.
- Adição de recursos/serviços pelo gerente.
- Visualização de recursos e gestão de estoque (gerente e funcionário).


### Should Have (Importante, mas pode esperar)

- Relatório mensal de salas usadas e recursos consumidos para o gerente.
- Gestão de acesso dos funcionários da empresa (cliente fixo).
- Alertas automáticos para falta de recursos (estoque baixo).
- Painel para funcionários acompanharem pedidos de limpeza.

### Could Have (Desejável, mas não necessário)

- Customização do espaço pelo cliente fixo (layout, serviços adicionais).
- Notificações em tempo real (ex.: confirmação de reserva, pedido atendido).
- Integração com calendário externo (Google/Outlook).
- Dashboard financeiro detalhado para o gerente.


### Won’t Have (Fora do escopo agora)

- Automação física de entrada/saída (portas inteligentes, catracas).
- Aplicativo mobile nativo (apenas responsividade web).
- Planos de fidelidade ou programas de pontos.

## 9. Requisitos Não Funcionais
Disponibilidade: O sistema deve estar disponível 99% do tempo.

Performance: As buscas e visualizações de calendário devem carregar em menos de 2 segundos.

Segurança: Autenticação segura com senha criptografada (bcrypt ou similar).

Escalabilidade: Suporte para até 500 usuários simultâneos.

Usabilidade: Interface intuitiva e responsiva para desktop e mobile.

Confiabilidade: Garantir integridade das reservas, evitando conflitos mesmo em acessos simultâneos.
