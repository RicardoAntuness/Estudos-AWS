- O Elastic Load Balancing é o serviço da AWS que distribui automaticamente o tráfego de entrada de aplicações entre vários recursos, como instâncias do Amazon EC2. 

- As filas do SQS são o local onde as mensagens ficam até que sejam processadas.  A AWS gerencia a infraestrutura para que a empresa hospede essas filas.  Elas são dimensionadas automaticamente, confiáveis e fáceis de configurar e usar.  O Amazon SNS é semelhante,  pois é usado para envio de mensagens para serviços, mas também pode enviar notificações para usuários finais.
- A AWS oferece diversas opções de computação, sem servidor.  Sem servidor significa que não é possível ver nem acessar a infraestrutura  ou as instâncias que hospedam a aplicação.
- O AWS Lambda é uma opção de computação sem servidor  O Lambda é um serviço pelo qual você pode fazer upload de códigos na função Lambda.
- O Lambda é projetado para executar o código em até 15 minutos,  portanto ele não serve para processos com longa duração, como deep learning.  Ele é mais adequado para processamento rápido como backend da web,  gerenciamento de solicitações ou serviço de processamento de relatórios  de despesas de back end, no qual cada invocação é concluída em menos de 15 minutos.
- O Docker é uma plataforma que usa virtualização de nível  de sistema operacional para entregar software em contêineres.  Um contêiner é um pacote para código no qual se empacota a aplicação,  os elementos dela, bem como quaisquer configurações de que ela precisa para ser executada.
- O Fargate é uma plataforma  de computação sem servidor para ECS ou EKS.
- O AWS Lambda(opens in a new tab) é um serviço que permite a execução de códigos sem a necessidade de provisionar ou gerenciar servidores. 
- Os contêineres são uma maneira comum de empacotar códigos, configurações e dependências da aplicação em um único objeto. Você também pode usar contêineres para processos e fluxos de trabalho nos quais há requisitos essenciais de segurança, confiabilidade e dimensionamento.
- O Amazon Elastic Container Service (Amazon ECS)(opens in a new tab) é um sistema de gerenciamento de contêineres altamente dimensionável e de alto desempenho que permite executar e dimensionar aplicações em contêineres na AWS. 
- O AWS Fargate(opens in a new tab) é um mecanismo de computação sem servidor para contêineres. Ele funciona com o Amazon ECS e o Amazon EKS. 
- Definimos a computação em nuvem como entrega de recursos de TI sob demanda  pela internet, como pagamento conforme o uso.  Isso significa que você solicita recursos de TI como computação,  rede, armazenamento, analytics ou outros tipos de recursos que são disponibilizados sob demanda.  Você não paga pelo recurso com antecedência.


Em vez disso, você faz o provisionamento e paga no final do mês.  A AWS oferece serviços em muitas categorias  que podem ser usados em conjunto para criação de soluções.  Até agora, abordamos apenas alguns serviços.  Você aprendeu sobre o Amazon EC2.  Com o EC2 é possível iniciar e encerrar servidores virtuais  chamados instâncias do EC2 de forma dinâmica.


Quando uma instância do EC2 é iniciada, é preciso escolher a família da instância.  A família da instância determina o hardware em que a instância deve ser executada.  Instâncias podem ser criadas para um propósito específico.  As categorias são de uso geral.  Otimizada para computação.  Otimizada para memória, de computação acelerada e otimizada para armazenamento.


É possível dimensionar instâncias do EC2 verticalmente, redimensionando a instância  ou aumentar a quantidade ou iniciar novas instâncias e adicioná-las ao grupo.  É possível aumentar a quantidade de forma automática com o Amazon EC2 Auto Scaling.  Depois de aumentar a quantidade de instâncias do EC2, é preciso distribuir o tráfego entre essas instâncias.


É aí que entra o Elastic Load Balancing.  Os modelos de preços de instâncias do EC2 são diferentes.  Pode ser sob demanda, que é mais flexível e não precisa de contrato,  preço de instâncias Spot para usar a capacidade ociosa de recursos com desconto,  Saving Plans ou instâncias reservadas, com celebração de contrato com a AWS para obtenção de desconto  quando você se compromete com um determinado nível de uso.


