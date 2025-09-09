# WorkSpace

## 1. Resumo
O coworking é um local de trabalho compartilhado, onde empresas, CNPJs MEI, freelancers, startups, advogados etc. utilizam de forma esporádica ou contínua, dependendo das suas necessidades — seja para uma rápida reunião com um cliente, seja para um uso fixo até alcançar estabilidade e migrar para um local próprio.

## 2. Visão
**O Problema:** A gestão de um coworking é uma grande responsabilidade e bastante complexa, tanto pela quantidade de aspectos a se administrar quanto pela diversidade de clientes. Há múltiplos espaços para gerenciar, com contratos de locação de curto e longo prazo, além de recursos alugados. Isso pode gerar conflitos de agendamento, indisponibilidade de recursos, além da demora causada pela burocracia, o que pode levar à insatisfação dos clientes.  

**Nossa Visão:** O WorkSpace busca simplificar a gestão da ampla gama de produtos e recursos, oferecendo a possibilidade de os próprios inquilinos realizarem a reserva de espaços e serviços. Assim, cada cliente poderá usufruir dos recursos de acordo com suas necessidades, com mais autonomia e menos burocracia.  

## 3. Público-Alvo
- Profissionais autônomos e freelancers que utilizam coworking.  
- Pequenas e médias empresas que alugam salas esporadicamente.  
- Gestores de coworking que precisam de controle sobre os espaços.  
- Equipes remotas que precisam de reuniões presenciais pontuais.  

## 4. Escopo
**Incluso**
- Cadastro e autenticação de usuários (clientes, gerente, funcionários).  
- Reserva de salas (esporádica ou fixa).  
- Gestão de salas e contratos pelo gerente.  
- Requisição de recursos e serviços adicionais.  
- Gestão de estoque de recursos (funcionários + gerente).  
- Relatórios mensais para gestão financeira e operacional.  
- Portal único com redirecionamento para a área específica de cada perfil.  

**Não Incluso (fora do escopo inicial)**  
- Integração direta com meios de pagamento externos (ex.: PayPal, Stripe).  
- Automação física de portas, catracas e sensores.  
- Aplicativo mobile nativo.  

## 5. Personas
### Persona 1: O cliente esporádico  
**Nome:** Carlos, o Advogado  

**Perfil:**  
Profissional que atende clientes em diversas cidades. Precisa, de forma rápida e simplificada, de um espaço para reuniões pontuais.  

**Objetivos:**  
- Ter um local confiável para trabalhar.  
- Alugar de forma simples, rápida e sem burocracia.  
- Gerenciar seus gastos de maneira clara e acessível.  

**Dores:**  
- Demora na resposta do gestor do coworking.  
- Burocracia excessiva no aluguel.  
- Risco de sobreposição de agenda.  

---

### Persona 2: O cliente fixo  
**Nome:** André, o dono de startup  

**Perfil:**  
Empreendedor com uma ideia inovadora que precisa de um espaço fixo até consolidar sua empresa.  

**Objetivos:**  
- Ter um local para consolidar sua empresa, com aluguel mensal.  
- Poder alugar recursos e solicitar serviços adicionais.  
- Acompanhar gastos com aluguel e recursos.  
- Gerenciar o acesso de seus funcionários ao coworking.  

**Dores:**  
- Contrato inflexível em caso de mudança.  
- Não poder personalizar o espaço conforme suas necessidades.  
- Risco de multa na quebra de contrato.  

---

### Persona 3: A gerente  
**Nome:** Mônica, gerente do coworking  

**Perfil:**  
Responsável por administrar escritórios e espaços de trabalho, alugando-os com contratos flexíveis, de curto ou longo prazo.  

**Objetivos:**  
- Divulgar seus espaços disponíveis.  
- Automatizar contratos e cobranças.  
- Facilitar a gestão de recursos.  

**Dores:**  
- Perda de tempo elaborando contratos manuais.  
- Dificuldade para monitorar recursos remotamente.  
- Falta de controle total sobre o consumo no coworking.  

---

### Persona 4: O funcionário  
**Nome:** Ângelo, funcionário do coworking  

**Perfil:**  
Auxiliar contratado para organização, limpeza e reposição de produtos.  

**Objetivos:**  
- Monitorar a falta de recursos (sabonete, papel higiênico, café etc.).  
- Atender solicitações de limpeza.  
- Acompanhar entrada e saída de pessoas.  

**Dores:**  
- Dificuldade para acompanhar a reposição em áreas comuns.  
- Necessidade de verificar manualmente registros de acesso.  
- Risco de esquecer pedidos manuais de limpeza, gerando insatisfação.  

## 6. User Stories
### Acesso ao site

Como qualquer usuário, quero acessar o site e ser redirecionado para a área adequada.  

**Critérios de Aceite:**
- Dado que sou um cliente, quero acessar o agendamento/locação de espaço e posteriormente os pedidos de serviço/recursos.
- Dado que sou um funcionário, quero acessar os serviços requeridos e os recursos e o controle de entrada/saida de pessoas.
- Dado que sou um gerente, quero acessar os agendamentos/locações, os recursos e o relatório mensal.

