# 🏗️ Arquitetura do Sistema -- Lembra Fácil

## 📌 1. Visão Geral Arquitetural

O projeto **Lembra Fácil** foi estruturado utilizando padrões modernos
de desenvolvimento Android, com foco em:

-   Escalabilidade
-   Testabilidade
-   Separação de responsabilidades
-   Manutenibilidade
-   Organização profissional

A arquitetura adotada combina:

-   **MVVM (Model-View-ViewModel)**
-   **Clean Architecture**
-   **Repository Pattern**
-   **Injeção de Dependência com Hilt**

------------------------------------------------------------------------

## 🧱 2. Stack Tecnológica

-   Kotlin
-   Jetpack Compose
-   Material 3
-   MVVM
-   Clean Architecture
-   Room (Persistência Local)
-   WorkManager (Agendamento)
-   Hilt (Injeção de Dependência)
-   Coroutines + Flow
-   Testes Unitários (JUnit)

------------------------------------------------------------------------

## 🏛️ 3. Estrutura em Camadas (Clean Architecture)

A aplicação foi organizada em três camadas principais:

    UI (Presentation)
    ↓
    Domain (Regras de Negócio)
    ↓
    Data (Persistência e Fontes de Dados)

### 3.1 Camada UI (Presentation)

Responsável por:

-   Exibição das telas (Jetpack Compose)
-   Interação do usuário
-   Comunicação com ViewModel

Componentes:

-   Screens (Hoje, Tarefas, Nova/Editar)
-   ViewModels
-   Navigation

A camada UI não acessa diretamente banco de dados ou regras complexas.

------------------------------------------------------------------------

### 3.2 Camada Domain

Responsável por:

-   Regras de negócio
-   Casos de uso (UseCases)
-   Modelos de domínio

Exemplos de UseCases:

-   GetTodayTasks
-   CreateTask
-   MarkTaskAsDone
-   SnoozeTask

Essa camada é independente de Android.

------------------------------------------------------------------------

### 3.3 Camada Data

Responsável por:

-   Persistência com Room
-   Implementação de Repositories
-   Mapeamento entre entidades e modelos de domínio

Componentes:

-   DAO
-   Database
-   RepositoryImpl
-   Mappers

------------------------------------------------------------------------

## 🔄 4. Fluxo de Dados

Fluxo padrão:

    UI → ViewModel → UseCase → Repository → DataSource (Room)

Fluxo detalhado:

1.  Usuário toca em botão.
2.  ViewModel recebe evento.
3.  ViewModel chama UseCase.
4.  UseCase aplica regra de negócio.
5.  Repository acessa Room.
6.  Dados retornam via Flow.
7.  UI é atualizada automaticamente.

------------------------------------------------------------------------

## 💉 5. Injeção de Dependência (Hilt)

Hilt é utilizado para:

-   Fornecer instâncias de Repository
-   Fornecer Database
-   Gerenciar ciclo de vida dos componentes

Estrutura:

-   @HiltAndroidApp
-   @AndroidEntryPoint
-   @Module + @Provides
-   @Inject

Benefícios:

-   Baixo acoplamento
-   Testabilidade
-   Código mais limpo

------------------------------------------------------------------------

## 🗃️ 6. Persistência de Dados

Banco local implementado com **Room**.

Entidades principais:

-   TaskEntity

DAO:

-   InsertTask
-   UpdateTask
-   DeleteTask
-   GetTodayTasks

Persistência totalmente local (MVP).

------------------------------------------------------------------------

## ⏰ 7. Agendamento de Notificações

Utilização de **WorkManager** para:

-   Agendar notificações futuras
-   Repetição automática de tarefas recorrentes

WorkManager garante execução mesmo após reinicialização do dispositivo.

------------------------------------------------------------------------

## 🧪 8. Estratégia de Testes

Testes unitários focam em:

-   UseCases
-   Regras de recorrência
-   Cálculo de próxima ocorrência
-   Comportamento de Snooze

ViewModels podem ser testadas com Mock de Repository.

------------------------------------------------------------------------

## 📂 9. Estrutura de Pastas

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

## 🎯 10. Justificativa das Decisões Técnicas

  Decisão              Justificativa
  -------------------- -----------------------------------
  MVVM                 Separação clara entre UI e lógica
  Clean Architecture   Escalabilidade e manutenção
  Hilt                 Redução de acoplamento
  Room                 Persistência simples e robusta
  WorkManager          Confiabilidade no agendamento
  Compose              Modernidade e produtividade

------------------------------------------------------------------------

## 🚀 11. Escalabilidade Futura

A arquitetura permite futuras expansões:

-   Sincronização em nuvem
-   Autenticação Google
-   Backup automático
-   Multi-dispositivo
-   Camada de API remota

Sem necessidade de reestruturação completa.

------------------------------------------------------------------------

## 📌 Conclusão

A arquitetura adotada no projeto **Lembra Fácil** segue padrões modernos
de mercado, garantindo organização, testabilidade e manutenção
facilitada.

Essa estrutura posiciona o projeto como um aplicativo desenvolvido com
práticas profissionais, adequado para portfólio técnico e evolução
contínua.

------------------------------------------------------------------------

## 👨‍💻 Autor

Maikel H. da Silva\
Curso: Análise e Desenvolvimento de Sistemas\
Disciplina: Programação para Dispositivos Móveis