E o Savings Plans que se aplica ao AWS Lambda e ao AWS Fargate e às instâncias EC2.  Há também serviços de mensagens como o Amazon Simple Queue Service ou SQS.  Com esse serviço é possível desacoplar os componentes do sistema.  As mensagens ficam na fila até que sejam consumidas ou excluídas.


O Amazon Simple Notification Service ou SNS é usado para o envio de mensagens como emails,  mensagens de texto, notificações por push ou solicitações HTTP.  Quando uma mensagem é publicada, ela é enviada para todos esses assinantes.  Você também aprendeu que a AWS tem diferentes serviços de computação, não só servidores virtuais como o EC2.


Há serviços de contêiner como Amazon Elastic Container Service ou ECS,  e o Amazon Elastic Kubernetes Service ou EKS, que são ferramentas de orquestração de contêiner.  Você pode usar essas ferramentas com instâncias do EC2, mas não é preciso gerenciá-la se não quiser.


Você pode usar o AWS Fargate para que os contêineres sejam executados em uma plataforma de computação sem servidor.  Também há o AWS Lambda,  no qual é possível carregar o código e configurá-lo para ser executado com base em gatilhos.

Somente o período de execução do código é cobrado.  Sem contêineres, sem máquinas virtuais, apenas código e configuração.

- A resposta correta é Otimizada para computação.
As outras respostas estão incorretas porque:
    instâncias de uso geral equilibram os recursos de computação, memória e rede. Essa família de instância não seria a melhor escolha para a aplicação nesse cenário. As instâncias otimizadas para computação são mais adequadas para cargas de trabalho de processamento em lote do que as instâncias de uso geral.
    As instâncias otimizadas para memória são ideais para cargas de trabalho que processam grandes conjuntos de dados na memória, como bancos de dados de alto desempenho.
    As instâncias otimizadas para armazenamento foram projetadas para cargas de trabalho que exigem alto acesso sequencial de leitura e gravação a grandes conjuntos de dados no armazenamento local. A pergunta não especifica o tamanho dos dados que serão processados. O processamento em batch é o processamento de dados em grupos. Uma instância otimizada para computação é ideal para esse tipo de carga de trabalho, que se beneficiaria de um processador de alto desempenho.

- Para entender a infraestrutura global da AWS, pense na cafeteria. Se um evento como um desfile, uma inundação ou queda de energia afetar uma unidade, os clientes ainda poderão tomar café em outra unidade a apenas alguns quarteirões de distância.

- Exemplo simples

Imagine que você gosta de um café específico e sempre vai à mesma unidade perto de casa. Um dia, há um problema nesse local (como uma falha elétrica). Como há outras filiais próximas, você pode ir a uma delas e continuar tomando seu café normalmente.

Da mesma forma, se um data center da AWS tiver um problema, seus serviços continuam funcionando porque a AWS tem outros data centers que assumem a carga automaticamente. Isso garante confiabilidade e continuidade para os usuários. 🚀

- Com o AWS CloudFormation, você pode considerar sua infraestrutura como código. Isso significa que você pode criar um ambiente escrevendo linhas de código em vez de usar o console de gerenciamento da AWS para provisionar recursos individualmente.

- Um armazenamento de instância(opens in a new tab) é um meio temporário de armazenamento a nível de bloco para uma instância do Amazon EC2. Um armazenamento de instância é o armazenamento em disco fisicamente anexo ao computador host para uma instância do EC2 e, portanto, tem a mesma vida útil da instância. Quando a instância for terminada, você perderá todos os dados no armazenamento de instância.

- O Amazon Elastic Block Store (Amazon EBS)(opens in a new tab) é um serviço que fornece volumes de armazenamento a nível de bloco que você pode usar com instâncias do Amazon EC2. Se você interromper ou terminar uma instância do Amazon EC2, todos os dados no volume do EBS anexo permanecerão disponíveis.

- O Amazon Relational Database Service (Amazon RDS)(opens in a new tab) é um serviço que permite executar bancos de dados relacionais na nuvem AWS.

- O Amazon Relational Database Service (Amazon RDS)(opens in a new tab) é um serviço que permite executar bancos de dados relacionais na nuvem AWS.

- Em um banco de dados não relacional, você cria tabelas. Uma tabela é um lugar em que você pode armazenar e consultar dados.

