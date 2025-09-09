# WorkSpace – Gestão de espaços para coworking

**Equipe de Produto:** AConstUNI  
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
   3.2 [Product Backlog Priorizado](#32-product-backlog-priorizado)  
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

As **User Stories** foram definidas considerando as necessidades das personas.  

Principais funcionalidades:  
- Acesso ao site com redirecionamento por perfil.  
- Gerenciamento de salas pelo gerente.  
- Controle de entrada/saída por funcionários.  
- Aluguel esporádico e fixo de workspaces.  
- Gerenciamento de membros da sala.  
- Pedidos de recursos e serviços.  
- Adição de novos recursos pelo gerente.  
- Gerenciamento de estoque de recursos.  
- Visualização de relatórios mensais pelo gerente.  

### 3.1 Diagrama de Casos de Uso
<img width="1766" height="1710" alt="image" src="https://github.com/user-attachments/assets/73ec834c-988b-4904-85d3-29fb56b3a2c2" />

### 3.2 Product Backlog Priorizado (MoSCoW)

**Must Have (Obrigatório)**  
- Acesso ao site (cliente, gerente, funcionário).  
- Aluguel esporádico de salas.  
- Gerenciamento de pessoas com acesso à sala.  
- Gerenciamento de salas pelo gerente.  
- Pedidos de recursos/serviços por clientes.  
- Adição de recursos/serviços pelo gerente.  
- Gestão de estoque (funcionário e gerente).  

**Should Have (Importante, mas pode esperar)**  
- Relatório mensal de salas usadas e recursos consumidos.  
- Gestão de acesso de funcionários da empresa.  
- Alertas automáticos para falta de recursos.  
- Painel de pedidos de limpeza para funcionários.  
- Notificações em tempo real.  

**Could Have (Desejável, mas não necessário)**  
- Customização do espaço para clientes fixos.  
- Integração com calendários externos.  
- Dashboard financeiro detalhado.  

**Won’t Have (Fora do escopo agora)**  
- Automação física de entrada/saída.  
- Aplicativo mobile nativo.  
- Programas de fidelidade.  

---

## 4. Requisitos Não Funcionais
- **Disponibilidade:** 99% do tempo.  
- **Performance:** Respostas < 2 segundos em buscas e calendários.  
- **Segurança:** Autenticação com senha criptografada (bcrypt ou similar).  
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
