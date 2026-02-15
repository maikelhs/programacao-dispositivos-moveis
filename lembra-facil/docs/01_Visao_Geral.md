 ## 📱 Projeto: Aplicativo de Lembretes Simplificado para Tarefas Recorrentes

## 1. Visão Geral do Projeto

Este projeto propõe o desenvolvimento de um aplicativo Android focado em auxiliar pessoas com 60+ anos na gestão de tarefas recorrentes e não recorrentes, com ênfase em simplicidade, clareza e usabilidade.

A ideia surgiu de uma necessidade real: uma pessoa de 65 anos com múltiplas responsabilidades mensais (contas, compromissos religiosos, propriedades, etc.) que enfrenta dificuldades em lembrar todas as obrigações, resultando em risco de multas e estresse desnecessário.

O objetivo é criar uma solução extremamente simples e intuitiva, diferente dos aplicativos tradicionais que apresentam excesso de funcionalidades e complexidade.

---

## 2. Problema Identificado

Pessoas mais velhas frequentemente:

- Possuem múltiplas contas recorrentes (água, luz, internet, proteção veicular, dízimo, etc.)
- Precisam enviar leituras mensais (ex: energia elétrica)
- Administram mais de um imóvel
- Não se adaptam bem a aplicativos financeiros complexos
- Correm risco de esquecimento e pagamento de multas

Aplicativos existentes:
- São excessivamente complexos
- Focam em controle financeiro detalhado
- Exigem curva de aprendizado elevada

---

## 3. Proposta de Solução

Desenvolver um aplicativo com foco em:

- Interface minimalista
- Botões grandes
- Poucas telas
- Linguagem simples
- Fluxo previsível
- Interação direta via pergunta:  
  **"Você já fez esta tarefa?"**

A experiência do usuário deve ser:

> Abrir o app → Ver tarefas de hoje → Marcar como feito ou lembrar mais tarde.

Sem dashboards, gráficos ou excesso de configurações.

---

## 4. Escopo Inicial (MVP)

O MVP será desenvolvido rodando exclusivamente no celular do usuário principal (sem sincronização ou login).

### Telas previstas: 3

### 4.1 Tela 1 — "Hoje" (Tela Principal)

Função:
- Listar apenas tarefas do dia
- Exibir botões:
  - ✅ Feito
  - ⏰ Mais tarde
- Mostrar status visual simples

Essa será a tela mais utilizada.

---

### 4.2 Tela 2 — "Tarefas"

Função:
- Listar todas as tarefas cadastradas
- Permitir edição
- Permitir exclusão
- Botão "+ Nova Tarefa"

Uso principal: configuração e manutenção.

---

### 4.3 Tela 3 — "Nova / Editar Tarefa"

Campos:
- Nome da tarefa
- Frequência:
  - Uma vez
  - Semanal
  - Mensal
- Data inicial
- Categoria (opcional)

Sem opções avançadas.

---

## 5. Funcionalidades do MVP

- Cadastro de tarefas recorrentes e não recorrentes
- Persistência local de dados
- Geração automática de próxima ocorrência
- Marcação de tarefa como concluída
- Opção de lembrar mais tarde
- Notificações programadas
- Histórico de conclusão

---

## 6. Arquitetura Técnica (Modo Profissional)

O projeto será desenvolvido seguindo padrões modernos do mercado Android.

### Stack Tecnológica

- Kotlin
- Jetpack Compose
- Material 3
- MVVM
- Room (persistência local)
- WorkManager (agendamento de tarefas)
- Hilt (injeção de dependência)
- Coroutines + Flow
- Testes Unitários

---

## 7. Estrutura de Camadas

```
core/  
di/  
utils/

data/  
local/  
repository/  
mapper/

domain/  
model/  
usecase/  
repository/

ui/  
today/  
tasks/  
edit/  
navigation/  
components/
```


Essa estrutura garante:

- Separação de responsabilidades
- Facilidade de manutenção
- Testabilidade
- Aderência a padrões de mercado

---

## 8. Roadmap de Desenvolvimento

### Etapa 1
Definição de modelos e regras de negócio.

### Etapa 2
Implementação do banco local com Room.

### Etapa 3
Criação de UseCases:
- GetTodayTasks
- CreateTask
- MarkTaskAsDone
- SnoozeTask

### Etapa 4
Implementação das telas em Compose.

### Etapa 5
Agendamento de notificações com WorkManager.

### Etapa 6
Implementação de testes unitários.

### Etapa 7
Ajustes de UX e acessibilidade (foco 65+).

---

## 9. Estimativa de Tempo

Modo profissional (arquitetura completa):

- 40 a 70 horas de desenvolvimento
- 2 a 3 semanas com dedicação parcial
- 8 a 12 dias com dedicação intensa

Sem sincronização em nuvem neste momento.

---

## 10. Diferenciais do Projeto

- Baseado em necessidade real
- Foco em público negligenciado
- Arquitetura profissional
- Aplicação prática de conceitos modernos Android
- Forte potencial para portfólio

---

## 11. Evoluções Futuras (Fase 2)

- Sincronização entre dispositivos (pai e filho)
- Login com Google
- Histórico compartilhado
- Backup automático
- Relatórios simples
- Modo acessibilidade avançado

---

## 12. Objetivo Estratégico

Além de resolver um problema familiar real, este projeto tem como objetivo:

- Consolidar conhecimento em desenvolvimento Android moderno
- Praticar arquitetura profissional
- Simular ambiente de desenvolvimento de mercado
- Criar um projeto robusto para portfólio técnico

---

# Conclusão

Trata-se de um projeto tecnicamente viável, com escopo controlado, arquitetura profissional e forte potencial de aplicação real.

O desenvolvimento seguirá boas práticas de mercado e servirá tanto como solução funcional quanto como evolução profissional do desenvolvedor.
