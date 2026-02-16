# 📱 Telas do Aplicativo -- Lembra Fácil

## 📌 1. Visão Geral

Este documento descreve as telas do aplicativo **Lembra Fácil**,
detalhando suas funções, comportamentos esperados e fluxo de navegação.

O objetivo é garantir clareza na experiência do usuário e alinhamento
entre design e implementação técnica.

------------------------------------------------------------------------

## 🏠 2. Tela Principal -- Hoje

### 🎯 Objetivo

Exibir exclusivamente as tarefas do dia atual, permitindo ação rápida e
direta.

### 📋 Elementos da Tela

-   Nome do aplicativo
-   Data atual
-   Lista de tarefas do dia
-   Botões de ação:
    -   ✅ Feito
    -   ⏰ Mais tarde
-   Informação da próxima tarefa futura (rodapé)

### ✅ Ação: Feito

Ao tocar:

1.  A tarefa é marcada como concluída.
2.  O status visual muda (ex: fundo verde + ícone ✔).
3.  Se a tarefa for recorrente:
    -   A próxima ocorrência é criada automaticamente.
4.  A tarefa deixa de aparecer na lista do dia após atualização.

### ⏰ Ação: Mais tarde

Ao tocar:

1.  A tarefa é adiada.
2.  O sistema agenda nova exibição:
    -   Algumas horas depois **OU**
    -   No dia seguinte (regra definida internamente).
3.  Pode sair temporariamente da lista atual.

### 🎨 Indicadores Visuais

-   🟢 Verde → Concluída\
-   🟠 Laranja → Adiada\
-   ⚪ Normal → Pendente

------------------------------------------------------------------------

## 📂 3. Tela -- Tarefas

### 🎯 Objetivo

Gerenciar todas as tarefas cadastradas.

### 📋 Elementos da Tela

-   Lista completa de tarefas
-   Frequência da tarefa (ex: semanal, mensal)
-   Botão ➕ Nova Tarefa
-   Menu de opções (⋮):
    -   ✏️ Editar
    -   🗑️ Excluir

### ➕ Nova Tarefa

Abre a tela de cadastro.

### ✏️ Editar

Permite alterar:

-   Nome
-   Frequência
-   Data inicial
-   Categoria

### 🗑️ Excluir

Exibe confirmação:

> "Deseja realmente excluir esta tarefa?"

Se confirmado:

-   Remove permanentemente a tarefa
-   Remove futuras ocorrências associadas

⚠ Esta ação não pode ser desfeita.

------------------------------------------------------------------------

## 📝 4. Tela -- Nova / Editar Tarefa

### 🎯 Objetivo

Criar ou modificar tarefas.

### 📌 Campos Disponíveis

#### 🏷 Nome da Tarefa

Campo obrigatório.

Exemplos:

-   Tomar remédio
-   Pagar conta de luz
-   Fazer exercícios

#### 🔁 Frequência

-   Uma vez
-   Semanal
-   Mensal

Define a regra de repetição automática.

#### 📅 Data Inicial

Define o início da tarefa.

Exemplos:

-   Hoje
-   Próxima segunda-feira
-   Dia 5 do mês

#### 🗂 Categoria (Opcional)

Exemplos:

-   Saúde
-   Financeiro
-   Exercícios
-   Pessoal
-   Outros

### 💾 Botão Salvar

-   Registra a tarefa
-   Cria primeira ocorrência (se recorrente)
-   Retorna à tela anterior

### ❌ Botão Cancelar

Fecha sem salvar alterações.

------------------------------------------------------------------------

## 🔔 5. Notificações

O aplicativo envia alertas quando:

-   A tarefa estiver próxima do horário definido
-   A tarefa estiver vencida

Possibilidades futuras:

-   Marcar como concluída direto pela notificação
-   Abrir aplicativo diretamente na tarefa

------------------------------------------------------------------------

## 🔄 6. Fluxo de Navegação

Hoje → Tarefas → Nova Tarefa\
Hoje → Tarefas → Editar\
Hoje → Feito / Mais tarde

Fluxo principal:

Abrir app → Visualizar tarefas do dia → Executar ação → Encerrar

------------------------------------------------------------------------

## 📌 7. Diretrizes de UX

O design prioriza:

-   Simplicidade
-   Botões grandes
-   Poucas opções por tela
-   Clareza visual
-   Acessibilidade para público 60+

------------------------------------------------------------------------

## 📊 8. Observações Técnicas

Cada ação da interface está vinculada a:

-   ViewModel (camada de apresentação)
-   UseCase (regra de negócio)
-   Repository (persistência)
-   Room (armazenamento local)

Essa separação garante:

-   Testabilidade
-   Manutenção facilitada
-   Arquitetura escalável
