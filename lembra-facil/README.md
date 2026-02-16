# 📱 Lembra Fácil

Aplicativo Android desenvolvido para auxiliar pessoas com 60+ anos a
gerenciar tarefas recorrentes e não recorrentes de forma simples, clara
e acessível.

Projeto construído com arquitetura profissional utilizando Kotlin,
Jetpack Compose e boas práticas modernas de desenvolvimento Android.

------------------------------------------------------------------------

## 🎯 Problema

Pessoas mais velhas frequentemente possuem múltiplas responsabilidades
mensais (contas, compromissos, propriedades, obrigações recorrentes) e
enfrentam dificuldade ao utilizar aplicativos complexos.

A maioria das soluções existentes:

-   Possui excesso de funcionalidades
-   Exige curva de aprendizado elevada
-   Foca em controle financeiro detalhado
-   Não prioriza simplicidade

O **Lembra Fácil** propõe uma solução minimalista e direta.

------------------------------------------------------------------------

## 💡 Proposta de Solução

Experiência principal:

> Abrir o app → Ver tarefas do dia → Marcar como Feito ou Lembrar mais
> tarde

Sem dashboards complexos.\
Sem gráficos desnecessários.\
Interface focada em clareza e previsibilidade.

------------------------------------------------------------------------

## 🚀 Funcionalidades (MVP)

-   Cadastro de tarefas únicas
-   Cadastro de tarefas recorrentes (semanal/mensal)
-   Listagem de tarefas do dia
-   Marcação como "Feito"
-   Opção "Mais tarde" (Snooze)
-   Geração automática da próxima ocorrência
-   Persistência local com Room
-   Notificações com WorkManager

------------------------------------------------------------------------

## 🏗 Arquitetura

O projeto foi estruturado com foco profissional:

-   MVVM (Model-View-ViewModel)
-   Clean Architecture
-   Repository Pattern
-   Injeção de Dependência com Hilt
-   Coroutines + Flow
-   Persistência com Room
-   Agendamento com WorkManager

Fluxo de dados:

UI → ViewModel → UseCase → Repository → DataSource (Room)

------------------------------------------------------------------------

## 🛠 Tecnologias Utilizadas

-   Kotlin
-   Jetpack Compose
-   Material 3
-   Room
-   WorkManager
-   Hilt
-   Navigation Compose
-   JUnit (testes unitários)

------------------------------------------------------------------------

## 📂 Estrutura do Projeto

    core/
    di/
    utils/

    data/
     ├── local/
     ├── repository/
     └── mapper/

    domain/
     ├── model/
     ├── usecase/
     └── repository/

    ui/
     ├── today/
     ├── tasks/
     ├── edit/
     ├── navigation/
     └── components/

------------------------------------------------------------------------

## 📊 Planejamento e Gestão

O desenvolvimento foi organizado com:

-   GitHub Projects (Kanban)
-   Issues e Sub-Issues
-   Padrão de commits vinculado a tarefas
-   Controle de tempo com Clockify

Estimativa do MVP: \~38 horas.

------------------------------------------------------------------------

## 📸 Telas

-   Tela "Hoje" (principal)
-   Tela "Tarefas" (gerenciamento)
-   Tela "Nova / Editar Tarefa"

Imagens disponíveis na pasta `docs/04_telas`.

------------------------------------------------------------------------

## ⚙️ Como Executar

1.  Clonar o repositório:

    ``` bash
    git clone https://github.com/maikelhs/programacao-dispositivos-moveis
    ```

2.  Abrir no Android Studio (Giraffe ou superior)

3.  Executar em dispositivo físico ou emulador

------------------------------------------------------------------------

## 🔮 Evoluções Futuras

-   Sincronização em nuvem
-   Login com Google
-   Backup automático
-   Compartilhamento familiar
-   Melhorias avançadas de acessibilidade

------------------------------------------------------------------------

## 🎓 Objetivo Acadêmico

Projeto desenvolvido na disciplina:

**Programação para Dispositivos Móveis**\
Curso: Análise e Desenvolvimento de Sistemas

Com foco em:

-   Aplicação prática de arquitetura moderna
-   Simulação de ambiente profissional
-   Construção de portfólio técnico

------------------------------------------------------------------------

## 👨‍💻 Autor

Maikel H. da Silva\
GitHub: https://github.com/maikelhs
