# 🤖 NeuroCar Bot — Agente de Vendas Automotivo com IA

Agente de IA para atendimento e qualificação de leads de concessionária via Telegram, 
com fluxo completo de vendas automatizadas e handoff para consultor humano.

---

## 🚗 O que esse projeto faz

- Atende clientes automaticamente no Telegram
- Qualifica leads (nome, contato, orçamento, tipo de carro)
- Apresenta veículos do inventário
- Conduz o cliente até o fechamento
- Realiza handoff para consultor humano no momento correto

---

## 🧠 Como funciona o fluxo

1. Cliente envia mensagem via Telegram
2. Mensagem é capturada pelo n8n (Telegram Trigger)
3. Contexto é extraído (chatId, userId, mensagem)
4. Agente de IA interpreta a intenção do cliente
5. IA consulta inventário local (JSON)
6. Conversa evolui conforme estágio da venda
7. No fechamento:
   - Cliente é avisado que será atendido por um humano
   - Dados permanecem registrados na sessão

---

## 🧩 Tecnologias utilizadas

- **n8n**
- **OpenAI (GPT-4o-mini)**
- **Telegram Bot API**
- **JSON (inventário local)**
- **Conversation Memory**

---

## 🔄 Estágios de venda implementados

- Credenciamento do lead
- Navegação por veículos
- Simulação de compra e financiamento
- Fechamento
- Transferência para consultor humano

---

## ✅ Diferenciais técnicos

- Uso de **Conversation Memory** para manter contexto
- Lógica de **handoff humano** no momento do fechamento
- Inventário desacoplado da IA
- Fluxo resiliente a mensagens fora de ordem
- Projeto totalmente funcional sem backend próprio

---

## 📌 Próximos passos (evoluções planejadas)

Este projeto foi pensado de forma modular e escalável. Algumas evoluções naturais foram mapeadas, mas não implementadas neste MVP para manter o foco no fluxo principal de vendas e handoff.

Entre elas:

- 📊 Persistência de leads (ex: Google Sheets, banco de dados ou CRM)

- 🔔 Notificação ativa do consultor humano no momento do handoff

  - Envio automático de mensagem com nome, contato, orçamento e carro de interesse

  - Continuidade do atendimento diretamente via WhatsApp


- 📅 Controle centralizado de agendamentos de test drive

  - Evitar marcação do mesmo veículo no mesmo horário

  - Visão única de agenda por carro/data


- 🔁 Estratégias de follow-up para leads que não fecharam no primeiro contato

- 📈 Dashboard de acompanhamento do funil de vendas

- 🔌 Integração com CRMs (ex: HubSpot, Pipedrive

Essas evoluções foram pensadas para uma próxima iteração do projeto, caso ele
fosse levado para um ambiente de produção real.

---

## 🎯 Objetivo do projeto

Demonstrar capacidade de:
- Modelar fluxos reais de negócio
- Trabalhar com automação e IA aplicada
- Criar soluções prontas para produção
