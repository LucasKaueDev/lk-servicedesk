# LK ServiceDesk 🛠️📩

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)](#)
[![Stack](https://img.shields.io/badge/stack-Node.js%20%7C%20Express%20%7C%20PostgreSQL-blue)](#)
[![Frontend](https://img.shields.io/badge/frontend-HTML%20%7C%20CSS%20%7C%20JavaScript-orange)](#)
[![License](https://img.shields.io/badge/license-MIT-green)](#licen%C3%A7a)

Sistema **HelpDesk / Service Desk** para gerenciamento de chamados de TI, com **controle de status** e **SLA automático por prioridade**, focado em simular um cenário real de suporte.

---

## 🎯 Objetivo

Centralizar e organizar chamados de suporte de TI, permitindo:
- Criação e acompanhamento do fluxo do chamado
- Prioridade e prazo (SLA) definido automaticamente
- Alertas visuais quando o SLA estiver vencido
- Visão rápida por dashboard

---

## 🧩 Problema

Muitas equipes de TI ainda dependem de planilhas ou ferramentas pouco flexíveis para gerenciar chamados, o que dificulta:
- Acompanhamento do status
- Priorização eficiente
- Cumprimento de prazos (SLA)
- auditoria e histórico

---

## 💡 Solução

O **LK ServiceDesk** oferece uma interface web simples e objetiva para:
- Abrir chamados
- Acompanhar o andamento
- Registrar comentários e eventos
- Controlar SLA por prioridade
- Destacar chamados vencidos visualmente

---

## 🛠️ Tecnologias

### Front-end
- HTML
- CSS
- JavaScript (Vanilla)

### Back-end
- Node.js
- Express

### Banco de dados
- PostgreSQL

---

## 🚀 Funcionalidades (MVP)

### ✅ Chamados
- [ ] Criar chamado (título, descrição, categoria, prioridade)
- [ ] Listar chamados com filtros (status, prioridade, categoria)
- [ ] Visualizar detalhes do chamado
- [ ] Atualizar status: **Aberto → Em Andamento → Resolvido → Fechado**
- [ ] Editar prioridade e categoria

### ✅ SLA (Diferencial)
- [ ] SLA automático por prioridade (define `due_at`)
- [ ] Alertas visuais de SLA vencido
- [ ] Lista de chamados vencidos no Dashboard

### ✅ Comentários e Histórico
- [ ] Comentários por chamado
- [ ] Registro de eventos (mudanças de status/prioridade)

### ✅ Dashboard
- [ ] Total de chamados
- [ ] Chamados abertos / em andamento
- [ ] Chamados vencidos (SLA estourado)
- [ ] Tempo médio de resolução (simples)

---

## ⏱️ SLA por prioridade (padrão do projeto)

| Prioridade | SLA |
|-----------|-----|
| Baixa     | 72 horas |
| Média     | 48 horas |
| Alta      | 24 horas |
| Crítica   | 4 horas |

---

## 🧭 Status do chamado

- **ABERTO**
- **EM ANDAMENTO**
- - **EM ESPERA**
- **RESOLVIDO**
- **FECHADO**

---

## 🗂️ Estrutura do Projeto (planejada)

```txt
lk-servicedesk/
  backend/
    src/
      routes/
      controllers/
      middleware/
      db/
      server.js
  frontend/
    index.html
    css/
    js/
  README.md
