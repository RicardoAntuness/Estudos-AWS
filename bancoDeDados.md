# 🚀 Serviços de Banco de Dados na AWS

A AWS oferece uma variedade de serviços de banco de dados para diferentes necessidades, desde bancos relacionais até NoSQL, data warehouses e soluções especializadas.

---

## 📌 Bancos de Dados Relacionais (RDBMS)

### 🔹 Amazon RDS (Relational Database Service)
- Serviço gerenciado para **MySQL, PostgreSQL, MariaDB, Oracle, SQL Server e Amazon Aurora**.
- Recursos como backups automáticos, escalabilidade e alta disponibilidade.

### 🔹 Amazon Aurora
- Compatível com **MySQL e PostgreSQL**, mas otimizado para alta performance e disponibilidade.
- Disponível na versão **Aurora Serverless**, que escala automaticamente conforme a demanda.

---

## 📌 Bancos de Dados NoSQL

### 🔹 Amazon DynamoDB
- Banco **NoSQL key-value e document-oriented**, totalmente gerenciado e altamente escalável.
- Suporte a eventos em tempo real via **DynamoDB Streams**.

### 🔹 Amazon ElastiCache
- Serviço de cache em memória para **Redis e Memcached**, utilizado para acelerar aplicações web.

### 🔹 Amazon Keyspaces (for Apache Cassandra)
- Banco de dados gerenciado compatível com **Apache Cassandra**, ideal para aplicações distribuídas.

---

## 📌 Data Warehouses e Big Data

### 🔹 Amazon Redshift
- Data warehouse gerenciado, baseado em **PostgreSQL**, otimizado para análise de grandes volumes de dados.
- Integração nativa com **S3, Athena, Glue e outras ferramentas de análise**.

### 🔹 AWS Glue
- Serviço de **ETL (Extração, Transformação e Carga)** que facilita a preparação de dados para análise.

### 🔹 Amazon Athena
- Serviço **serverless** para consultas **SQL em dados armazenados no S3**, sem necessidade de provisionamento de infraestrutura.

---

## 📌 Bancos de Dados para Casos de Uso Específicos

### 🔹 Amazon DocumentDB (Compatível com MongoDB)
- Banco **NoSQL** para documentos, compatível com **MongoDB**, otimizado para aplicações escaláveis.

### 🔹 Amazon Timestream
- Banco de dados otimizado para **séries temporais**, ideal para IoT, métricas e monitoramento.

### 🔹 Amazon Neptune
- Banco de dados **gráfico**, usado para redes sociais, motores de recomendação e detecção de fraudes.

### 🔹 Amazon Quantum Ledger Database (QLDB)
- Banco de dados imutável para **registros de transações**, ideal para auditorias.

### 🔹 Amazon Managed Blockchain
- Serviço para criar e gerenciar redes **blockchain**, suportando **Hyperledger Fabric e Ethereum**.

---

## 📌 Ferramentas Complementares

- **AWS Database Migration Service (DMS)** → Migração de bancos de dados para AWS.
- **AWS Backup** → Backup automatizado para bancos de dados da AWS.
- **AWS Lake Formation** → Criação de data lakes escaláveis no S3.
