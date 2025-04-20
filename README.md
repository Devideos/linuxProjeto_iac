# 🖥️ Script de Criação de Estrutura de Diretórios, Grupos e Usuários no Linux

Este projeto contém um script em **Shell Script (Bash)** desenvolvido para automatizar a criação de uma estrutura organizacional básica em sistemas Linux. É ideal para empresas ou ambientes educacionais que desejam gerenciar usuários e permissões de forma padronizada, organizada e segura.

---

## 🔧 O que o script faz?

✅ Cria diretórios:

- `/publico` – Acesso livre para todos os usuários.
- `/adm`, `/ven`, `/sec` – Diretórios restritos conforme o grupo de trabalho.

✅ Cria grupos de usuários:

- `GRP_ADM` – Administrativo  
- `GRP_VEN` – Vendas  
- `GRP_SEC` – Segurança

✅ Cria usuários e os adiciona aos respectivos grupos:

- Cada usuário recebe:
  - Diretório home
  - Shell Bash padrão
  - Senha padrão criptografada (`Senha123`)
  - Associação a um grupo específico

✅ Define permissões dos diretórios:

- `/adm`, `/ven`, `/sec` → acesso exclusivo para o root e membros do grupo correspondente (permissão 770)
- `/publico` → acesso total para todos os usuários (permissão 777)

---

## 👤 Usuários Criados

| Nome        | Grupo     |
|-------------|-----------|
| carlos      | GRP_ADM   |
| maria       | GRP_ADM   |
| joao        | GRP_ADM   |
| debora      | GRP_VEN   |
| sebastiana  | GRP_VEN   |
| roberto     | GRP_VEN   |
| josefina    | GRP_SEC   |
| amanda      | GRP_SEC   |
| rogerio     | GRP_SEC   |

---

## 🧰 Requisitos

- Sistema operacional Linux (testado no Ubuntu)
- Acesso root (superusuário)
- `openssl` instalado (para criptografar senha)

---

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/davidpereiradev/nome-do-repositorio.git
