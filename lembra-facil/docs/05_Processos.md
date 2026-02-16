# ⚙️ Setup do Repositório -- GitHub + Git (Windows)

## 📌 1. Objetivo

Este documento descreve o processo de criação, clonagem e organização do
repositório do projeto **Lembra Fácil**, utilizando GitHub e Git no
ambiente Windows.

O objetivo é garantir versionamento correto, organização local adequada
e boas práticas de desenvolvimento.

------------------------------------------------------------------------

## 🧱 2. Criação do Repositório no GitHub

### 2.1 Configuração Inicial

1.  Acessar https://github.com\
2.  Clicar em **New repository**\
3.  Configurar:

-   **Repository name:** `programacao-dispositivos-moveis`
-   **Visibility:** Public (recomendado para portfólio)
-   Marcar:
    -   ✅ Add README
    -   ✅ Add .gitignore → Android

4.  Clicar em **Create repository**

Resultado:

-   Repositório remoto criado
-   README.md inicial
-   .gitignore configurado para projetos Android

------------------------------------------------------------------------

## 💻 3. Clonagem do Repositório

### 3.1 Primeiro Clone

No terminal:

``` bash
git clone https://github.com/maikelhs/programacao-dispositivos-moveis
```

O Git cria automaticamente uma pasta com o nome do repositório dentro do
diretório atual.

Regra importante:

> O `git clone` cria a pasta do repositório dentro da pasta onde o
> terminal está posicionado.

------------------------------------------------------------------------

## 📂 4. Organização Recomendada no Windows

Criar pasta específica para projetos:

``` bash
mkdir C:\Projetos
cd C:\Projetos
```

Realizar clone dentro dessa pasta:

``` bash
git clone https://github.com/maikelhs/programacao-dispositivos-moveis
```

Estrutura recomendada:

C:`\Projetos`{=tex}`\programacao`{=tex}-dispositivos-moveis

------------------------------------------------------------------------

## 🔄 5. Repositório Local vs Remoto

### 📌 Repositório Local

Pasta no seu computador contendo o código.

### 📌 Repositório Remoto

Repositório hospedado no GitHub.

### Fluxo de sincronização

Enviar alterações:

``` bash
git push
```

Receber alterações:

``` bash
git pull
```

------------------------------------------------------------------------

## 🧠 6. Comandos Essenciais

Adicionar arquivos:

``` bash
git add .
```

Criar commit:

``` bash
git commit -m "mensagem descritiva"
```

Enviar para GitHub:

``` bash
git push
```

Atualizar repositório local:

``` bash
git pull
```

------------------------------------------------------------------------

## 📋 7. Boas Práticas

-   Manter apenas um clone local do repositório\
-   Trabalhar sempre dentro da pasta principal\
-   Nunca versionar arquivos de build\
-   Escrever commits claros e descritivos\
-   Utilizar padrão de commit vinculado às Issues

Exemplo:

``` bash
feat: implementar estrutura inicial do projeto (#1)
```

------------------------------------------------------------------------

## 🚀 8. Próximo Passo

Após o clone:

1.  Abrir o projeto no Android Studio\
2.  Criar o projeto Android dentro da pasta correta\
3.  Realizar primeiro commit estruturado

------------------------------------------------------------------------

## 📌 Conclusão

A configuração correta do repositório garante:

-   Versionamento seguro\
-   Organização adequada\
-   Histórico rastreável\
-   Base sólida para desenvolvimento profissional
