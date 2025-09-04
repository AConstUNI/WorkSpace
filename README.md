# WorkSpace

## 1. Resumo
O cowork space e um local de trabalho compartilhado, onde empresas, CNPJ’s MEI, freelancer’s, start-up’s, advogados, etc... utilizam de forma esporádica ou continua dependendo das suas necessidades, seja para uma rápida reunião com um cliente, até um local fixo até gerar uma estabilidade para alugar ou construir local próprio de uma start-up 

## 2. Visão
O Problema: A gestão de um coworking space e uma grande responsabilidade e complicada, tanto pela quantidade de coisas a se gerir, quanto pela quantidade de clientes que se pode existir, são muitos espaços para se cuidar de contrato de locação a longo prazo como também a curto prazo, muitos materiais alugados, assim podendo ocorrer conflitos de agendamentos, aluguel de recursos já esgotados, alem da possível demora causada pela burocracia de agendamentos, assim podendo causar insatisfação do cliente 

Nossa Visão: o COS: Cow Orc Space e simplificar a gestão da grande gama de produtos, assim como facilitar a gestão dos recursos do work space, dando a possibilidade dos próprios inquilinos fazerem o aluguel de seus espaços e dos recursos disponibilizado pelo local, assim fazendo que cada cliente possa usufruir dos recursos adequados as necessidades deles. 


## 3. Público-Alvo
Profissionais autônomos e freelancers que utilizam coworking.

Pequenas e médias empresas que alugam salas esporadicamente.

Gestores de coworking que precisam de controle de uso dos espaços.

Equipes remotas que precisam de reuniões presenciais pontuais.


## 4. Personas
### Persona 1:  O cliente esporádico 

Nome: Carlos, o Advogado.  

Perfil:  
  Profissional que aceita serviços em diversas cidades, ele tem um cliente e precisa rapidamente e de forma simplificada um espaço para fazer suas reuniões naquela cidade. 

Objetivos:  
- Ter um local a qual procurar uma área de trabalho. 
- Alugar de forma simples, rápida, autónoma e simplificada sem enfrentar burocracia de contrato de aluguel e riscos de sobreposição de agenda. 
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
- Não poder estar presencialmente acompanhando a disponibilidade de recursos. 
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

## 5. User Stories
### Reserva de Sala

Como membro, quero reservar uma sala de reunião em um horário disponível, para realizar reuniões com clientes.

### Visualização de Disponibilidade

Como membro, quero visualizar no calendário a disponibilidade das salas, para escolher um horário adequado.

### Cancelamento de Reserva

Como membro, quero cancelar minha reserva, para liberar o espaço caso não possa comparecer.

### Cadastro de Recursos

Como gestor, quero cadastrar novas salas e estações, para disponibilizá-las para reserva.

### Bloqueio de Horário Ocupado

Como sistema, quero impedir que um recurso seja reservado em horário já ocupado, para evitar conflitos de agendamento.

## 6. Escopo
Incluso
- Cadastro e autenticação de membros.
- Cadastro de recursos (salas e estações).
- Visualização de disponibilidade em calendário.
- Reserva de recursos com bloqueio de horários já ocupados.
- Cancelamento de reservas pelo próprio usuário.
- Notificações de confirmação e cancelamento.

Não Incluso (fora do escopo inicial)
- Pagamento online.
- Integração com APIs externas de calendário (Google, Outlook).
- Gestão financeira do coworking.
- Recursos de chat ou videoconferência.


## 7. Diagramas de Caso de Uso
<img width="1766" height="1710" alt="image" src="https://github.com/user-attachments/assets/73ec834c-988b-4904-85d3-29fb56b3a2c2" />

## 8. Backlog com Priorização MoSCoW
### Must Have (Obrigatório)

[M1] Cadastro de membros.

[M2] Cadastro de recursos (salas/estações).

[M3] Visualização de disponibilidade no calendário.

[M4] Realizar reservas.

[M5] Bloqueio de horários ocupados.

[M6] Cancelamento de reservas pelo usuário.

### Should Have (Importante, mas pode esperar)

[S1] Notificações por e-mail de confirmação/cancelamento.

[S2] Filtros de busca por tipo de sala ou capacidade.

### Could Have (Desejável, mas não necessário)

[C1] Integração com Google Calendar.

[C2] Histórico de reservas anteriores.


### Won’t Have (Fora do escopo agora)

[W1] Pagamento online.

[W2] Relatórios financeiros do coworking.

## 9. Requisitos Não Funcionais
Disponibilidade: O sistema deve estar disponível 99,5% do tempo.

Performance: As buscas e visualizações de calendário devem carregar em menos de 2 segundos.

Segurança: Autenticação segura com senha criptografada (bcrypt ou similar).

Escalabilidade: Suporte para até 500 usuários simultâneos.

Usabilidade: Interface intuitiva e responsiva para desktop e mobile.

Confiabilidade: Garantir integridade das reservas, evitando conflitos mesmo em acessos simultâneos.