- O Amazon DynamoDB(opens in a new tab) é um serviço de banco de dados de chave-valor. Ele oferece um desempenho de um dígito de milissegundo em qualquer scaling.

- O Amazon Redshift(opens in a new tab) é um serviço de data warehouse que você pode usar para análise de Big Data. Ele oferece a capacidade de coletar dados de muitas fontes além de ajudar a entender relações e tendências em todos os seus dados.

- O AWS Database Migration Service (AWS DMS)(opens in a new tab) permite migrar bancos de dados relacionais e não relacionais e outros tipos de armazenamentos de dados.

- Com o AWS DMS, você move dados entre bancos de dados de origem e de destino. Os bancos de dados de origem e de destino(opens in a new tab) podem ser do mesmo tipo ou de tipos diferentes. Durante a migração, o banco de dados de origem permanece operacional, reduzindo o tempo de inatividade em qualquer aplicativo que dependa do banco de dados. 

- Modelo de Responsabilidade compartilhada AWS fica responsável pelo DataCenter.
- Com o modelo de responsabilidade compartilhada  a AWS controla a segurança da nuvem e os clientes controlam a segurança na nuvem.

- Responsabilidade do cliente: 
    - Plataforma, aplicações, Identity and Access Management (IAM).
    - Configuração de sistemas operacionais, rede e firewall.
    - Criptografia de dados no lado do cliente, criptografia de dados no lado do servidor e proteção de tráfego de rede.

- Responsabilidade da Amazon Web Services (AWS) 	
    - Software: computação, armazenamento, banco de dados, rede
    - Hardware: Regiões, Zonas de Disponibilidade, locais de borda

- Um grupo do IAM é um conjunto de usuários do IAM. Quando você atribui uma política do IAM a um grupo, todos os usuários do grupo recebem permissões especificadas pela política.
- Uma política do IAM é um documento que concede ou nega permissões para serviços e recursos AWS.  
- Um usuário do IAM é uma identidade que você cria na AWS. Ele representa a pessoa ou o aplicativo que interage com os serviços e recursos AWS. Consiste em um nome e credenciais.
- Ao criar uma conta AWS pela primeira vez, você começa com uma identidade conhecida como usuário-raiz.


- Suponha que sua empresa tenha múltiplas contas AWS. Você pode usar o AWS Organizations(opens in a new tab) para consolidar e gerenciar múltiplas contas AWS em um local central.
- Quando você cria uma organização, o AWS Organizations cria automaticamente uma raiz, que é o contêiner primário para todas as contas da organização. 
- No AWS Organizations, você pode agrupar contas em unidades organizacionais (UO) para facilitar o gerenciamento de contas com requisitos de negócios ou segurança semelhantes. Ao aplicar uma política a uma UO, todas as contas na UO herdam automaticamente as permissões especificadas na política.  

- O AWS Artifact é um serviço que concede acesso sob demanda a relatórios de segurança e conformidade da AWS e a contratos on-line selecionados. O AWS Artifact consiste em duas seções principais: AWS Artifact Agreements e o AWS Artifact Reports.
- O centro de conformidade para o cliente contém recursos que ajudam você a saber mais sobre a conformidade da AWS. 
---
- O que acontece com os dados armazenados no Instance Store de uma instância do Amazon EC2 quando ela é encerrada?
    - Os dados são perdidos permanentemente
