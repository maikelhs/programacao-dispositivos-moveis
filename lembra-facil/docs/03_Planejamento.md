# 📌 Planejamento do Projeto -- Lembra Fácil

## 1. Objetivo

Organizar o desenvolvimento do projeto utilizando práticas profissionais
de gestão, garantindo rastreabilidade, controle de progresso e
organização das tarefas.

Ferramentas utilizadas:

-   GitHub Projects (Kanban)
-   Issues
-   Sub-issues
-   Labels
-   Controle de fluxo de desenvolvimento

------------------------------------------------------------------------

## 2. Estrutura do Kanban

O quadro Kanban foi configurado com as seguintes colunas:

📥 Backlog\
🧠 Em Análise\
🚧 Em Desenvolvimento\
🧪 Em Teste\
✅ Concluído

### Descrição das Etapas

-   **Backlog:** Tarefas ainda não iniciadas\
-   **Em Análise:** Refinamento técnico e planejamento\
-   **Em Desenvolvimento:** Implementação ativa\
-   **Em Teste:** Validação funcional e revisão\
-   **Concluído:** Tarefa finalizada

------------------------------------------------------------------------

## 3. Organização das Issues

### Issue Macro

Exemplo:

Configurar arquitetura base do projeto (MVVM)

### Sub-Issues

-   Criar estrutura base de packages\
-   Configurar dependências do Hilt\
-   Configurar Room Database\
-   Criar camada Domain (UseCases + Entities)

Essa divisão permite maior controle e rastreabilidade do
desenvolvimento.

------------------------------------------------------------------------

## 4. Labels Utilizadas

-   architecture\
-   setup

As labels auxiliam na categorização e filtragem das tarefas.

------------------------------------------------------------------------

## 5. Fluxo de Trabalho Definido

1.  Criar Issue ou Sub-Issue\
2.  Adicionar ao Project\
3.  Iniciar em 📥 Backlog\
4.  Ao iniciar desenvolvimento → mover para 🚧 Em Desenvolvimento\
5.  Após implementação → mover para 🧪 Em Teste\
6.  Após validação → mover para ✅ Concluído\
7.  Encerrar Issue

------------------------------------------------------------------------

## 6. Padrão de Commit

Foi adotado o seguinte padrão:

``` bash
feat: descrição da funcionalidade (#numero_da_issue)
```

Exemplo:

``` bash
feat: criar estrutura base de packages (#2)
```

Esse padrão conecta automaticamente o commit à Issue correspondente.

------------------------------------------------------------------------

## 7. Benefícios da Organização

-   Rastreabilidade completa\
-   Histórico claro de evolução\
-   Organização profissional\
-   Simulação de ambiente corporativo\
-   Base sólida para portfólio

------------------------------------------------------------------------

## 📌 Conclusão

A utilização do GitHub Projects elevou o projeto Lembra Fácil ao padrão
de organização utilizado por equipes profissionais de desenvolvimento,
garantindo controle, disciplina e clareza no processo de construção do
aplicativo.
