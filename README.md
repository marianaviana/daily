# 🌞 Daily: Frase do Dia

[![Daily Quote Workflow](https://github.com/marianaviana/daily/actions/workflows/daily-commit.yml/badge.svg)](https://github.com/marianaviana/daily/actions/workflows/daily-commit.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Todos os dias uma nova frase motivacional é adicionada automaticamente a este repositório, com muito carinho (e um pouco de JavaScript + GitHub Actions ✨).

> 💬 Ideal para começar o dia com inspiração — ou para mostrar que seu GitHub está sempre em movimento 😉

## 🚀 Como funciona?

Este repositório usa **GitHub Actions** para atualizar diariamente o arquivo `frase-do-dia.txt` com uma frase diferente, retirada de um arquivo `frases.json` contendo 365 mensagens motivacionais.

A atualização ocorre **todos os dias às 00:00 (horário de Brasília)**.

### 🔧 Tecnologias usadas

- [GitHub Actions](https://docs.github.com/en/actions) para automatizar o processo.
- Node.js para escolher e salvar a frase do dia.
- Git para versionar cada nova frase com um commit diário.

## 📁 Estrutura do repositório

```
daily/
├─ frases.json            ← lista de frases motivacionais
├─ frase-do-dia.txt       ← atualizado automaticamente
├─ index.html             ← página inicial do projeto
├─ style.css              ← estilo do projeto
├─ .github/               ← arquivos do github
│  └─ workflows/          ← scripts de automação com github actions
│     └─ daily-quote.yml ← github action diária
```

## ✨ Exemplo de uso

Você pode consumir a frase do dia diretamente via raw do GitHub:
```bash
https://raw.githubusercontent.com/SEU_USUARIO/SEU_REPOSITORIO/main/frase-do-dia.txt
```

> Basta trocar `SEU_USUARIO` e `SEU_REPOSITORIO` pelo seu nome de usuário e nome do repositório, ou [veja um exemplo aqui](https://raw.githubusercontent.com/marianaviana/daily/main/frase-do-dia.txt).

---

## 🔐 Configurando o repositório

Para que o commit automático funcione corretamente, você precisa configurar um **token de acesso pessoal (PAT)** como secret:

### 1. Gere um GitHub Personal Access Token (classic)

- Acesse: [https://github.com/settings/tokens](https://github.com/settings/tokens)
- Clique em **"Generate new token (classic)"**
- Selecione as seguintes permissões:
  - `repo` (acesso completo a repositórios privados/públicos)
  - `workflow` (caso deseje acionar outros workflows)
- Defina a validade desejada e clique em **"Generate token"**
- Copie o token gerado

### 2. Adicione o token como um Secret no repositório

- Vá até seu repositório no GitHub
- Clique em **Settings > Secrets and variables > Actions**
- Clique em **New repository secret**
- Nome: `MY_PERSONAL_TOKEN`
- Valor: (cole aqui o token gerado)

⚠️ A primeira execução do workflow precisa ser feita manualmente para iniciar o processo.

---

## 🧪 Executando manualmente

Se quiser testar a ação manualmente:

1. Acesse a aba **"Actions"** do repositório
2. Selecione o fluxo `update-daily-quote`
3. Clique em **"Run workflow"**

---

## ❤️ Contribuindo

Quer sugerir novas frases? Fique à vontade para abrir um PR ou issue!  
Compartilhar boas palavras também é um ato de generosidade. 🌻

## 📜 Licença

[MIT](LICENSE)

As frases são de domínio público ou criadas por autores anônimos.

---

**Feito com ☕ e inspiração por [@marianaviana](https://github.com/marianaviana)**