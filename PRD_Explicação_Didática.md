pesquisa_prd.md
100%
# Guia Prático: O que é um PRD (Product Requirements Document)?

Na Engenharia de Software e Gestão de Produtos, o **PRD (Documento de Requisitos do Produto)** é o guia mestre de um projeto. Ele funciona como a "planta baixa" ou a "bússola" para equipes de produto, design e engenharia.

Se continuarmos com a analogia do **carro**:

* Os **Requisitos** são as especificações de cada peça (o motor, as rodas, o cinto).
* O **PRD** é o **manual de engenharia completo do carro**: ele explica quem vai dirigir, o propósito do veículo, os requisitos funcionais/não funcionais, os objetivos de negócio e as métricas de sucesso.

---

## 1. Qual é a finalidade de um PRD?

O objetivo principal de um PRD é alinhar **todos os envolvidos no projeto** sobre:
1. **Por que** estamos construindo isso? (Problema & Valor)
2. **Para quem** estamos construindo? (Público-alvo / Personas)
3. **O que** será construído? (Escopo & Funcionalidades)
4. **Como** saberemos se deu certo? (Métricas / KPIs)

> **A pergunta de ouro:** *"O que exatamente precisamos construir para resolver o problema do usuário, e como mediremos o sucesso?"*

---

## 2. Anatomia de um PRD Estruturado

Um bom PRD não precisa ser um documento longo e burocrático, mas sim **claro, conciso e acionável**. Ele costuma conter as seguintes seções:

1. **Visão Geral & Problema:** Descrição do problema que o produto resolve.
2. **Público-Alvo:** Quem se beneficiará da solução.
3. **Métricas de Sucesso (KPIs):** Indicadores que mostram o impacto do projeto.
4. **Requisitos Funcionais & Casos de Uso:** O que o usuário poderá fazer.
5. **Requisitos Não Funcionais:** Restrições técnicas e de desempenho.
6. **Fora de Escopo (Out of Scope):** O que **NÃO** será feito nesta fase (evita o acúmulo de escopo).

---

## 3. Estudo de Caso: PRD do Módulo "Clube de Assinatura" (Estilo iFood)

Abaixo está um exemplo prático de um PRD simplificado focado em uma funcionalidade real.

```markdown
# [PRD] Módulo de Assinatura: Delivery VIP (iFood Club)

## 1. Visão Geral
* **Objetivo:** Criar um programa de assinatura mensal para aumentar a retenção de clientes e a frequência de pedidos.
* **Problema:** Clientes deixam de pedir com frequência devido ao valor acumulado da taxa de entrega.
* **Solução:** Oferecer cupons de frete grátis mediante uma taxa fixa mensal.

## 2. Público-Alvo & Personas
* **Persona Principal:** Marcos, 28 anos, pede comida via app 3 a 5 vezes por semana e busca economizar em taxas de entrega.

## 3. Métricas de Sucesso (KPIs)
* Aumentar em **25%** a frequência média de pedidos dos assinantes.
* Alcançar **100.000 assinantes pagos** nos primeiros 90 dias após o lançamento.
* Manter a taxa de cancelamento (Churn) abaixo de **5% ao mês**.

## 4. Requisitos Funcionais (RF)
* **RF01 - Adesão ao Plano:** O usuário deve conseguir assinar o plano com cobrança recorrente no cartão de crédito.
* **RF02 - Aplicar Desconto Automático:** O checkout deve identificar o assinante e aplicar o cupom de frete grátis automaticamente.
* **RF03 - Gestão da Assinatura:** O usuário deve conseguir visualizar seus cupons disponíveis e cancelar a renovação a qualquer momento.

## 5. Requisitos Não Funcionais (RNF)
* **RNF01 - Tempo de Resposta:** A verificação de status do assinante durante o checkout deve demorar no máximo **100ms**.
* **RNF02 - Segurança:** As informações de cobrança recorrente devem seguir o padrão PCI-DSS.

## 6. Fora de Escopo (V1)
* *Não* teremos suporte a pagamento de assinatura via PIX nesta primeira versão (apenas cartão de crédito).
* *Não* haverá planos corporativos/em grupo na V1.
```

---

## 💡 Resumo Prático: Por que usar um PRD?

| Sem PRD ❌ | Com PRD ✅ |
| :--- | :--- |
| Equipes de design e desenvolvimento com visões diferentes. | Todos trabalham com a mesma fonte de verdade (*Single Source of Truth*). |
| Mudanças constantes no escopo durante o desenvolvimento. | Escopo bem delimitado e priorizado. |
| Dificuldade para medir o retorno financeiro ou impacto. | Critérios de sucesso claros desde o primeiro dia. |
