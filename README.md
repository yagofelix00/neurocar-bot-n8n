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

Algumas melhorias já estavam mapeadas no desenho da solução, mas não foram
implementadas nesta versão por limitação de tempo, mantendo o foco no fluxo
principal de vendas.

Entre elas:

- Persistir leads em banco de dados
- Integração com CRM (ex: HubSpot, Pipedrive)
- Inventário dinâmico via API externa
- Dashboard de acompanhamento de vendas
- **Notificação ativa do consultor humano no momento do handoff**  
  (ex: envio automático de mensagem via Telegram, Slack ou Webhook com os dados
  do cliente e contexto da negociação)

Essas evoluções foram pensadas para uma próxima iteração do projeto, caso ele
fosse levado para um ambiente de produção real.

---

## 🎯 Objetivo do projeto

Demonstrar capacidade de:
- Modelar fluxos reais de negócio
- Trabalhar com automação e IA aplicada
- Criar soluções prontas para produção
