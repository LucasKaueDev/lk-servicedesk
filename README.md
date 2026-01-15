<!-- =========================================================
   LK ServiceDesk - README Premium (Layout Colorido)
========================================================= -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6a00ff&height=220&section=header&text=LK%20ServiceDesk&fontSize=55&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=HelpDesk%20%7C%20SLA%20Automático%20%7C%20Dashboard&descAlignY=60&descSize=18" width="100%"/>

<br/>

<p>
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-ffd000?style=for-the-badge&logo=github&logoColor=black" />
  <img src="https://img.shields.io/badge/Backend-Node.js%20%7C%20Express-00e676?style=for-the-badge&logo=node.js&logoColor=black" />
  <img src="https://img.shields.io/badge/Database-PostgreSQL-00b0ff?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Frontend-HTML%20%7C%20CSS%20%7C%20JS-ff7043?style=for-the-badge&logo=javascript&logoColor=black" />
</p>

<br/>

<h3>🚀 Sistema de chamados para simular um Service Desk real</h3>
<p>
  Um projeto moderno para portfólio: <b>controle de chamados + SLA automático + dashboard + histórico</b>.
</p>

<br/>

<p align="center">
  <a href="#-visão-geral"><img src="https://img.shields.io/badge/📌%20Visão%20Geral-6a00ff?style=flat-square"/></a>
  <a href="#-funcionalidades"><img src="https://img.shields.io/badge/✨%20Funcionalidades-ff7043?style=flat-square"/></a>
  <a href="#-sla-automático"><img src="https://img.shields.io/badge/⏱️%20SLA-00b0ff?style=flat-square"/></a>
  <a href="#-stack-do-projeto"><img src="https://img.shields.io/badge/🧩%20Stack-00e676?style=flat-square"/></a>
  <a href="#-estrutura-do-projeto"><img src="https://img.shields.io/badge/🗂️%20Estrutura-ffd000?style=flat-square"/></a>
  <a href="#-roadmap"><img src="https://img.shields.io/badge/🛣️%20Roadmap-ff1744?style=flat-square"/></a>
</p>



</div>

---

## 📌 Visão Geral

<div align="center">

<table>
<tr>
<td width="33%" align="center">

### 🎯 Objetivo
Organizar chamados de TI com fluxo claro e acompanhamento fácil.

</td>
<td width="33%" align="center">

### 🧩 Problema
Planilhas e ferramentas ruins atrapalham prazos, status e histórico.

</td>
<td width="33%" align="center">

### 💡 Solução
Interface web rápida com SLA e alertas visuais automáticos.

</td>
</tr>
</table>

</div>

---

## ✨ Funcionalidades

<div align="center">

<table>
<tr>
<td width="50%" valign="top">

### ✅ Módulo de Chamados 🎫
- [ ] Criar chamado (título, descrição, categoria, prioridade)
- [ ] Listar chamados com filtros (status, prioridade, categoria)
- [ ] Visualizar detalhes do chamado
- [ ] Atualizar status (fluxo completo)
- [ ] Editar prioridade e categoria

</td>
<td width="50%" valign="top">

### ✅ Módulo de SLA ⏱️ (Diferencial)
- [ ] SLA automático por prioridade (`due_at`)
- [ ] Alertas visuais de SLA vencido
- [ ] Lista de chamados vencidos no Dashboard
- [ ] Destaque de chamados críticos

</td>
</tr>

<tr>
<td width="50%" valign="top">

### ✅ Comentários e Histórico 💬
- [ ] Comentários por chamado
- [ ] Registro de eventos (status/prioridade)
- [ ] Auditoria e rastreabilidade

</td>
<td width="50%" valign="top">

### ✅ Dashboard 📊
- [ ] Total de chamados
- [ ] Chamados abertos / em andamento
- [ ] Chamados vencidos (SLA estourado)
- [ ] Tempo médio de resolução (simples)

</td>
</tr>
</table>

</div>

---

## ⏱️ SLA Automático

<div align="center">

### 🔥 Regras do SLA
✅ Ao abrir um chamado → o sistema define automaticamente o prazo  
✅ Se `agora > due_at` → chamado vira **VENCIDO**  
✅ Chamados vencidos ganham destaque visual no sistema

<br/>

<table>
<tr>
<th align="center">Prioridade</th>
<th align="center">SLA</th>
<th align="center">Cor</th>
</tr>
<tr>
<td align="center"><b>Baixa</b></td>
<td align="center">72 horas</td>
<td align="center">🟢</td>
</tr>
<tr>
<td align="center"><b>Média</b></td>
<td align="center">48 horas</td>
<td align="center">🔵</td>
</tr>
<tr>
<td align="center"><b>Alta</b></td>
<td align="center">24 horas</td>
<td align="center">🟠</td>
</tr>
<tr>
<td align="center"><b>Crítica</b></td>
<td align="center">4 horas</td>
<td align="center">🔴</td>
</tr>
</table>

</div>

---

## 🧭 Status do Chamado

<div align="center">

✅ Fluxo padrão do sistema:

```txt
ABERTO → EM ANDAMENTO → EM ESPERA → RESOLVIDO → FECHADO