---
- Um ataque de negação de serviço (DoS) é uma tentativa deliberada de tornar um site ou aplicação indisponível para os usuários.
- O AWS Shield é um serviço que protege aplicações contra ataques DDoS. O AWS Shield oferece dois níveis de proteção: Standard e Advanced.
- O AWS Shield Standard protege automaticamente todos os clientes AWS sem nenhum custo. Ele protege seus recursos AWS contra os tipos de ataques DDoS mais comuns e frequentes. 
- O AWS Shield Advanced é um serviço pago que fornece diagnósticos detalhados de ataques e a capacidade de detectar e mitigar ataques elaborados de DDoS. 
- O AWS WAF é um firewall de aplicação web que permite monitorar solicitações de rede que entram em aplicações web. 
- O Amazon Inspector ajuda a melhorar a segurança e a conformidade das aplicações executando avaliações de segurança automatizadas. Ele verifica os aplicativos quanto a vulnerabilidades de segurança e desvios das práticas recomendadas de segurança, como acesso aberto a instâncias do Amazon EC2 e instalações de versões de software vulneráveis. 
- O Amazon GuardDuty(opens in a new tab) é um serviço que realiza detecção inteligente de ameaças para sua infraestrutura e seus recursos AWS. Ele identifica ameaças monitorando continuamente a atividade da rede e o comportamento da conta no seu ambiente AWS.
---
- O AWS Key Management Service (AWS KMS)(opens in a new tab) permite que você execute operações de criptografia usando chaves de criptografia. Uma chave de criptografia é uma cadeia aleatória de dígitos usada para bloquear (criptografar) e desbloquear (descriptografar) dados. Você pode usar o AWS KMS para criar, gerenciar e usar chaves de criptografia. Você também pode controlar o uso de chaves em uma ampla gama de serviços e em suas aplicações.
- Com o AWS KMS, você pode escolher os níveis específicos de controle de acesso necessários para suas chaves. Por exemplo, você pode especificar quais usuários e funções do IAM podem gerenciar chaves. Do mesmo modo, você pode desativar temporariamente as chaves para que não sejam mais usadas. Suas chaves nunca saem do AWS KMS e você está sempre no controle delas.
- O AWS WAF(opens in a new tab) é um firewall de aplicação web que permite monitorar solicitações de rede que entram em aplicações web. 
- O Amazon Inspector ajuda a melhorar a segurança e a conformidade das aplicações executando avaliações de segurança automatizadas. Ele verifica os aplicativos quanto a vulnerabilidades de segurança e desvios das práticas recomendadas de segurança, como acesso aberto a instâncias do Amazon EC2 e instalações de versões de software vulneráveis. 
- O Amazon GuardDuty(opens in a new tab) é um serviço que realiza detecção inteligente de ameaças para sua infraestrutura e seus recursos AWS. Ele identifica ameaças monitorando continuamente a atividade da rede e o comportamento da conta no seu ambiente AWS.
- O Amazon CloudWatch(opens in a new tab) é um serviço da web que permite monitorar e gerenciar várias métricas e configurar ações de alarme de acordo com os dados dessas métricas.
- Com o CloudWatch, você pode criar alarmes(opens in a new tab) que vão executar ações automaticamente se o valor da métrica ultrapassar ou for inferior a um limite predefinido. 
- O AWS CloudTrail(opens in a new tab) registra as chamadas de API realizadas na sua conta. As informações gravadas são identidade do chamador da API, hora da chamada da API, endereço IP de origem do chamador da API e muito mais. Você pode pensar no CloudTrail como uma “trilha” (ou um log de ações) que alguém criou.
- No CloudTrail, você também pode ativar o CloudTrail Insights(opens in a new tab). Esse recurso opcional permite que o CloudTrail detecte automaticamente atividades de API incomuns em sua conta AWS. 
- O AWS Trusted Advisor(opens in a new tab) é um serviço da web que inspeciona seu ambiente AWS e faz recomendações em tempo real de acordo com as práticas recomendadas da AWS.
- O AWS Well-Architected Framework(opens in a new tab) ajuda você a entender como projetar e operar sistemas confiáveis, seguros, eficientes e econômicos na nuvem AWS. Com ele, é possível avaliar de maneira consistente suas arquiteturas em relação às práticas recomendadas e aos princípios de projeto e a identificar áreas para melhorias.
    - Confiabilidade
---
- A eficiência de desempenho é a capacidade de usar recursos computacionais com eficiência para cumprir requisitos do sistema e manter essa eficiência à medida que a demanda muda e as tecnologias evoluem. 
- Confiabilidade é a capacidade de um sistema fazer o seguinte:
    - Recuperar-se de interrupções na infraestrutura ou no serviço
    - Adquirir dinamicamente recursos de computação para atender à demanda
    - Reduzir interrupções, como configurações incorretas ou problemas de rede transitórios
