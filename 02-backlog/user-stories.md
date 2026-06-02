# User Stories — CliniqFlow

## Contexto

As User Stories abaixo representam os principais requisitos funcionais do CliniqFlow para o MVP. Cada história foi escrita no formato padrão e acompanha critérios de aceite no formato Gherkin (Given/When/Then).

---

## US-01 — Agendamento de Consulta

| | |
|---|---|
| **User Story** | Como recepcionista, quero agendar consultas na plataforma, para centralizar todos os agendamentos em um único lugar. |
| **Prioridade** | Alta |
| **Estimativa** | 5 pontos |
| **Critérios de Aceite** | **Dado** que a recepcionista está logada, **Quando** preencher data, horário, médico e paciente, **Então** o agendamento deve ser salvo e aparecer na agenda do dia. |
| **Observação** | Deve bloquear horários já ocupados para evitar duplo agendamento. |

---

## US-02 — Lembrete Automático de Consulta

| | |
|---|---|
| **User Story** | Como gestor da clínica, quero que o sistema envie lembretes automáticos aos pacientes, para reduzir faltas e cancelamentos de última hora. |
| **Prioridade** | Alta |
| **Estimativa** | 3 pontos |
| **Critérios de Aceite** | **Dado** que uma consulta está agendada, **Quando** faltar 24 horas para o horário, **Então** o sistema deve enviar um lembrete automático ao paciente via WhatsApp ou SMS. |
| **Observação** | O paciente deve poder confirmar ou cancelar pelo lembrete. |

---

## US-03 — Prontuário Eletrônico

| | |
|---|---|
| **User Story** | Como médico, quero registrar e acessar o prontuário do paciente na plataforma, para ter o histórico completo disponível antes e durante a consulta. |
| **Prioridade** | Alta |
| **Estimativa** | 8 pontos |
| **Critérios de Aceite** | **Dado** que o médico está logado e acessando uma consulta agendada, **Quando** abrir o prontuário do paciente, **Então** deve visualizar o histórico de atendimentos anteriores e poder registrar o atendimento atual. |
| **Observação** | Dados do prontuário devem seguir as diretrizes da LGPD e do CFM. |

---

## US-04 — Dashboard de KPIs

| | |
|---|---|
| **User Story** | Como gestor da clínica, quero visualizar os principais indicadores operacionais em um dashboard, para tomar decisões baseadas em dados. |
| **Prioridade** | Alta |
| **Estimativa** | 8 pontos |
| **Critérios de Aceite** | **Dado** que o gestor está logado, **Quando** acessar o dashboard, **Então** deve visualizar: total de consultas do dia, taxa de faltas, ocupação da agenda e faturamento estimado. |
| **Observação** | Dashboard deve ser atualizado em tempo real. |

---

## US-05 — Lista de Espera

| | |
|---|---|
| **User Story** | Como recepcionista, quero adicionar pacientes a uma lista de espera, para preencher automaticamente horários cancelados. |
| **Prioridade** | Média |
| **Estimativa** | 5 pontos |
| **Critérios de Aceite** | **Dado** que um paciente cancelou a consulta, **Quando** o horário ficar disponível, **Então** o sistema deve notificar o primeiro paciente da lista de espera. |
| **Observação** | Paciente da lista de espera deve confirmar em até 2 horas ou o próximo é notificado. |
