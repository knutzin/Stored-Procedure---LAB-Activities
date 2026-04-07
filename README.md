# 📊 Atividade Prática: Stored Procedures & Functions
**Disciplina:** Banco de Dados II  
**Instituição:** Pontifícia Universidade Católica de São Paulo (PUC-SP)  

---

## 📝 Descrição do Projeto
Este repositório contém a resolução do laboratório focado em **Lógica Procedural em Bancos de Dados Relacionais**. A atividade simula operações reais de um E-commerce, automatizando regras de negócio diretamente no servidor de banco de dados para garantir integridade e performance.

### Tecnologias Utilizadas
* **PostgreSQL:** RDBMS hospedado na plataforma [Neon.tech](https://neon.tech).
* **Python & Jupyter Notebook:** Ambiente para orquestração dos scripts.
* **ipython-sql:** Extensão para execução de comandos SQL via células de código.

---

## 🛠️ Estrutura de Dados
O sistema utiliza um esquema composto por 5 tabelas principais:
1.  **Customers:** Cadastro de clientes e saldo de pontos de fidelidade.
2.  **Products:** Catálogo com controle de estoque, categoria e validade.
3.  **Orders:** Registro mestre de pedidos.
4.  **Order_Items:** Detalhamento de itens, quantidades e preços unitários.
5.  **Audit_Logs:** Histórico de operações críticas e automações.

---

## 🚀 Implementações (10 Atividades)

O notebook cobre as seguintes funcionalidades:

1.  **Ajuste de Preços:** Procedure para atualização percentual em massa.
2.  **Descontos por Categoria:** Aplicação de promoções específicas com registro em log.
3.  **Processamento de Pedidos:** Automação completa de venda (Inserção + Baixa de Estoque).
4.  **Alerta de Estoque:** Monitoramento de produtos com menos de 10 unidades.
5.  **Cálculo de Preço Final (Function):** Função escalar que calcula impostos e descontos de fidelidade.
6.  **Top Selling Products:** Função que retorna o ranking de vendas em um período.
7.  **Customer LTV:** Cálculo do valor total gasto por um cliente ao longo do tempo.
8.  **Desconto por Validade:** Automação para reduzir preços de produtos próximos ao vencimento.
9.  **Limpeza de Logs:** Manutenção para remover registros de auditoria antigos.
10. **Relatório Diário:** Consolidação de vendas do dia e bonificação de clientes ativos.

---

## 🔧 Como Rodar o Projeto
1. Abra o arquivo `.ipynb` no **Google Colab**.
2. Configure o "Secret" `NEON_DB_URL` com sua string de conexão.
3. Execute a célula de **Setup** para criar e popular as tabelas.
4. Execute as definições de **Procedures** e **Functions**.

