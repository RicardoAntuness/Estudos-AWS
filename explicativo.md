# 🚀 Introdução à AWS

## 📌 O que é a AWS?
A **AWS (Amazon Web Services)** é uma plataforma de serviços em nuvem que permite hospedar aplicações, armazenar dados e processar informações **pagando apenas pelo que usar**. 

---

## 🖥️ Computação e Servidores

- **Amazon EC2** → Servidores virtuais configuráveis.
- **Elastic Load Balancing (ELB)** → Distribui o tráfego entre servidores.
- **Auto Scaling** → Cria mais servidores automaticamente conforme a demanda.

💡 **Exemplo:** Se um site recebe muitos acessos, o Auto Scaling adiciona servidores para evitar lentidão.

---

## ⚡ Computação Sem Servidor (Serverless)

- **AWS Lambda** → Executa código sem precisar configurar servidores.
- **AWS Fargate** → Roda contêineres sem precisar gerenciar servidores.

💡 **Exemplo:** O AWS Lambda pode processar imagens sem precisar manter servidores ativos o tempo todo.

---

## 📦 Armazenamento e Bancos de Dados

- **Amazon S3** → Armazena arquivos e imagens.
- **Amazon EBS** → Armazena dados de servidores EC2.
- **Amazon RDS** → Banco de dados relacional (MySQL, PostgreSQL, etc.).
- **Amazon DynamoDB** → Banco de dados NoSQL escalável.
- **Amazon Redshift** → Para análise de grandes volumes de dados.

💡 **Exemplo:** O S3 funciona como um Google Drive para armazenar arquivos.

---

## ✉️ Mensagens e Comunicação entre Sistemas

- **Amazon SQS** → Cria filas de mensagens para processar tarefas.
- **Amazon SNS** → Envia notificações para usuários e sistemas.

💡 **Exemplo:** Um site de compras pode usar **SQS** para organizar pedidos e **SNS** para enviar e-mails de confirmação.

---

## 🔐 Segurança e Controle de Acesso

- **IAM (Identity and Access Management)** → Gerencia usuários e permissões.
- **AWS Organizations** → Gerencia várias contas AWS.
- **AWS Artifact** → Acessa relatórios de segurança.

💡 **Exemplo:** IAM pode restringir acesso a serviços específicos para funcionários de uma empresa.

---

## 💰 Modelos de Preços da AWS

1. **Sob demanda** → Paga apenas pelo uso.
2. **Instâncias Spot** → Mais baratas, mas podem ser encerradas pela AWS.
3. **Instâncias reservadas** → Mais barato para quem reserva por longo prazo.
4. **Savings Plans** → Descontos para quem se compromete com um uso contínuo.

💡 **Exemplo:** Se você usa servidores ocasionalmente, **sob demanda** é ideal. Se usa constantemente, um **Savings Plan** pode reduzir custos.

---

## 🌍 Infraestrutura Global da AWS
A AWS tem data centers espalhados pelo mundo. Se um falhar, outro assume automaticamente.

💡 **Exemplo:** Se uma cafeteria da sua cidade fechar, você pode ir a outra unidade e continuar tomando café. A AWS faz o mesmo com seus servidores.

