# 🌞 Daily: Frase do Dia

Todos os dias uma nova frase motivacional é adicionada automaticamente a este repositório, com muito carinho (e um pouco de JavaScript + GitHub Actions ✨).

> 💬 Ideal para começar o dia com inspiração — ou para mostrar que seu GitHub está sempre em movimento 😉

## 🚀 Como funciona?

Este repositório usa **GitHub Actions** para atualizar diariamente o arquivo `frase-do-dia.txt` com uma frase diferente, retirada de um arquivo `frases.json` contendo 365 mensagens motivacionais.

A atualização ocorre **todos os dias às 00:01 (horário de Brasília)**.

### 🔧 Tecnologias usadas

- [GitHub Actions](https://docs.github.com/en/actions) para automatizar o processo.
- Node.js para escolher e salvar a frase do dia.
- Git para versionar cada nova frase com um commit diário.

## 📁 Estrutura do repositório

- 📁 frases.json           # Lista de frases motivacionais
- 📄 frase-do-dia.txt      # Frase atual do dia (atualizado automaticamente)
- 🔧 .github/workflows     # Scripts de automação com GitHub Actions

## ✨ Exemplo de uso

Você pode consumir a frase do dia diretamente via raw do GitHub:
https://raw.githubusercontent.com/SEU_USUARIO/SEU_REPOSITORIO/main/frase-do-dia.txt

> Basta trocar `SEU_USUARIO` e `SEU_REPOSITORIO` pelo seu nome de usuário e nome do repositório, ou [veja um exemplo aqui](https://raw.githubusercontent.com/mariviana/daily/main/frase-do-dia.txt).

---

## ❤️ Contribuindo

Quer sugerir novas frases? Fique à vontade para abrir um PR ou issue!  
Compartilhar boas palavras também é um ato de generosidade. 🌻

## 📜 Licença

Este projeto está sob a licença MIT.  
As frases são de domínio público ou criadas por autores anônimos.

---

**Feito com ☕ e inspiração por [@marianaviana](https://mariviana.dev/)**