- O pilar de segurança inclui a capacidade de proteger informações, sistemas e ativos e, ao mesmo tempo, entregar valor comercial por meio de avaliações de risco e estratégias de mitigação. 
- Excelência operacional é a capacidade de executar e monitorar sistemas para entregar valor comercial e melhorar continuamente os processos e procedimentos de apoio.  
- Otimização de custos é a capacidade de executar sistemas para entregar valor comercial com o menor preço.
- Sustentabilidade é a capacidade de melhorar continuamente os impactos da sustentabilidade, reduzindo o consumo de energia e aumentando a eficiência em todos os componentes de uma carga de trabalho, maximizando os benefícios dos recursos provisionados e minimizando o total de recursos necessários.

- Os seis pilares do AWS Well-Architected Framework:
        Excelência operacional
        Segurança
        Confiabilidade
        Eficiência de desempenho
        Otimização de custos
        Sustentabilidade
- Seis vantagens da computação em nuvem:
        Trocar despesas iniciais por despesas variáveis.
        Benefícios das grandes economias de escala.
        Parar de adivinhar capacidade.
        Aumentar a velocidade e agilidade.
        Parar de gastar dinheiro com execução e manutenção de data centers.
        Ter alcance global em minutos.

- Com o nível gratuito da AWS, você começa a usar determinados serviços sem ter que se preocupar com o custo durante o período especificado. 
- No AWS Budgets(opens in a new tab), você pode criar orçamentos para planejar o uso do serviço, os custos de serviço e as reservas de instâncias.
- As informações do AWS Budgets são atualizadas três vezes por dia. Isso ajuda você a definir com precisão a proximidade entre seu uso e os valores orçados ou limites de nível gratuito da AWS.
- O AWS Cost Explorer é uma ferramenta que permite visualizar, interpretar e gerenciar seus custos e uso da AWS ao longo do tempo.
- O Basic Support é gratuito para todos os clientes da AWS. Inclui acesso a whitepapers, documentação e comunidades de suporte. Com o Basic Support, você também pode entrar em contato com a AWS para tratar de questões de cobrança e aumento do limite de serviço
- O AWS Marketplace(opens in a new tab) é um catálogo digital com milhares de ofertas de software de provedores independentes de software. Você pode usar o AWS Marketplace para encontrar, testar e comprar software que pode ser executado na AWS. 
- O AWS Marketplace oferece produtos em várias categorias, como Software de infraestrutura, DevOps, Produtos de dados, Serviços profissionais, Aplicações de negócios, Machine Learning, Indústrias e Internet das Coisas (IoT).
- No nível mais alto, o AWS Cloud Adoption Framework (AWS CAF)(opens in a new tab) organiza orientações em seis áreas de foco chamadas perspectivas. Cada perspectiva aborda responsabilidades distintas. O processo de planejamento ajuda as pessoas certas em toda a organização a se prepararem para as mudanças futuras.
---
- Migrações da AWS:
    - Redefinir hospedagem (também conhecido como “lift-and-shift”) envolve a movimentação de aplicações sem alterações. No cenário de uma grande migração legada, em que a empresa busca implementar a migração e dimensionar rapidamente para atender a um caso de negócio, a hospedagem da maioria das aplicações é redefinida. 

    - Redefinir plataforma (também conhecido como “lift, tinker and shift”) envolve fazer algumas otimizações na nuvem para obter um benefício tangível. A otimização é alcançada sem alterar a arquitetura central do aplicativo.

    - Refatoração (também conhecida como rearquitetura) envolve reimaginar como uma aplicação é arquitetada e desenvolvida usando recursos nativos da nuvem. A refatoração costuma ser orientada pela forte necessidade que a empresa tem de adicionar recursos, scaling ou desempenho que, de outra forma, seriam difíceis de obter no ambiente atual da aplicação.

    - Recomprar envolve a mudança de uma licença tradicional para um modelo de software como serviço. Por exemplo, uma empresa pode optar por implementar a estratégia de recomprar migrando de um sistema de gerenciamento de relacionamento com o cliente (CRM) para o Salesforce.com.

    - Reter consiste em manter as aplicações essenciais para a empresa no ambiente de origem. Isso pode incluir aplicativos que exigem refatoração importante antes de serem migrados ou trabalhos que podem ser adiados.

    - Retirar é o processo de remoção de aplicações que não são mais necessários.

- A AWS Snow Family(opens in a new tab) é uma coleção de dispositivos físicos para transporte físico de até exabytes de dados para dentro e para fora da AWS. 