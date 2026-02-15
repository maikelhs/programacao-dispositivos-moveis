
# 📱 Lembretes Simplificado

Aplicativo Android focado em auxiliar pessoas 60+ a gerenciar tarefas recorrentes de forma simples, intuitiva e acessível.

Projeto desenvolvido com arquitetura profissional utilizando Kotlin, Jetpack Compose e boas práticas de mercado.

---

## 🎯 Problema

Pessoas mais velhas frequentemente possuem múltiplas responsabilidades mensais (contas, compromissos, propriedades) e enfrentam dificuldade em utilizar aplicativos financeiros complexos.

Este app propõe uma solução minimalista, focada apenas em lembrar e confirmar tarefas.

---

## 🚀 Funcionalidades (MVP)

- Cadastro de tarefas recorrentes (mensal/semanal) e únicas
- Listagem de tarefas do dia
- Marcação como "Feito"
- Opção "Lembrar mais tarde"
- Geração automática da próxima ocorrência
- Persistência local com Room
- Notificações com WorkManager

---

## 🏗️ Arquitetura

O projeto segue arquitetura em camadas:

- MVVM
- Clean Architecture (Domain, Data, UI)
- Repository Pattern
- Injeção de Dependência com Hilt
- Coroutines + Flow

Estrutura de pastas:

```
core/  
data/  
domain/  
ui/
```


---

## 🛠️ Tecnologias Utilizadas

- Kotlin
- Jetpack Compose
- Material 3
- Room
- WorkManager
- Hilt
- Android Navigation Compose

---

## 📸 Screenshots

*(Adicionar imagens das telas aqui)*

---

## ⚙️ Como Executar

1. Clone o repositório
2. Abra no Android Studio (Giraffe ou superior)
3. Execute em dispositivo físico ou emulador

---

## 📈 Próximas Evoluções

- Sincronização entre dispositivos
- Login com Google
- Backup automático
- Compartilhamento familiar
- Melhorias de acessibilidade

---

## 👨‍💻 Autor

Desenvolvido por Maikel Holewa  
Curso: Análise e Desenvolvimento de Sistemas  
Disciplina: Programação para Dispositivos Móveis
