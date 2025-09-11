# WorkSpace – Gestão de espaços para coworking

**Equipe de Produto:** AConstUNI - Caio David de Sousa Coutinho, Izak Vasconcelos Pinheiro, João Pedro Bezerra Silva, João Luiz Alves Mamede Netto, Tatiane Oliveira e Silva

**Product Owner:** Alex Junio Constantino  
**Data:** [data da entrega do documento para a equipe de desenvolvimento]  

---

# Sumário
1. [Introdução](#1-introdução)  
   1.1 [Visão Geral do Projeto](#11-visão-geral-do-projeto)  
   1.2 [Escopo do Projeto](#12-escopo-do-projeto)  
   1.3 [Glossário de Termos](#13-glossário-de-termos)  
2. [Personas e Público-Alvo](#2-personas-e-público-alvo)  
3. [Requisitos Funcionais](#3-requisitos-funcionais)  
   3.1 [Diagrama de Casos de Uso](#31-diagrama-de-casos-de-uso)  
   3.2 [Product Backlog Priorizado MoSCoW](#32-product-backlog-priorizado-moscow)  
4. [Requisitos Não Funcionais](#4-requisitos-não-funcionais)  
5. [Recomendações para a Equipe de Desenvolvimento](#5-recomendações-para-a-equipe-de-desenvolvimento)  
   5.1 [Sugestão para o Mínimo Produto Viável (MVP)](#51-sugestão-para-o-mínimo-produto-viável-mvp)  
   5.2 [Principais Desafios Técnicos Previstos](#52-principais-desafios-técnicos-previstos)  
   5.3 [Pontos de Atenção](#53-pontos-de-atenção)   

---

## 1. Introdução

### 1.1 Visão Geral do Projeto
O coworking é um local de trabalho compartilhado, onde empresas, CNPJs MEI, freelancers, startups, advogados etc. utilizam de forma esporádica ou contínua, dependendo das suas necessidades — seja para uma rápida reunião com um cliente, seja para um uso fixo até alcançar estabilidade e migrar para um local próprio.  

**O Problema:**  
A gestão de um coworking é uma grande responsabilidade e bastante complexa, tanto pela quantidade de aspectos a se administrar quanto pela diversidade de clientes. Há múltiplos espaços para gerenciar, com contratos de locação de curto e longo prazo, além de recursos alugados. Isso pode gerar conflitos de agendamento, indisponibilidade de recursos e demora causada pela burocracia, levando à insatisfação dos clientes.  

**Nossa Visão:**  
O **WorkSpace** busca simplificar a gestão da ampla gama de produtos e recursos, oferecendo a possibilidade de os próprios inquilinos realizarem a reserva de espaços e serviços. Assim, cada cliente poderá usufruir dos recursos de acordo com suas necessidades, com mais autonomia e menos burocracia.  

### 1.2 Escopo do Projeto
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

### 1.3 Glossário de Termos
- **Coworking:** Espaço compartilhado de trabalho.  
- **Recurso:** Produto ou serviço adicional (ex.: café, papel, limpeza).  
- **Contrato de locação:** Documento digital gerado automaticamente para formalizar reservas.  
- **Cliente esporádico:** Usuário que utiliza o espaço de forma pontual.  
- **Cliente fixo:** Usuário com contrato mensal de uso contínuo.  
- **Gerente:** Administrador responsável pela gestão de espaços, contratos e recursos.  
- **Funcionário:** Colaborador responsável por apoio operacional, organização e limpeza.  

---

## 2. Personas e Público-Alvo

### Público-Alvo
- Profissionais autônomos e freelancers que utilizam coworking.  
- Pequenas e médias empresas que alugam salas esporadicamente.  
- Gestores de coworking que precisam de controle sobre os espaços.  
- Equipes remotas que precisam de reuniões presenciais pontuais.  

### Personas
**Persona 1: O cliente esporádico – Carlos, o Advogado**  
- **Objetivos:** Ter um local confiável, alugar rápido e sem burocracia, gerenciar gastos.  
- **Dores:** Demora do gestor, burocracia, risco de sobreposição de agenda.  

**Persona 2: O cliente fixo – André, dono de startup**  
- **Objetivos:** Espaço fixo mensal, aluguel de recursos, acompanhamento de gastos, controle de acesso da equipe.  
- **Dores:** Contratos inflexíveis, pouca personalização, risco de multa em quebra de contrato.  

**Persona 3: A gerente – Mônica**  
- **Objetivos:** Divulgar espaços, automatizar contratos, facilitar gestão de recursos.  
- **Dores:** Perda de tempo com contratos manuais, dificuldade em monitorar recursos, falta de controle total.  

**Persona 4: O funcionário – Ângelo**  
- **Objetivos:** Monitorar recursos, atender solicitações de limpeza, acompanhar entradas/saídas.  
- **Dores:** Reposição manual, registros de acesso manuais, risco de esquecer solicitações.  

---

## 3. Requisitos Funcionais

#### Acesso ao site
Como qualquer usuário, quero acessar o site e ser redirecionado para a área adequada.  

**Critérios de Aceite:**
- Dado que sou um cliente, quero acessar o agendamento/locação de espaço e posteriormente os pedidos de serviço/recursos.  
- Dado que sou um funcionário, quero acessar os serviços requeridos e os recursos e o controle de entrada/saida de pessoas.  
- Dado que sou um gerente, quero acessar os agendamentos/locações, os recursos e o relatório mensal.  

---

#### Gerenciamento de salas
Como gerente (Mônica), quero conseguir gerenciar as salas no sistema.  

**Critérios de Aceite:**
- Dado que estou na área de gerenciamento de salas, quero visualizar todas as salas cadastradas no sistema e saber se estão livres ou ocupadas.  
- Dado que cliquei em uma sala, quero poder bloqueá-la para realizar reformas.  
- Dado que selecionei a opção de cadastro de sala, quero receber um formulário para preencher as informações da sala.  

---

#### Controle de entrada e saída de pessoas
Como funcionário (Ângelo), quero conseguir atualizar a entrada e saída de pessoas no sistema.  

**Critérios de Aceite:**
- Dado que estou na área de gestão de entrada/saída, quero visualizar as pessoas que estão nas salas.  
- Dado que cliquei no botão de adicionar pessoa, quero poder selecionar uma pessoa cadastrada e adicionar que ela entrou ou saiu.  

---

#### Aluguel esporádico de workspace
Como cliente esporádico (Carlos), quero abrir o website e procurar um escritório adequado para realizar minha reunião com meu cliente.  

**Critérios de Aceite:**  
- Dado que estou na tela de agendamento, quando seleciono o escritório desejado, quero visualizar os horários disponíveis e preços.  
- Dado que realizei a reserva, quero receber automaticamente o contrato de locação, especificando a data, horário e preço do espaço.  

---

#### Aluguel fixo de workspace
Como cliente fixo (André), quero abrir o website e, em uma seção específica para locações de longa duração, escolher um local de trabalho para meu negócio que está começando.  

**Critérios de Aceite:**  
- Dado que escolhi meu workspace na tela de locação, quero realizar o cadastro de minha empresa no sistema.  
- Dado que a locação foi realizada com sucesso, a sala não deve mais aparecer disponível em nenhuma parte do sistema, e o contrato deve estar acessível na tela.  

---

#### Gerenciamento de membro da sala
Como cliente (André ou Carlos), quero abrir o site e poder adicionar uma pessoa como membro da sala.  

**Critérios de Aceite:**  
- Dado que possuo uma sala alugada/alocada, quero poder cadastrar uma pessoa para ela ter acesso a sala.  
- Dado que selecione uma pessoa, quero visualizar os horários de entrada e saída da mesma.  
- Dado que selecione uma pessoa, quero poder remover o acesso da mesma.  

---

#### Pedidos de recursos e serviços
Como cliente (André ou Carlos), quero abrir o site e requisitar recursos ou serviços para a sala alugada/alocada.  

**Critérios de Aceite:**  
- Dado que possuo uma sala alugada/alocada, quero poder solicitar recursos ou serviços disponíveis no site para minha sala.  

---

#### Adição de novos recursos ou serviços
Como gerente (Mônica), quero adicionar novos recursos ou serviços no sistema através do website.  

**Critérios de Aceite:**  
- Dado que estou na página de recursos, quero ter uma aba para cadastrar novos produtos/serviços no sistema.  
- Dado que selecionei a aba, quero preencher um formulário para cadastrar o produto/serviço.  
- Dado que o produto foi cadastrado com sucesso, quero receber um alerta confirmando a adição.  

---

#### Gerenciamento de recursos
Como funcionário (Ângelo) ou gerente (Mônica), quero acessar a página de recursos para visualizar e catalogar os recursos recebidos.  

**Critérios de Aceite:**  
- Dado que acessei a página de recursos, quero visualizar todos os recursos cadastrados no sistema.  
- Dado que filtrei os recursos por “em falta”, quero visualizar quais estão com problemas ou indisponíveis.  
- Dado que selecionei a opção de adicionar recursos, quero cadastrar produtos no sistema através de um formulário com opções pré-definidas.  

---

#### Visualização de relatório mensal
Como gerente (Mônica), quero visualizar o relatório mensal da empresa.  

**Critérios de Aceite:**  
- Dado que acesso o site, quero visualizar o relatório mensal de salas utilizadas e serviços/recursos consumidos.  

---


### 3.1 Diagrama de Casos de Uso
![Imagem do WhatsApp de 2025-09-09 à(s) 13 51 39_9aa18b53](https://github.com/user-attachments/assets/4d609a65-9bea-41af-8319-4f26ffa1f19f)

### 3.1.1 Especificações dos Casos de Uso
---
#### Casos de Uso do Membro
---
##### UC01 – Login / Autenticação
- **Ator Principal:** Membro  
- **Objetivo:** Permitir que o membro acesse o sistema de forma segura.  
- **Pré-condições:** O membro deve estar previamente cadastrado.  
- **Fluxo Principal:**  
  1. O membro informa credenciais (usuário e senha).  
  2. O sistema valida as credenciais.  
  3. O sistema autentica o membro e libera acesso as funcionalidades de membro.  
- **Fluxos Alternativos:**  
  - Credenciais inválidas → sistema exibe mensagem de informações incorretas.  
- **Exceções:**  
  - Falha de comunicação com o servidor → login não realizado.


##### UC02 – Reserva sala
- **Ator Principal:** Membro  
- **Objetivo:** Reservar uma sala ou estação de trabalho disponível.  
- **Pré-condições:** Usuário autenticado; recurso ativo.  
- **Fluxo Principal:**  
  1. O membro acessa o calendário.  
  2. Seleciona sala/estação, data e horário.  
  3. O sistema verifica disponibilidade.  
  4. O sistema impede conflitos de horário.  
  5. O sistema confirma a reserva.  
  6. O sistema envia notificação de sucesso.  
- **Fluxos Alternativos:**  
  - Intervalo inválido → sistema informa o erro.  
  - Fora da política de tempo → sistema recusa.  
- **Exceções:**  
  - Recurso inativo ou bloqueado.   


##### UC03 – Cancela reserva
- **Ator Principal:** Membro  
- **Objetivo:** Cancelar uma reserva existente.  
- **Pré-condições:** Usuário autenticado; reserva existente.  
- **Fluxo Principal:**  
  1. O membro acessa suas reservas.  
  2. Seleciona a reserva a ser cancelada.  
  3. O sistema remove a reserva.  
  4. O sistema envia notificação de sucesso.  
- **Exceções:**
  - Reserva já iniciada → sistema mostra mensagem de erro e volta a tela de reserva.


##### UC04 – Edita reserva
- **Ator Principal:** Membro  
- **Objetivo:** Adicionar acesso de pessoas a sala.  
- **Pré-condições:** Usuário autenticado; reserva existente.  
- **Fluxo Principal:**  
  1. O membro seleciona a reserva.  
  2. O membro seleciona a opção de adição de pessoa.
  3. O membro informa o nome da pessoa.  
  4. O sistema verifica se ja tem alguem com o mesmo nome.  
  5. O sistema confirma a adição.  
  6. O sistema envia notificação de sucesso.  
- **Fluxo Alternativo:**
  - O membro clica na pessoa → sistema mostra as entradas e saídas daquela pessoa


##### UC05 – Visualiza disponibilidade
- **Ator Principal:** Membro  
- **Objetivo:** Consultar disponibilidade de salas/estações.  
- **Fluxo Principal:**  
  1. O membro acessa o calendário.  
  2. O sistema exibe recursos disponíveis e horários livres.  


##### UC06 – Recebe notificação de reserva
- **Ator Principal:** Membro  
- **Objetivo:** Informar ao membro sobre confirmações ou alterações de reservas.  
- **Pré-condições:** O membro deve possuir reservas registradas.  
- **Fluxo Principal:**  
  1. O sistema envia notificação ao membro após criação, alteração ou cancelamento de uma reserva.  


---
#### Casos de Uso do Gestor
---
##### UC07 – Login / Autenticação
- **Ator Principal:** Gestor  
- **Objetivo:** Permitir que o gestor acesse o sistema de forma segura.  
- **Pré-condições:** O gestor deve estar previamente cadastrado.  
- **Fluxo Principal:** Quase igual ao UC01 (Login do Membro) mudando apenas libera o acesso para as funcionalidades de gestor.  


##### UC08 – Cadastra recursos
- **Ator Principal:** Gestor  
- **Objetivo:** Incluir salas/estações no sistema.  
- **Pré-condições:** Gestor autenticado.  
- **Fluxo Principal:**  
  1. Gestor acessa menu de recursos.  
  2. Informa dados do recurso.  
  3. O sistema valida duplicidade.  
  4. O sistema registra recurso.  
  5. O sistema envia notificação de sucesso.


##### UC09 – Cadastra serviços
- **Ator Principal:** Gestor  
- **Objetivo:** Incluir serviços (ex.: limpeza, manutenção).  
- **Fluxo Principal:**  
  1. Gestor acessa menu de serviços.  
  2. Informa dados do serviço.  
  3. O sistema valida duplicidade.  
  4. O sistema registra serviço.  
  5. O sistema envia notificação de sucesso.  


##### UC10 – Edita recurso
- **Ator Principal:** Gestor  
- **Objetivo:** Alterar dados de um recurso existente.  
- **Fluxo Principal:**  
  1. Gestor seleciona recurso.  
  2. Informa novos dados.  
  3. O sistema atualiza registro.  
  4. O sistema envia notificação de sucesso.  


##### UC11 – Exclui recurso
- **Ator Principal:** Gestor  
- **Objetivo:** Remover um recurso.  
- **Fluxo Principal:**  
  1. Gestor seleciona recurso.  
  2. Confirma exclusão.  
  3. O sistema exclui recurso.  
  4. O sistema envia notificação de sucesso.  


##### UC12 – Visualiza todas as reservas
- **Ator Principal:** Gestor  
- **Objetivo:** Consultar todas as reservas registradas.  
- **Fluxo Principal:**  
  1. Gestor acessa relatórios de reservas.  
  2. O sistema exibe todas as reservas com status.  


##### UC13 – Gera relatórios de utilização
- **Ator Principal:** Gestor  
- **Objetivo:** Emitir relatórios de ocupação.  
- **Fluxo Principal:**  
  1. Gestor solicita relatório.  
  2. O sistema gera relatório consolidado.  


##### UC14 – Gerencia membros
- **Ator Principal:** Gestor  
- **Objetivo:** Incluir, editar ou remover membros.  
- **Fluxo Principal:**  
  1. Gestor acessa módulo de membros.  
  2. Realiza operação desejada.  
  3. O sistema confirma alteração.  

---
#### Casos de Uso do Funcionário
---
##### UC15 – Login / Autenticação
- **Ator Principal:** Funcionário  
- **Objetivo:** Permitir que o funcionário acesse o sistema de forma segura.  
- **Pré-condições:** Funcionário deve estar previamente cadastrado.  
- **Fluxo Principal:** Quase igual ao UC01 (Login do Membro) mudando apenas libera o acesso para as funcionalidades de funcionário.  


##### UC16 – Visualiza recursos
- **Ator Principal:** Funcionário  
- **Objetivo:** Consultar recursos disponíveis para manutenção/serviço.  
- **Fluxo Principal:**  
  1. Funcionário acessa menu de recursos.  
  2. O sistema exibe lista de recursos.  


##### UC17 – Registra serviços
- **Ator Principal:** Funcionário  
- **Objetivo:** Registrar execução de serviços (limpeza, manutenção, etc.).  
- **Fluxo Principal:**  
  1. Funcionário seleciona serviço.  
  2. Informa data/hora e status.  
  3. O sistema registra execução.  
  4. O sistema envia notificação de sucesso.  


#### UC18 – Atualiza status de recurso
- **Ator Principal:** Funcionário  
- **Objetivo:** Atualizar o status de um recurso (ativo, manutenção, indisponível).  
- **Fluxo Principal:**  
  1. Funcionário acessa recurso.  
  2. Altera status.  
  3. O sistema registra alteração.  
  4. O sistema envia notificação de sucesso.
 
---

### 3.2 Product Backlog Priorizado (MoSCoW)

**Must Have (Obrigatório)**  
- [M1] Login com redirecionamento para sua devida área (cliente, gerente, funcionário).  
- [M2] Gerenciamento de salas pelo gerente.  
- [M3] Aluguel esporádico de salas. 
- [M4] Aluguel fixo de salas com geração de contrato automático. 
- [M5] Adição de recursos/serviços pelo gerente.  
- [M6] Pedidos de recursos/serviços por clientes.  
- [M7] Gestão de estoque (funcionário e gerente).  

**Should Have (Importante, mas pode esperar)**  
- [S1] Relatório mensal de salas usadas e recursos consumidos.
- [S2] Gestão de acesso de pessoas realizado pelo cliente.
- [S3] Painel de pedidos de limpeza para funcionários.
- [S4] Notificações em tempo real.
- [S5] Alertas automáticos para falta de recursos.

**Could Have (Desejável, mas não necessário)**  
- [C1] Customização do espaço para clientes fixos.  
- [C2] Integração com calendários externos.  
- [C3] Dashboard financeiro detalhado.  

**Won’t Have (Fora do escopo agora)**  
- [W1] Programas de fidelidade.  
- [W2] Aplicativo mobile nativo.  
- [W3] Automação física de entrada/saída.  

---

## 4. Requisitos Não Funcionais
- **Disponibilidade:** 99% do tempo.  
- **Performance:** Respostas < 2 segundos em buscas e calendários.  
- **Segurança:** Autenticação com senha criptografada.  
- **Escalabilidade:** Até 500 usuários simultâneos.  
- **Usabilidade:** Interface responsiva e intuitiva.  
- **Confiabilidade:** Garantir integridade das reservas em acessos simultâneos.  

---

## 5. Recomendações para a Equipe de Desenvolvimento

### 5.1 Sugestão para o Mínimo Produto Viável (MVP)
- Login e autenticação.  
- Reserva de salas (esporádica).  
- Gerenciamento básico de salas pelo gerente.  
- Pedidos de recursos e serviços.  
- Gestão simples de estoque.  

### 5.2 Principais Desafios Técnicos Previstos
- Evitar sobreposição de reservas em acessos simultâneos.  
- Gerenciar permissões diferentes entre cliente, gerente e funcionário.  
- Manter escalabilidade com até 500 usuários ativos.  
- Garantir notificações confiáveis (emails, alertas no sistema).  

### 5.3 Pontos de Atenção
- UX deve ser intuitiva para diferentes perfis de usuários.  
- Integração futura com meios de pagamento precisa ser planejada.  
- O sistema deve prever possíveis conflitos de agendamento em tempo real.  
- Registro de logs para auditoria e rastreabilidade.  