---

### Gerenciamento de salas

Como gerente (Mônica), quero conseguir gerenciar as salas no sistema.  

**Critérios de Aceite:**
- Dado que estou na área de gerenciamento de salas, quero visualizar todas as salas cadastradas no sistema e saber se estão livres ou ocupadas.
- Dado que cliquei em uma sala, quero poder bloqueá-la para realizar reformas.
- Dado que selecionei a opção de cadastro de sala, quero receber um formulário para preencher as informações da sala.

---

### Controle de entrada e saida de pessoas

Como funcionário (Ângelo), quero conseguir atualizar a entrada e saída de pessoas no sistema.

**Critérios de Aceite:**
- Dado que estou na área de gestão de entrada/saída, quero visualizar as pessoas que estão nas salas
- Dado que cliquei no botão de adicionar pessoa, quero poder selecionar uma pessoa cadastrada e adicionar que ela entrou ou saiu.

---

### Aluguel esporádico de workspace

Como cliente esporádico (Carlos), quero abrir o website e procurar um escritório adequado para realizar minha reunião com meu cliente.  

**Critérios de Aceite:**  
- Dado que estou na tela de agendamento, quando seleciono o escritório desejado, quero visualizar os horários disponíveis e preços.  
- Dado que realizei a reserva, quero receber automaticamente o contrato de locação, especificando a data, horário e preço do espaço.  

---

### Aluguel fixo de workspace

Como cliente fixo (André), quero abrir o website e, em uma seção específica para locações de longa duração, escolher um local de trabalho para meu negócio que está começando.  

**Critérios de Aceite:**  
- Dado que escolhi meu workspace na tela de locação, quero realizar o cadastro de minha empresa no sistema.  
- Dado que a locação foi realizada com sucesso, a sala não deve mais aparecer disponível em nenhuma parte do sistema, e o contrato deve estar acessível na tela.  

---

### Gerenciamento de membro da sala

Como cliente (André ou Carlos), quero abrir o site e poder adicionar uma pessoa como membro da sala.  

**Critérios de Aceite:**  
- Dado que possuo uma sala alugada/alocada, quero poder cadastrar uma pessoa para ela ter acesso a sala.
- Dado que selecione uma pessoa, quero visualizar os horários de entrada e saída da mesma.
- Dado que selecione uma pessoa, quero poder remover o acesso da mesma.

---

### Pedidos de recursos e serviços

Como cliente (André ou Carlos), quero abrir o site e requisitar recursos ou serviços para a sala alugada/alocada.  

**Critérios de Aceite:**  
- Dado que possuo uma sala alugada/alocada, quero poder solicitar recursos ou serviços disponíveis no site para minha sala.  

---

### Adição de novos recursos ou serviços

Como gerente (Mônica), quero adicionar novos recursos ou serviços no sistema através do website.  

**Critérios de Aceite:**  
- Dado que estou na página de recursos, quero ter uma aba para cadastrar novos produtos/serviços no sistema.  
- Dado que selecionei a aba, quero preencher um formulário para cadastrar o produto/serviço.  
- Dado que o produto foi cadastrado com sucesso, quero receber um alerta confirmando a adição.  

---

### Gerenciamento de recursos

Como funcionário (Ângelo) ou gerente (Mônica), quero acessar a página de recursos para visualizar e catalogar os recursos recebidos.  

**Critérios de Aceite:**  
- Dado que acessei a página de recursos, quero visualizar todos os recursos cadastrados no sistema.  
- Dado que filtrei os recursos por “em falta”, quero visualizar quais estão com problemas ou indisponíveis.  
- Dado que selecionei a opção de adicionar recursos, quero cadastrar produtos no sistema através de um formulário com opções pré-definidas.  

---

### Visualização de relatório mensal

Como gerente (Mônica), quero visualizar o relatório mensal da empresa.  

**Critérios de Aceite:**  
- Dado que acesso o site, quero visualizar o relatório mensal de salas utilizadas e serviços/recursos consumidos.  

---

## 7. Casos de Uso
### Diagrama
<img width="1766" height="1710" alt="image" src="https://github.com/user-attachments/assets/73ec834c-988b-4904-85d3-29fb56b3a2c2" />

### Casos de Uso Identificados

**Atores**
- **Membro**: usuário que reserva salas e estações de trabalho.  
- **Gestor**: administrador do coworking, responsável pela gestão dos recursos.  

**Casos de Uso do Membro**
- Reserva sala  
- Cancela reserva  
- Edita reserva  
- Login / Autenticação  
- Visualiza disponibilidade  
- Recebe notificação de reserva  

**Casos de Uso do Gestor**
- Cadastra recursos  
- Edita recurso  
- Exclui recurso  
- Visualiza todas as reservas  
- Gera relatórios de utilização  
- Gerencia membros  

