# ☁️ Laboratório - Criando Instância de Banco de Dados no Microsoft Azure

Repositório criado como parte do desafio da DIO para praticar a configuração de uma instância de banco de dados SQL no **Microsoft Azure**. Aqui estão os resumos, comandos e dicas que documentam toda a experiência.

---

## 🎯 Objetivos do Desafio

- Criar uma instância de banco de dados no Azure;
- Aprender a configurar conexões e regras de firewall;
- Documentar o processo técnico de forma clara;
- Compartilhar conhecimento por meio do GitHub.

---

## 🛠️ Etapas Realizadas

### 1. Acesso ao Portal do Azure
- Login com conta Microsoft;
- Navegação até a opção **Banco de Dados SQL**.

### 2. Criação da Instância de Banco de Dados
- Criação de novo grupo de recursos;
- Nome do banco de dados: `db-teste-dio`;
- Criação de um novo servidor lógico com:
  - Nome: `servidor-dio`
  - Região: Brasil Sul (ou a de sua escolha)
  - Autenticação: login/senha definidos
- Seleção de camada de desempenho: básica (para testes).

### 3. Configuração do Firewall
- Inclusão do IP local para acesso ao banco;
- Permissão de acesso de outros serviços do Azure (se necessário).

### 4. Teste de Conexão
- Uso do **Azure Data Studio**, **DBeaver**, ou **SQL Server Management Studio (SSMS)**;
- Teste da string de conexão fornecida no portal Azure;
- Execução de um comando simples (ex: `SELECT @@VERSION;`).

---

## 📷 Capturas de Tela

As imagens a seguir mostram o processo de criação e teste do banco:

- `/images/db-criacao.png` – Configuração inicial no portal.
- `/images/conexao-testada.png` – Conexão bem-sucedida com o banco.

---

## 📝 Dicas e Observações

- Sempre salve a string de conexão fornecida pelo Azure;
- Lembre-se de liberar o IP de quem vai acessar o banco (incluindo o seu);
- Para testes, use a camada **Gratuita ou Básica** para evitar custos;
- Use variáveis de ambiente ou arquivos `.env` para armazenar credenciais em projetos reais.

---

## 🚀 Tecnologias Utilizadas

- Microsoft Azure (SQL Database)
- Ferramentas de conexão (ex: DBeaver / Azure Data Studio)
- Git & GitHub

---

## 📚 Referências

- [Documentação Azure SQL Database](https://learn.microsoft.com/pt-br/azure/azure-sql/)
- Aulas do curso na DIO

---


