## Estudos AWS - UDEMY

- Freetier => Ambiente pra testes e desenvolvimento.
---
- Criar Alerta financeiro de tipo um limite de 10 dólares, e quando da os 10 dólares recebe aviso por e-mail. Usa-se o CloudWatch.
- Cloud Computing => Conexão de várias localizações, DataCenters.
- Vantagens do Cloud: 
    - Custo Reduzido, economiza em manutenções, compras de memórias, redes, discos, etc.
    - Escala Global, pagar menos e alcançar maior distância.
    - Velocidade, Performance, Agilidade: Iniciar serviços em minutos.
    - Produtividade, Segurança e Flexibilidade: Trabalho Remoto.
- Tipos de Cloud
    - IAAS: Alugar uma estrutura de um servidor, uma VM, Storage, parte física.
    - PAAS: Sistema Operacional, hospedagem de site.
    - SAAS: Usuário adquire acesso a uma aplicação, dropbox.
- Implementados:
    - Nuvem Publica: AWS, Azure, GPC
    - Nuvem Privada: Bancos, Governos, Equipes Financeiras.
    - Nuvem Hibrida: Meio Público e Meio Privado
- Suporte:
    - Developer
    - Business
    - Enterprise On-Ramp
    - Enterprise
---
- IAM: Usuários, Grupos, Funções e Políticas.
- Serve para organizar Usuários na AWS.

## AWS Identity and Access Management (IAM), MFA e AWS Organizations

### AWS Identity and Access Management (IAM)

O AWS Identity and Access Management (IAM) é um serviço da AWS que ajuda a controlar quem está autenticado e autorizado a usar os recursos da AWS.

### Principais Características

- **Controle Granular de Acesso**: Permite criar usuários, grupos, papéis e políticas de permissão para controlar o acesso de maneira detalhada.
- **Compartilhamento Seguro de Acesso**: Permite criar múltiplos usuários IAM, evitando o compartilhamento de credenciais de root.
- **Identidade Federada**: Possibilita autenticação via provedores de identidade, como SAML e redes corporativas.
- **Compatível com Multi-Fator Authentication (MFA)**: Adiciona uma camada extra de segurança na autenticação de usuários.
- **Integração com AWS Services**: Permite definir permissões para qualquer serviço AWS.
- **Auditoria com AWS CloudTrail**: Registra todas as ações de usuários e APIs IAM para fins de auditoria.
- **Gratuito**: Não há custo para usar o IAM; você paga apenas pelos serviços da AWS utilizados pelos usuários.

---

## Autenticação Multifator (MFA)

A Autenticação Multifator (MFA) é um método de segurança que exige múltiplos fatores de verificação para conceder acesso a um sistema.

### Benefícios e Características

- **Segurança Aprimorada**: Protege contra acessos não autorizados mesmo que um fator seja comprometido.
- **Diversos Métodos de Autenticação**: Suporta SMS, aplicativos de autenticação, tokens de hardware, biometria, entre outros.
- **Compatibilidade**: Funciona com diversos serviços e plataformas, como AWS, Google Cloud e Azure.
- **AWS MFA**: A AWS recomenda a ativação do MFA para proteger contas contra acessos indevidos.

---

## AWS Organizations

O AWS Organizations é um serviço da AWS que permite gerenciar múltiplas contas AWS a partir de um único local.

### Principais Características

- **Gerenciamento Centralizado de Contas**: Facilita o controle de contas e recursos de uma organização.
- **Controle de Acesso Hierárquico**: Permite agrupar contas em Unidades Organizacionais (OUs) para organização eficiente.
- **Políticas de Controle de Serviço (SCPs)**: Define regras de acesso uniformes para todas as contas.
- **Consolidação de Cobrança**: Simplifica a gestão de custos ao unificar as cobranças de múltiplas contas.
- **Automação**: Permite criar e gerenciar contas de forma automatizada via APIs e AWS CloudFormation.

---

- O IAM, MFA e AWS Organizations são ferramentas essenciais para a segurança e gerenciamento eficiente de recursos na AWS. Com o IAM, você controla acessos de maneira granular, enquanto a MFA adiciona uma camada extra de proteção. Já o AWS Organizations facilita

- A infraestrutura global da AWS é a base sobre a qual os serviços da AWS são construídos. Ela consiste em uma série de Regiões e Zonas de Disponibilidade espalhadas pelo mundo, projetadas para fornecer um serviço seguro, confiável e escalável.

- O Modelo de Responsabilidade Compartilhada da AWS é uma estrutura de governança que delineia a divisão de responsabilidades de segurança entre a Amazon Web Services (AWS) e o usuário (cliente). Essa divisão de responsabilidades permite que a AWS se concentre na segurança da infraestrutura de computação em nuvem, enquanto o usuário se concentra na segurança dos dados e recursos que colocam na nuvem.