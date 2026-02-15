# 📱 Programação para Dispositivos Móveis  
## Setup do Repositório com GitHub + Git (Windows)

Este documento descreve, passo a passo, o processo de criação do repositório no GitHub e clonagem para o ambiente local no Windows.

---

# 🔹 1. Criação do Repositório no GitHub

1. Acessar https://github.com
2. Clicar em **New repository**
3. Configurar:

- **Repository name:** `programacao-dispositivos-moveis`
- **Description:** Projetos e experimentos desenvolvidos na disciplina de Programação para Dispositivos Móveis, utilizando Android Studio, Kotlin e Jetpack Compose.
- **Visibility:** `Public` (recomendado para portfólio)

4. Marcar:
   - ✅ Add README
   - ✅ Add .gitignore → Selecionar **Android**

5. (Opcional) Add License → Pode deixar sem por enquanto
6. Clicar em **Create repository**

Resultado:
- Repositório remoto criado
- Arquivo `README.md` criado
- Arquivo `.gitignore` configurado para Android

---

# 🔹 2. Primeiro Clone (Pasta do Usuário)

No Prompt de Comando, o diretório atual era:


Foi executado:

```bash
git clone https://github.com/maikelhs/programacao-dispositivos-moveis
```


Resultado:

Foi criada automaticamente a pasta:

```
C:\Users\Computador\programacao-dispositivos-moveis
```

📌 Regra importante:  
O `git clone` cria a pasta do repositório dentro do diretório atual do terminal.


---

# 🔹 3. Tentativa de Organização em C:\Projetos

Foi executado:

```cd C:\Projetos```

Erro exibido:

`O sistema não pode encontrar o caminho especificado.`

Motivo:  
A pasta `C:\Projetos` ainda não existia.


---

# 🔹 4. Criando a Pasta Correta para Organização

Criar a pasta:

`mkdir C:\Projetos`

Entrar na pasta:

`cd C:\Projetos`

---

# 🔹 5. Segundo Clone (Agora Organizado)

Com o terminal em:

`C:\Projetos>`

Executado novamente:

`git clone https://github.com/maikelhs/programacao-dispositivos-moveis`

Resultado:

Nova pasta criada:

`C:\Projetos\programacao-dispositivos-moveis`

---

# 🔹 6. Situação Atual

Existem duas cópias locais do mesmo repositório:

1️⃣ `C:\Users\Computador\programacao-dispositivos-moveis`  
2️⃣ `C:\Projetos\programacao-dispositivos-moveis`

⚠ Importante:  
São duas cópias independentes localmente.

Elas só sincronizam através do GitHub usando:

`git push git pull`

---

# 🔹 7. Organização Recomendada

Manter apenas uma cópia local para evitar confusão.

Recomendado manter:

`C:\Projetos\programacao-dispositivos-moveis`

Remover a cópia antiga:

`rmdir /s C:\Users\Computador\programacao-dispositivos-moveis`

Ou apagar manualmente pelo Explorador de Arquivos.

---

# 🔹 8. Conceitos Importantes

## 📌 Repositório Local

É a pasta no seu computador onde o projeto está salvo.

## 📌 Repositório Remoto

É o repositório hospedado no GitHub.

Fluxo de sincronização:

Enviar alterações para o GitHub:

`git push`

Baixar alterações do GitHub:

`git pull`

---

# 🔹 9. Comandos Essenciais Utilizados

Listar arquivos:

`dir`

Criar pasta:

`mkdir NomeDaPasta`

Entrar em pasta:

`cd Caminho`

Clonar repositório:

`git clone URL`

Remover pasta:

`rmdir /s NomeDaPasta`

---

# 🔹 10. Próximo Passo

1. Abrir `C:\Projetos\programacao-dispositivos-moveis` no Android Studio
    
2. Criar o projeto Android dentro dessa pasta
    
3. Realizar o primeiro commit:
    

`git add . git commit -m "Criação do projeto Android (Kotlin + Jetpack Compose)" git push`

---

# ✅ Conclusão

Repositório criado corretamente.  
.gitignore configurado.  
Clone organizado.  
Estrutura pronta para iniciar o desenvolvimento Android com versionamento profissional.

`---  Se você quiser, posso agora gerar também:  - 📌 Um README padrão definitivo para o projeto - 📌 Um modelo de commit profissional - 📌 Um guia de fluxo Git para estudo - 📌 Ou já partimos para criar o projeto Android dentro da pasta correta  Qual próximo passo você quer dar? 🚀`