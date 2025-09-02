# WorkSpace

## 1. Resumo
O WorkSpace é uma plataforma web e mobile para gerenciamento e reserva de salas de reunião e estações de trabalho em espaços de coworking. Inspirado no modelo do Regus, o sistema permite que membros visualizem a disponibilidade em um calendário interativo, façam reservas e cancelem quando necessário, garantindo o controle de conflitos de agendamento em tempo real.

## 2. Visão
Facilitar a gestão de espaços de trabalho compartilhados, oferecendo aos membros uma forma rápida, intuitiva e segura de reservar recursos, otimizando o uso das salas e garantindo maior aproveitamento do coworking.

## 3. Público-Alvo
Profissionais autônomos e freelancers que utilizam coworking.

Pequenas e médias empresas que alugam salas esporadicamente.

Gestores de coworking que precisam de controle de uso dos espaços.

Equipes remotas que precisam de reuniões presenciais pontuais.

## 4. Escopo
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

## 5. Personas
### João Silva – Freelancer de Marketing
32 anos, trabalha em coworking para reuniões com clientes.

- Valoriza praticidade e visualização rápida de horários.

### Ana Souza – Gestora de Coworking

40 anos, administra os espaços e controla a disponibilidade.

- Precisa evitar conflitos de agendamento e manter ocupação alta.

### Carlos Mendes – Desenvolvedor Remoto

28 anos, reserva estações de trabalho para produtividade extra.

- Busca interface simples e fácil cancelamento.

### Maria Oliveira – Consultora Empresarial

45 anos, aluga salas de reunião para treinamentos.

- Precisa agendar com antecedência e evitar sobreposição.

## 6. User Stories
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