---

### Detalhamento do Caso de Uso — **Reserva sala**

**Nome:** Reserva sala  
**Ator Principal:** Membro  
**Stakeholders:** Membro, Gestor  
**Objetivo:** Permitir que o membro reserve uma sala ou estação em horário livre.  
**Trigger:** Membro seleciona um recurso e inicia a solicitação de reserva.  

**Pré-condições**
- Membro autenticado.  
- Recurso ativo e disponível no sistema.  

**Pós-condições**
- **Sucesso:** Reserva confirmada e salva com status “ativa”; notificação enviada (quando habilitada).  
- **Falha:** Nenhuma alteração feita; mensagem de erro exibida.  

**Fluxo Principal**
1. O membro acessa o calendário de um recurso.  
2. Seleciona data, hora de início e término.  
3. O sistema **inclui** “Visualiza disponibilidade”.  
4. O sistema **inclui** “Impedir reserva em horário ocupado” para validar conflitos.  
5. O sistema confirma a criação da reserva.  
6. O sistema **estende** “Recebe notificação de reserva”, caso notificações estejam habilitadas.  

**Fluxos Alternativos**
- **FA1 — Intervalo inválido:** se término ≤ início, o sistema exibe erro e retorna ao passo 2.    
- **FA2 — Fora da política:** se a data exceder o limite configurado (ex.: até 30 dias à frente), o sistema rejeita e informa a política.  

**Exceções**
- **E1 — Conflito:** outro membro já reservou o mesmo horário → sistema bloqueia e sugere alternativas.  
- **E2 — Falha de comunicação:** reserva confirmada, mas notificação não entregue; sistema registra log.  
- **E3 — Condição de corrida:** duas reservas simultâneas → apenas a primeira confirmada é persistida.  
- **E4 — Recurso inativo:** caso o recurso esteja inativo, o sistema bloqueia a ação.  

**Regras de Negócio**
- **RN1:** Não permitir sobreposição de horários em um mesmo recurso.  
- **RN2:** Definir duração mínima (30 min) e máxima (4h).  
- **RN3:** Reservas devem respeitar o horário de funcionamento do coworking.  
- **RN4:** Cada membro só pode criar, editar e cancelar suas próprias reservas.  
- **RN5:** Gestores têm acesso de visualização a todas as reservas.  

**Critérios de Aceitação**
- **CA1:** Dado que uma sala está livre entre 14:00–15:00, quando o membro reserva nesse intervalo, então o sistema confirma e exibe a reserva.  
- **CA2:** Dado que existe reserva entre 10:00–11:00, quando outro membro tenta reservar 10:30–11:00, então o sistema recusa e informa conflito.  
- **CA3:** Dado que notificações estão habilitadas, quando a reserva é confirmada, então o membro recebe notificação.  

---

## 8. Backlog com Priorização MoSCoW
### Must Have (Obrigatório)
- Acesso ao site com redirecionamento para áreas de cliente, gerente ou funcionário.  
- Aluguel esporádico de salas (busca, escolha de horário, preço, contrato automático).  
- Gerenciamento de pessoas com acesso a sala pelo cliente (associados do cliente que está alugando a sala).
- Gerenciamento de salas pelo gerente (cadastrar, bloquear para reforma, visualizar ocupação).  
- Pedidos de recursos e serviços para clientes com salas alugadas.  
- Adição de recursos/serviços pelo gerente.  
- Visualização de recursos e gestão de estoque (gerente e funcionário).  

### Should Have (Importante, mas pode esperar)
- Relatório mensal de salas usadas e recursos consumidos para o gerente.  
- Gestão de acesso dos funcionários da empresa (cliente fixo).  
- Alertas automáticos para falta de recursos (estoque baixo).  
- Painel para funcionários acompanharem pedidos de limpeza.  
- Notificações em tempo real (ex.: confirmação de reserva, pedido atendido).

### Could Have (Desejável, mas não necessário)
- Customização do espaço pelo cliente fixo (layout, serviços adicionais).  
- Integração com calendário externo (Google/Outlook).  
- Dashboard financeiro detalhado para o gerente.  

### Won’t Have (Fora do escopo agora)
- Automação física de entrada/saída (portas inteligentes, catracas).  
- Aplicativo mobile nativo (apenas responsividade web).  
- Planos de fidelidade ou programas de pontos.  

---

## 9. Requisitos Não Funcionais
- **Disponibilidade:** O sistema deve estar disponível 99% do tempo.  
- **Performance:** As buscas e visualizações de calendário devem carregar em menos de 2 segundos.  
- **Segurança:** Autenticação segura com senha criptografada (bcrypt ou similar).  
- **Escalabilidade:** Suporte para até 500 usuários simultâneos.  
- **Usabilidade:** Interface intuitiva e responsiva para desktop e mobile.  
- **Confiabilidade:** Garantir integridade das reservas, evitando conflitos mesmo em acessos simultâneos.  

