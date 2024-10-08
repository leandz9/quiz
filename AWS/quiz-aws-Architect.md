####  Uma equipe de desenvolvimento de aplicativos está projetando um microsserviço que converterá imagens grandes em imagens menores e compactadas. Quando um usuário faz upload de uma imagem por meio da interface da Web, o microsserviço deve armazenar a imagem em um bucket do Amazon S3, processar e compactar a imagem com uma função do AWS Lambda e armazenar a imagem em sua forma compactada em um bucket diferente do S3.
### Um arquiteto de soluções precisa projetar uma solução que use componentes duráveis e sem monitoração de estado para processar as imagens automaticamente.
### Que combinação de ações atenderá a esses requisitos? (Escolha dois.)

* [X] Configure a função do Lambda para usar a fila do Amazon Simple Queue Service (Amazon SQS) como a origem da invocação. Quando a mensagem SQS for processada com êxito, exclua a mensagem na fila. (*)

* [X] Crie uma fila do Amazon Simple Queue Service (Amazon SQS). Configure o bucket do S3 para enviar uma notificação para a fila do SQS quando uma imagem for carregada no bucket do S3. (*)

### Uma empresa tem um fluxo de trabalho de ingestão de dados que consiste no seguinte:
### • Um tópico do Amazon Simple Notification Service (Amazon SNS) para notificações sobre novas entregas de dados
### • Uma função do AWS Lambda para processar os dados e registrar metadados
### A empresa observa que o fluxo de trabalho de ingestão falha ocasionalmente devido a problemas de conectividade de rede. Quando essa falha ocorre, a função do Lambda não ingere os dados correspondentes, a menos que a empresa execute manualmente o trabalho.
### Que combinação de ações um arquiteto de soluções deve tomar para garantir que a função do Lambda ingera todos os dados no futuro? (Escolha dois.)

* [X] Crie uma fila do Amazon Simple Queue Service (Amazon SQS) e inscreva-a no tópico SNS. (*)

* [X] Modifique a função do Lambda para ler de uma fila do Amazon Simple Queue Service (Amazon SQS). (*)

### Uma empresa realiza manutenção mensal em sua infraestrutura da AWS. Durante essas atividades de manutenção, a empresa precisa alternar as credenciais de seus bancos de dados do Amazon RDS for MySQL em várias regiões da AWS.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Armazene as credenciais como segredos no AWS Secrets Manager. Use a replicação secreta de várias regiões para as regiões necessárias. Configure o Gerenciador de Segredos para girar os segredos em uma agenda. (*)

### Uma empresa deseja executar seus aplicativos críticos em contêineres para atender aos requisitos de escalabilidade e disponibilidade. A empresa prefere focar na manutenção das aplicações críticas. A empresa não deseja ser responsável pelo provisionamento e gerenciamento da infraestrutura subjacente que executa a carga de trabalho em contêineres.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Use o Amazon Elastic Container Service (Amazon ECS) no AWS Fargate. (*)

### Uma empresa fornece um serviço VoIP (Voice over Internet Protocol) que usa conexões UDP. O serviço consiste em instâncias do Amazon EC2 executadas em um grupo de Auto Scaling. A empresa tem implantações em várias regiões da AWS.
### A empresa precisa encaminhar os usuários para a Região com menor latência. A empresa também precisa de failover automatizado entre regiões.
### Qual solução atenderá a esses requisitos?

* [X] Implante um Application Load Balancer (ALB) e um grupo de destino associado. Associe o grupo de destino ao grupo de Auto Scaling. Crie um registro ponderado do Amazon Route 53 que aponte para aliases para cada ALB. Implante uma distribuição do Amazon CloudFront que use o registro ponderado como origem. (*)

### Uma empresa está criando um aplicativo na Nuvem AWS. O aplicativo armazenará dados em buckets do Amazon S3 em duas regiões da AWS. A empresa deve usar uma chave gerenciada pelo cliente do AWS Key Management Service (AWS KMS) para criptografar todos os dados armazenados nos buckets do S3. Os dados em ambos os buckets do S3 devem ser criptografados e descriptografados com a mesma chave KMS. Os dados e a chave devem ser armazenados em cada uma das duas regiões.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Crie uma chave KMS multi-região gerenciada pelo cliente. Crie um bucket do S3 em cada região. Configure a replicação entre os buckets do S3. Configure o aplicativo para usar a chave KMS com criptografia do lado do cliente.(*)

### Uma empresa tem um aplicativo que fornece serviços de marketing para lojas. Os serviços são baseados em compras anteriores feitas pelos clientes da loja. As lojas carregam dados de transações para a empresa através de SFTP, e os dados são processados e analisados para gerar novas ofertas de marketing. Alguns dos arquivos podem exceder 200 GB de tamanho.
### Recentemente, a empresa descobriu que algumas das lojas carregaram arquivos que contêm informações de identificação pessoal (PII) que não deveriam ter sido incluídas. A empresa quer que os administradores sejam alertados se as PII forem compartilhadas novamente. A empresa também quer automatizar a remediação.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos com o menor esforço de desenvolvimento?

* [X] Use um bucket do Amazon S3 como um ponto de transferência seguro. Use o Amazon Macie para verificar os objetos no bucket. Se os objetos contiverem PII, use o Amazon Simple Notification Service (Amazon SNS) para disparar uma notificação aos administradores para remover os objetos que contêm PII. (*)

### Uma empresa hospeda um aplicativo em várias instâncias do Amazon EC2. O aplicativo processa mensagens de uma fila do Amazon SQS, grava em uma tabela do Amazon RDS e exclui a mensagem da fila. Registros duplicados ocasionais são encontrados na tabela RDS. A fila do SQS não contém mensagens duplicadas.
### O que um arquiteto de soluções deve fazer para garantir que as mensagens sejam processadas apenas uma vez?

* [X] Use a chamada da API ChangeMessageVisibility para aumentar o tempo limite de visibilidade. (*)

### Uma empresa migrou recentemente para a AWS e deseja implementar uma solução para proteger o tráfego que entra e sai da VPC de produção. A empresa tinha um servidor de inspeção em seu data center local. O servidor de inspeção executou operações específicas, como inspeção de fluxo de tráfego e filtragem de tráfego. A empresa quer ter as mesmas funcionalidades na Nuvem AWS.
### Qual solução atenderá a esses requisitos?

* [X] Use o AWS Network Firewall para criar as regras necessárias para inspeção de tráfego e filtragem de tráfego para a VPC de produção. (*)

### Uma empresa tem uma carga de trabalho de produção que é executada em 1.000 instâncias Linux do Amazon EC2. A carga de trabalho é alimentada por software de terceiros. A empresa precisa corrigir o software de terceiros em todas as instâncias do EC2 o mais rápido possível para corrigir uma vulnerabilidade crítica de segurança.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Agende uma janela de manutenção do AWS Systems Manager para aplicar o patch a todas as instâncias do EC2. (*)

### Uma empresa tem um aplicativo Web de três camadas implantado na AWS. Os servidores Web são implantados em uma sub-rede pública em uma VPC. Os servidores de aplicativos e servidores de banco de dados são implantados em sub-redes privadas na mesma VPC. A empresa implantou um dispositivo de firewall virtual de terceiros do AWS Marketplace em uma VPC de inspeção. O appliance é configurado com uma interface IP que pode aceitar pacotes IP.
### Um arquiteto de soluções precisa integrar o aplicativo Web com o dispositivo para inspecionar todo o tráfego para o aplicativo antes que o tráfego chegue ao servidor Web.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional? 

* [X] Implante um Balanceador de Carga de Gateway na VPC de inspeção. Crie um ponto de extremidade do Balanceador de Carga do Gateway para receber os pacotes de entrada e encaminhar os pacotes para o dispositivo. (*)

### Uma empresa executa sua infraestrutura na AWS e tem uma base registrada de 700.000 usuários para seu aplicativo de gerenciamento de documentos. A empresa pretende criar um produto que converta arquivos de .pdf grandes em arquivos de imagem .jpg. Os arquivos .pdf têm em média 5 MB de tamanho. A empresa precisa armazenar os arquivos originais e os arquivos convertidos. Um arquiteto de soluções deve projetar uma solução escalável para acomodar a demanda que crescerá rapidamente ao longo do tempo.
### Qual solução atende a esses requisitos de forma MAIS econômica?

* [X] Salve os arquivos .pdf no Amazon S3. Configure um evento PUT do S3 para invocar uma função do AWS Lambda para converter os arquivos para .jpg formato e armazená-los novamente no Amazon S3. (*)

### Uma empresa deseja melhorar sua capacidade de clonar grandes quantidades de dados de produção em um ambiente de teste na mesma região da AWS. Os dados são armazenados em instâncias do Amazon EC2 em volumes do Amazon Elastic Block Store (Amazon EBS). As modificações nos dados clonados não devem afetar o ambiente de produção. O software que acessa esses dados requer desempenho de E/S consistentemente alto.
### Um arquiteto de soluções precisa minimizar o tempo necessário para clonar os dados de produção no ambiente de teste.
### Qual solução atenderá a esses requisitos?

* [X] Tire snapshots do EBS dos volumes do EBS de produção. Ative o recurso de restauração rápida de snapshots do EBS nos snapshots do EBS. Restaure os snapshots em novos volumes do EBS. Anexe os novos volumes do EBS às instâncias do EC2 no ambiente de teste. (*)

### Um aplicativo é executado em uma instância do Amazon EC2 em uma VPC. O aplicativo processa logs armazenados em um bucket do Amazon S3. A instância do EC2 precisa acessar o bucket do S3 sem conectividade com a Internet.
### Qual solução fornecerá conectividade de rede privada ao Amazon S3?

* [X] Um. Crie um VPC endpoint de gateway para o bucket do S3. (*)

### Uma empresa executa um aplicativo de comércio eletrônico em instâncias do Amazon EC2 atrás de um Application Load Balancer. As instâncias são executadas em um grupo do Amazon EC2 Auto Scaling em várias zonas de disponibilidade. O grupo Auto Scaling é dimensionado com base nas métricas de utilização da CPU. O aplicativo de comércio eletrônico armazena os dados da transação em um banco de dados MySQL 8.0 hospedado em uma grande instância do EC2.
### O desempenho do banco de dados diminui rapidamente à medida que a carga do aplicativo aumenta. O aplicativo lida com mais solicitações de leitura do que transações de gravação. A empresa quer uma solução que dimensione automaticamente o banco de dados para atender à demanda de cargas de trabalho de leitura imprevisíveis, mantendo a alta disponibilidade.
### Qual solução atenderá a esses requisitos?

* [X] Use o Amazon Aurora com uma implantação Multi-AZ. Configure o Auto Scaling do Aurora com réplicas do Aurora. (*)

### Uma empresa executa um aplicativo de processamento de imagens altamente disponível em instâncias do Amazon EC2 em uma única VPC. As instâncias do EC2 são executadas dentro de várias sub-redes em várias zonas de disponibilidade. As instâncias do EC2 não se comunicam entre si. No entanto, as instâncias do EC2 fazem download de imagens do Amazon S3 e fazem upload de imagens para o Amazon S3 por meio de um único gateway NAT. A empresa está preocupada com as taxas de transferência de dados.
### Qual é a maneira MAIS econômica para a empresa evitar cobranças regionais de transferência de dados?

* [X] Implante um VPC endpoint de gateway para o Amazon S3. (*)

### Um hospital implantou recentemente uma API RESTful com o Amazon API Gateway e o AWS Lambda. O hospital usa o API Gateway e o Lambda para carregar relatórios em formato PDF e JPEG. O hospital precisa modificar o código Lambda para identificar informações de saúde protegidas (PHI) nos relatórios.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Use o Amazon Textract para extrair o texto dos relatórios. Use o Amazon Comprehend Medical para identificar a PHI a partir do texto extraído. (*)

### Uma empresa está criando um aplicativo web de comércio eletrônico na AWS. O aplicativo envia informações sobre novos pedidos para uma API REST do Amazon API Gateway para processar. A empresa quer garantir que os pedidos sejam processados na ordem em que são recebidos.
### Qual solução atenderá a esses requisitos?

* [X] Use uma integração do API Gateway para enviar uma mensagem para uma fila FIFO do Amazon Simple Queue Service (Amazon SQS) quando o aplicativo receber um pedido. Configure a fila FIFO do SQS para invocar uma função do AWS Lambda para processamento. (*)

### Uma empresa mantém um repositório pesquisável de itens em seu site. Os dados são armazenados em uma tabela de banco de dados do Amazon RDS for MySQL que contém mais de 10 milhões de linhas. O banco de dados tem 2 TB de armazenamento SSD de uso geral. Há milhões de atualizações contra esses dados todos os dias através do site da empresa.
### A empresa notou que algumas operações de inserção estão levando 10 segundos ou mais. A empresa determinou que o desempenho do armazenamento de banco de dados é o problema.
### Qual solução resolve esse problema de desempenho?

* [X] Altere o tipo de armazenamento para SSD de IOPS provisionadas. (*)

### O site de uma empresa usa um armazenamento de instâncias do Amazon EC2 para seu catálogo de itens. A empresa quer garantir que o catálogo esteja altamente disponível e que o catálogo seja armazenado em um local durável.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Mova o catálogo para um sistema de arquivos do Amazon Elastic File System (Amazon EFS). (*)

### Uma empresa precisa de capacidade garantida do Amazon EC2 em três zonas de disponibilidade específicas em uma região específica da AWS para um próximo evento que durará 1 semana.
### O que a empresa deve fazer para garantir a capacidade EC2?

* [X] Crie uma Reserva de Capacidade sob Demanda que especifique a Região e as três Zonas de Disponibilidade necessárias. (*)

### Uma empresa possui um aplicativo que gera um grande número de arquivos, cada um com aproximadamente 5 MB de tamanho. Os arquivos são armazenados no Amazon S3. A política da empresa exige que os arquivos sejam armazenados por 4 anos antes de poderem ser excluídos. A acessibilidade imediata é sempre necessária, pois os arquivos contêm dados críticos de negócios que não são fáceis de reproduzir. Os arquivos são frequentemente acessados nos primeiros 30 dias da criação do objeto, mas são raramente acessados após os primeiros 30 dias.
### Qual solução de armazenamento é MAIS econômica?

* [X] Crie uma política de ciclo de vida do bucket do S3 para mover arquivos do S3 Standard para o S3 Standard-Infrequent Access (S3 Standard-IA) 30 dias após a criação do objeto. Exclua os arquivos 4 anos após a criação do objeto. (*)

### Uma empresa de comércio eletrônico quer lançar um site de um negócio por dia na AWS. Cada dia contará com exatamente um produto à venda por um período de 24 horas. A empresa quer ser capaz de lidar com milhões de solicitações a cada hora com latência de milissegundos durante os horários de pico.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Use um bucket do Amazon S3 para hospedar o conteúdo estático do site, implante uma distribuição do Amazon CloudFront, defina o bucket do S3 como origem e use as funções do Amazon API Gateway e do AWS Lambda para as APIs de back-end. Armazene os dados no Amazon DynamoDB. (*)

### Uma empresa executa um aplicativo web de mercado on-line na AWS. O aplicativo atende centenas de milhares de usuários durante os horários de pico. A empresa precisa de uma solução escalável e quase em tempo real para compartilhar os detalhes de milhões de transações financeiras com vários outros aplicativos internos. As transações também precisam ser processadas para remover dados confidenciais antes de serem armazenadas em um banco de dados de documentos para recuperação de baixa latência.
### O que um arquiteto de soluções deve recomendar para atender a esses requisitos?

* [X] Transmita os dados de transações para o Amazon Kinesis Data Streams. Use a integração do AWS Lambda para remover dados confidenciais de cada transação e, em seguida, armazene os dados de transações no Amazon DynamoDB. Outros aplicativos podem consumir os dados de transações fora do fluxo de dados do Kinesis. (*)

### Uma empresa tem mais de 5 TB de dados de arquivos em servidores de arquivos do Windows que são executados no local. Usuários e aplicativos interagem com os dados todos os dias.
### A empresa está transferindo suas cargas de trabalho do Windows para a AWS. À medida que a empresa continua esse processo, ela exige acesso à AWS e ao armazenamento de arquivos local com latência mínima. A empresa precisa de uma solução que minimize a sobrecarga operacional e não exija alterações significativas nos padrões de acesso a arquivos existentes. A empresa usa uma conexão VPN Site a Site da AWS para conectividade com a AWS.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Implante e configure o Amazon FSx for Windows File Server na AWS. Implante e configure um Amazon FSx File Gateway no local. Mova os dados do arquivo local para o FSx File Gateway. Configure as cargas de trabalho na nuvem para usar o FSx for Windows File Server na AWS. Configure as cargas de trabalho locais para usar o FSx File Gateway. (*)

### Uma empresa lançou recentemente uma variedade de novas cargas de trabalho em instâncias do Amazon EC2 em sua conta da AWS. A empresa precisa criar uma estratégia para acessar e administrar as instâncias de forma remota e segura. A empresa precisa implementar um processo repetível que funcione com serviços nativos da AWS e siga o AWS Well-Architected Framework.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Anexe a função apropriada do IAM a cada instância existente e nova. Use o AWS Systems Manager Session Manager para estabelecer uma sessão SSH remota. (*)

### Uma empresa hospeda um data lake na AWS. O data lake consiste em dados no Amazon S3 e no Amazon RDS for PostgreSQL. A empresa precisa de uma solução de relatórios que forneça visualização de dados e inclua todas as fontes de dados dentro do data lake. Somente a equipe de gestão da empresa deve ter acesso total a todas as visualizações. O restante da empresa deve ter acesso limitado.
### Qual solução atenderá a esses requisitos?

* [X] Crie uma análise no Amazon QuickSight. Conecte todas as fontes de dados e crie novos conjuntos de dados. Publique painéis para visualizar os dados. Compartilhe os painéis com os usuários e grupos apropriados. (*)

### Uma empresa está se preparando para lançar um aplicativo Web voltado para o público na Nuvem AWS. A arquitetura consiste em instâncias do Amazon EC2 dentro de uma VPC atrás de um ELB (Elastic Load Balancer). Um serviço de terceiros é usado para o DNS. O arquiteto de soluções da empresa deve recomendar uma solução para detectar e proteger contra ataques DDoS em grande escala.
### Qual solução atende a esses requisitos?

* [X] Habilite o AWS Shield Advanced e atribua o ELB a ele. (*)

### Uma empresa está desenvolvendo um aplicativo Web de duas camadas na AWS. Os desenvolvedores da empresa implantaram o aplicativo em uma instância do Amazon EC2 que se conecta diretamente a um banco de dados back-end do Amazon RDS. A empresa não deve codificar credenciais de banco de dados no aplicativo. A empresa também deve implementar uma solução para girar automaticamente as credenciais do banco de dados regularmente.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Armazene as credenciais do banco de dados como segredo no AWS Secrets Manager. Ative a rotação automática para o segredo. Anexe a permissão necessária à função EC2 para conceder acesso ao segredo. (*)

### Uma empresa usa o NFS para armazenar arquivos de vídeo grandes no armazenamento conectado à rede local. Cada arquivo de vídeo varia em tamanho de 1 MB a 500 GB. O armazenamento total é de 70 TB e não está mais crescendo. A empresa decide migrar os arquivos de vídeo para o Amazon S3. A empresa deve migrar os arquivos de vídeo o mais rápido possível, usando a menor largura de banda de rede possível.
### Qual solução atenderá a esses requisitos?

* [X] Crie um trabalho do AWS Snowball Edge. Receba um dispositivo Snowball Edge no local. Use o cliente Snowball Edge para transferir dados para o dispositivo. Retorne o dispositivo para que a AWS possa importar os dados para o Amazon S3. (*)

### Uma empresa está implementando um novo aplicativo de negócios. O aplicativo é executado em duas instâncias do Amazon EC2 e usa um bucket do Amazon S3 para armazenamento de documentos. Um arquiteto de soluções precisa garantir que as instâncias do EC2 possam acessar o bucket do S3.
### O que o arquiteto de soluções deve fazer para atender a esse requisito?

* [X] Crie uma função do IAM que conceda acesso ao bucket do S3. Anexe a função às instâncias do EC2. (*)

### Uma empresa tem um aplicativo local que gera uma grande quantidade de dados sensíveis ao tempo armazenados em backup no Amazon S3. O aplicativo cresceu e há reclamações de usuários sobre limitações de banda da internet. Um arquiteto de soluções precisa projetar uma solução de longo prazo que permita backups oportunos para o Amazon S3 e com impacto mínimo na conectividade com a Internet para usuários internos.
### Qual solução atende a esses requisitos?

* [X] Estabeleça uma nova conexão do AWS Direct Connect e direcione o tráfego de backup por meio dessa nova conexão. (*)

### Uma equipe de desenvolvimento executa testes mensais com uso intensivo de recursos em sua instância de banco de dados de uso geral do Amazon RDS for MySQL com o Performance Insights habilitado. O teste dura 48 horas uma vez por mês e é o único processo que usa o banco de dados. A equipe deseja reduzir o custo de execução dos testes sem reduzir os atributos de computação e memória da instância de banco de dados.
### Qual solução atende a esses requisitos de forma MAIS econômica?

* [X] Crie um sanpshot quando os testes forem concluídos. Encerre a instância de banco de dados e restaure o snapshot quando necessário. (*)

### Uma empresa está hospedando um site estático no Amazon S3 e está usando o Amazon Route 53 para DNS. O site está experimentando um aumento da demanda de todo o mundo. A empresa deve diminuir a latência para os usuários que acessam o site.
### Qual solução atende a esses requisitos de forma MAIS econômica?

* [X] Adicione uma distribuição do Amazon CloudFront na frente do bucket do S3. Edite as entradas do Route 53 para apontar para a distribuição do CloudFront. (*)

### Uma empresa que hospeda seu aplicativo web na AWS deseja garantir todas as instâncias do Amazon EC2. Instâncias de banco de dados do Amazon RDS. e os clusters do Amazon Redshift são configurados com tags. A empresa quer minimizar o esforço de configuração e operação dessa verificação.
### O que um arquiteto de soluções deve fazer para conseguir isso?

* [X] Use as regras do AWS Config para definir e detectar recursos que não estão marcados corretamente. (*)

### Uma empresa está migrando um aplicativo distribuído para a AWS. O aplicativo atende cargas de trabalho variáveis. A plataforma herdada consiste em um servidor primário que coordena trabalhos em vários nós de computação. A empresa quer modernizar o aplicativo com uma solução que maximize a resiliência e escalabilidade.
### Como um arquiteto de soluções deve projetar a arquitetura para atender a esses requisitos?

* [X] Configure uma fila do Amazon Simple Queue Service (Amazon SQS) como um destino para os trabalhos. Implemente os nós de computação com instâncias do Amazon EC2 gerenciadas em um grupo de Auto Scaling. Configure o EC2 Auto Scaling com base no tamanho da fila. (*)

### Uma empresa registrou seu nome de domínio no Amazon Route 53. A empresa usa o Amazon API Gateway na região ca-central-1 como uma interface pública para suas APIs de microsserviço de back-end. Serviços de terceiros consomem as APIs com segurança. A empresa deseja projetar sua URL de API Gateway com o nome de domínio da empresa e o certificado correspondente para que os serviços de terceiros possam usar HTTPS.
### Qual solução atenderá a esses requisitos?

* [X] Crie um ponto de extremidade do Gateway de API Regional. Associe o ponto de extremidade do API Gateway ao nome de domínio da empresa. Importe o certificado público associado ao nome de domínio da empresa para o AWS Certificate Manager (ACM) na mesma região. Anexe o certificado ao ponto de extremidade do API Gateway. Configure o Route 53 para rotear o tráfego para o ponto de extremidade do API Gateway. (*)

### Uma empresa está armazenando arquivos de backup usando o armazenamento do Amazon S3 Standard. Os arquivos são acessados com frequência por 1 mês. No entanto, os arquivos não são acessados após 1 mês. A empresa deve manter os arquivos por tempo indeterminado.
### Qual solução de armazenamento atenderá a esses requisitos de forma MAIS econômica?

* [X] Crie uma configuração do ciclo de vida do S3 para fazer a transição de objetos do S3 Standard para o S3 Glacier Deep Archive após 1 mês. (*)

### Um arquiteto de soluções está desenvolvendo uma arquitetura de VPC que inclui várias sub-redes. A arquitetura hospedará aplicativos que usam instâncias do Amazon EC2 e instâncias de banco de dados do Amazon RDS. A arquitetura consiste em seis sub-redes em duas zonas de disponibilidade. Cada zona de disponibilidade inclui uma sub-rede pública, uma sub-rede privada e uma sub-rede dedicada para bancos de dados. Somente instâncias do EC2 executadas nas sub-redes privadas podem ter acesso aos bancos de dados do RDS.
### Qual solução atenderá a esses requisitos?

* [X] Crie um grupo de segurança que permita o tráfego de entrada do grupo de segurança atribuído a instâncias nas sub-redes privadas. Anexe o security group às instâncias de banco de dados. (*)

### Uma empresa tem um bucket do Amazon S3 que contém dados críticos. A empresa deve proteger os dados contra exclusão acidental.
### Que combinação de etapas um arquiteto de soluções deve seguir para atender a esses requisitos? (Escolha dois.)

* [X] Habilite MFA Delete no bucket do S3. (*)

* [X] Habilite o controle de versão no bucket do S3. (*)

### Uma empresa está migrando aplicativos para a AWS. Os aplicativos são implantados em contas diferentes. A empresa gerencia as contas usando central do AWS Organizations. A equipe de segurança da empresa precisa de uma solução de logon único (SSO) em todas as contas da empresa. A empresa deve continuar gerenciando os usuários e grupos em seu Microsoft Active Directory autogerenciado local.
### Qual solução atenderá a esses requisitos?

* [X] Habilite o AWS Single Sign-On (AWS SSO) no console do AWS SSO. Crie uma relação de confiança de floresta unidirecional ou uma confiança de domínio unidirecional para conectar o Microsoft Active Directory autogerenciado da empresa ao AWS SSO usando o AWS Directory Service for Microsoft Active Director. (*)

### Uma equipe de desenvolvimento precisa hospedar um site que será acessado por outras equipes. O conteúdo do site consiste em HTML, CSS, JavaScript do lado do cliente e imagens.
### Qual método é o MAIS econômico para hospedar o site?

* [X] Crie um bucket do Amazon S3 e hospede o site lá. (*)

### Uma empresa está executando um servidor de arquivos SMB em seu data center. O servidor de arquivos armazena arquivos grandes acessados com frequência nos primeiros dias após a criação dos arquivos. Após 7 dias os arquivos são raramente acessados.
### O tamanho total dos dados está aumentando e está próximo da capacidade total de armazenamento da empresa. Um arquiteto de soluções deve aumentar o espaço de armazenamento disponível da empresa sem perder o acesso de baixa latência aos arquivos acessados mais recentemente. O arquiteto de soluções também deve fornecer gerenciamento do ciclo de vida dos arquivos para evitar problemas futuros de armazenamento.
### Qual solução atenderá a esses requisitos?

* [X] Crie um Amazon S3 File Gateway para estender o espaço de armazenamento da empresa. Crie uma política de ciclo de vida do S3 para fazer a transição dos dados para o S3 Glacier Deep Archive após 7 dias. (*)

### Uma empresa está hospedando um aplicativo Web na AWS usando uma única instância do Amazon EC2 que armazena documentos carregados pelo usuário em um volume do Amazon EBS. Para melhor escalabilidade e disponibilidade, a empresa duplicou a arquitetura e criou uma segunda instância do EC2 e um volume do EBS em outra zona de disponibilidade, colocando ambos atrás de um Application Load Balancer. Após concluir essa alteração, os usuários relataram que, cada vez que atualizavam o site, podiam ver um subconjunto de seus documentos ou outro, mas nunca todos os documentos ao mesmo tempo.
### O que um arquiteto de soluções deve propor para garantir que os usuários vejam todos os seus documentos de uma só vez?

* [X] Copie os dados de ambos os volumes do EBS para o Amazon EFS. Modificar o aplicativo para salvar novos documentos no Amazon EFS. (*)

### Uma empresa executa várias cargas de trabalho do Windows na AWS. Os funcionários da empresa usam compartilhamentos de arquivos do Windows hospedados em duas instâncias do Amazon EC2. Os compartilhamentos de arquivos sincronizam dados entre si e mantêm cópias duplicadas. A empresa quer uma solução de armazenamento altamente disponível e durável que preserve como os usuários acessam os arquivos atualmente.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Estenda o ambiente de compartilhamento de arquivos para o Amazon FSx for Windows File Server com uma configuração Multi-AZ. Migre todos os dados para o FSx para Windows File Server. (*)

### Uma empresa está desenvolvendo um aplicativo que fornece estatísticas de envio de pedidos para recuperação por uma API REST. A empresa quer extrair as estatísticas de envio, organizar os dados em um formato HTML fácil de ler e enviar o relatório para vários endereços de e-mail ao mesmo tempo todas as manhãs.
### Que combinação de etapas um arquiteto de soluções deve seguir para atender a esses requisitos? (Escolha dois.)

* [X] Crie um evento agendado do Amazon EventBridge (Amazon CloudWatch Events) que invoque uma função do AWS Lambda para consultar os dados na API do aplicativo. (*)

* [X] Use o Amazon Simple Email Service (Amazon SES) para formatar os dados e enviar o relatório por e-mail. (*)

### Uma empresa está projetando um aplicativo. O aplicativo usa uma função do AWS Lambda para receber informações por meio do Amazon API Gateway e armazená-las em um banco de dados do Amazon Aurora PostgreSQL.
### Durante a fase de prova de conceito, a empresa tem que aumentar significativamente as cotas do Lambda para lidar com os altos volumes de dados que a empresa precisa carregar no banco de dados. Um arquiteto de soluções deve recomendar um novo design para melhorar a escalabilidade e minimizar o esforço de configuração.
### Qual solução atenderá a esses requisitos?

* [X] Configure duas funções do Lambda. Configure uma função para receber as informações. Configure a outra função para carregar as informações no banco de dados. Integre as funções do Lambda usando uma fila do Amazon Simple Queue Service (Amazon SQS). (*)

### Uma empresa global hospeda seu aplicativo Web em instâncias do Amazon EC2 atrás de um Application Load Balancer (ALB). A aplicação web tem dados estáticos e dados dinâmicos. A empresa armazena seus dados estáticos em um bucket do Amazon S3. A empresa quer melhorar o desempenho e reduzir a latência para os dados estáticos e dinâmicos. A empresa está usando seu próprio nome de domínio registrado no Amazon Route 53.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Crie uma distribuição do Amazon CloudFront que tenha o bucket do S3 e o ALB como origens. Configure o Route 53 para rotear o tráfego para a distribuição do CloudFront. (*)

### Uma empresa está lançando um novo aplicativo e exibirá métricas de aplicativos em um painel do Amazon CloudWatch. O gerente de produto da empresa precisa acessar esse painel periodicamente. O gerente de produto não tem uma conta da AWS. Um arquiteto de soluções deve fornecer acesso ao gerente de produto seguindo o princípio de privilégio mínimo.
### Qual solução atenderá a esses requisitos?

* [X] Compartilhe o painel no console do CloudWatch. Insira o endereço de e-mail do gerente de produto e conclua as etapas de compartilhamento. Forneça um link compartilhável para o painel para o gerente de produto. (*)

### Uma empresa tem um aplicativo executado em instâncias do Amazon EC2 e usa um banco de dados do Amazon Aurora. As instâncias do EC2 se conectam ao banco de dados usando nomes de usuário e senhas armazenados localmente em um arquivo. A empresa quer minimizar a sobrecarga operacional do gerenciamento de credenciais.
### O que um arquiteto de soluções deve fazer para atingir esse objetivo?

* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)

### Uma empresa tem milhares de dispositivos de borda que, coletivamente, geram 1 TB de alertas de status por dia. Cada alerta tem aproximadamente 2 KB de tamanho. Um arquiteto de soluções precisa implementar uma solução para ingerir e armazenar os alertas para análises futuras.
### A empresa quer uma solução altamente disponível. No entanto, a empresa precisa minimizar custos e não quer gerenciar infraestrutura adicional. Além disso, a empresa quer manter 14 dias de dados disponíveis para análise imediata e arquivar quaisquer dados com mais de 14 dias.
### Qual é a solução operacionalmente mais eficiente que atende a esses requisitos?

* [X] Crie um fluxo de entrega do Amazon Kinesis Data Firehose para ingerir os alertas. Configure o fluxo do Kinesis Data Firehose para entregar os alertas a um bucket do Amazon S3. Configure uma configuração do ciclo de vida do S3 para fazer a transição de dados para o Amazon S3 Glacier após 14 dias. (*)

### Uma empresa está implantando um novo aplicativo Web público na AWS. O aplicativo será executado atrás de um Application Load Balancer (ALB). O aplicativo precisa ser criptografado na borda com um certificado SSL/TLS emitido por uma autoridade de certificação (CA) externa. O certificado deve ser alternado a cada ano antes que o certificado expire.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Use o AWS Certificate Manager (ACM) para importar um certificado SSL/TLS. Aplique o certificado ao ALB. Use o Amazon EventBridge (Amazon CloudWatch Events) para enviar uma notificação quando o certificado estiver perto da expiração. Gire o certificado manualmente. (*)

### Uma empresa precisa revisar sua implantação na Nuvem AWS para garantir que seus buckets do Amazon S3 não tenham alterações de configuração não autorizadas.
### O que um arquiteto de soluções deve fazer para atingir esse objetivo?

* [X] Ative o AWS Config com as regras apropriadas. (*)

### Uma empresa tem um aplicativo que ingere mensagens recebidas. Dezenas de outros aplicativos e microsserviços consomem rapidamente essas mensagens. O número de mensagens varia drasticamente e às vezes aumenta repentinamente para 100.000 a cada segundo. A empresa quer desacoplar a solução e aumentar a escalabilidade.
### Qual solução atende a esses requisitos?

* [X] Publique as mensagens em um tópico do Amazon Simple Notification Service (Amazon SNS) com várias assinaturas do Amazon Simple Queue Service (Amazon SQS). Configure os aplicativos de consumidor para processar as mensagens das filas. (*)

### Uma empresa armazena arquivos de transcrição de chamadas mensalmente. Os usuários acessam os arquivos aleatoriamente dentro de 1 ano após a chamada, mas os usuários acessam os arquivos raramente após 1 ano. A empresa quer otimizar sua solução, dando aos usuários a capacidade de consultar e recuperar arquivos com menos de 1 ano o mais rápido possível. Um atraso na recuperação de arquivos mais antigos é aceitável.
### Qual solução atenderá a esses requisitos de forma MAIS econômica?

* [X] Armazene arquivos individuais no Amazon S3 Intelligent-Tiering. Use as políticas de ciclo de vida do S3 para mover os arquivos para o S3 Glacier Flexible Retrieval após 1 ano. Consulte e recupere os arquivos que estão no Amazon S3 usando o Amazon Athena. Consulte e recupere os arquivos que estão no S3 Glacier usando o S3 Glacier Select. (*)

### Uma empresa tem um site hospedado na AWS. O site está atrás de um Application Load Balancer (ALB) que está configurado para lidar com HTTP e HTTPS separadamente. A empresa quer encaminhar todas as solicitações para o site para que as solicitações usem HTTPS.
### O que um arquiteto de soluções deve fazer para atender a esse requisito?

* [X] Crie uma regra de ouvinte no ALB para redirecionar o tráfego HTTP para HTTPS. (*)

### Uma empresa coleta dados de temperatura, umidade e pressão atmosférica em cidades de vários continentes. O volume médio de dados que a empresa coleta de cada site diariamente é de 500 GB. Cada site tem uma conexão de Internet de alta velocidade.
### A empresa quer agregar os dados de todos esses sites globais o mais rápido possível em um único bucket do Amazon S3. A solução deve minimizar a complexidade operacional.
### Qual solução atende a esses requisitos?

* [X] Ative a aceleração de transferência do S3 no bucket do S3 de destino. Use multipart uploads para carregar diretamente os dados do site para o bucket do S3 de destino. (*)

### Uma empresa deseja migrar seu aplicativo local para a AWS. O aplicativo produz arquivos de saída que variam em tamanho de dezenas de gigabytes a centenas de terabytes. Os dados do aplicativo devem ser armazenados em uma estrutura de sistema de arquivos padrão. A empresa quer uma solução que escale automaticamente. é altamente disponível e requer sobrecarga operacional mínima.
### Qual solução atenderá a esses requisitos?

* [X] Migre o aplicativo para instâncias do Amazon EC2 em um grupo de Auto Scaling Multi-AZ. Use o Amazon Elastic File System (Amazon EFS) para armazenamento. (*)

### Uma empresa hospeda mais de 300 sites e aplicativos globais. A empresa exige uma plataforma para analisar mais de 30 TB de dados de clickstream por dia.
### O que um arquiteto de soluções deve fazer para transmitir e processar os dados de fluxo de cliques?

* [X] Colete os dados do Amazon Kinesis Data Streams. Use o Amazon Kinesis Data Firehose para transmitir os dados para um data lake do Amazon S3. Carregue os dados no Amazon Redshift para análise. (*)

### Uma empresa observa um aumento nos custos do Amazon EC2 em sua fatura mais recente. A equipe de faturamento percebe o dimensionamento vertical indesejado de tipos de instância para algumas instâncias do EC2. Um arquiteto de soluções precisa criar um gráfico comparando os últimos 2 meses de custos do EC2 e realizar uma análise aprofundada para identificar a causa raiz do dimensionamento vertical.
### Como o arquiteto de soluções deve gerar as informações com o MÍNIMO de sobrecarga operacional?

* [X] Use o recurso de filtragem granular do Cost Explorer para realizar uma análise detalhada dos custos do EC2 com base nos tipos de instância. (*)

### Uma empresa está administrando um site de mídia social popular. O site dá aos usuários a capacidade de carregar imagens para compartilhar com outros usuários. A empresa quer garantir que as imagens não contenham conteúdo impróprio. A empresa precisa de uma solução que minimize o esforço de desenvolvimento.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Use o Amazon Rekognition para detectar conteúdo impróprio. Use a revisão humana para previsões de baixa confiança. (*)

### Um arquiteto de soluções está usando o Amazon S3 para projetar a arquitetura de armazenamento de um novo aplicativo de mídia digital. Os arquivos de mídia devem ser resilientes à perda de uma zona de disponibilidade. Alguns arquivos são acessados com frequência, enquanto outros arquivos raramente são acessados em um padrão imprevisível. O arquiteto de soluções deve minimizar os custos de armazenamento e recuperação dos arquivos de mídia.
### Qual opção de armazenamento atende a esses requisitos?

* [X] S3 Intelligent-Tiering. (*)

### O aplicativo de uma empresa se integra a várias fontes de software como serviço (SaaS) para coleta de dados. A empresa executa instâncias do Amazon EC2 para receber os dados e fazer upload dos dados para um bucket do Amazon S3 para análise. A mesma instância do EC2 que recebe e carrega os dados também envia uma notificação ao usuário quando um upload é concluído. A empresa tem notado um desempenho lento do aplicativo e quer melhorar o desempenho o máximo possível.
### Qual solução atenderá a esses requisitos com a MENOR sobrecarga operacional?

* [X] Crie um fluxo do Amazon AppFlow para transferir dados entre cada origem SaaS e o bucket do S3. Configure uma notificação de evento do S3 para enviar eventos para um tópico do Amazon Simple Notification Service (Amazon SNS) quando o upload para o bucket do S3 estiver concluído. (*)

### Uma empresa hospeda seus aplicativos de vários níveis na AWS. Para fins de conformidade, governança, auditoria e segurança, a empresa deve acompanhar as alterações de configuração em seus recursos da AWS e registrar um histórico de chamadas de API feitas a esses recursos.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Use o AWS Config para acompanhar alterações de configuração e o AWS CloudTrail para registrar chamadas de API. (*)

### Uma empresa precisa da capacidade de analisar os arquivos de log de seu aplicativo proprietário. Os logs são armazenados no formato JSON em um bucket do Amazon S3. As consultas serão simples e serão executadas sob demanda. Um arquiteto de soluções precisa realizar a análise com alterações mínimas na arquitetura existente.
### O que o arquiteto de soluções deve fazer para atender a esses requisitos com o mínimo de sobrecarga operacional?

* [X] Use o Amazon Athena diretamente com o Amazon S3 para executar as consultas conforme necessário. (*)

### UDEMY####

### Uma empresa fornece uma interface baseada em REST para um aplicativo que permite que uma empresa parceira envie dados quase em tempo real. O aplicativo então processa os dados recebidos e os armazena para análise posterior. O aplicativo é executado em instâncias do Amazon EC2.
### A empresa parceira recebeu muitos erros 503 de serviço indisponível ao enviar dados para o aplicativo e a capacidade de computação atinge seus limites e não consegue processar solicitações quando ocorrem picos no volume de dados.
### Qual design um arquiteto de soluções deve implementar para melhorar a escalabilidade?

* [X] Use Amazon Kinesis Data Streams para ingerir os dados. Processe os dados usando funções AWS Lambda. (*)

### Um aplicativo em execução no Amazon EC2 precisa invocar de forma assíncrona uma função AWS Lambda para executar o processamento de dados. Os serviços devem ser desacoplados.
### Qual serviço pode ser usado para desacoplar os serviços de computação?

* [X] Amazon SNS. (*)

### Uma empresa usa uma instância de banco de dados MySQL do Amazon RDS para armazenar dados de pedidos de clientes. A equipe de segurança solicitou que a criptografia SSL/TLS em trânsito seja usada para criptografar conexões com o banco de dados de servidores de aplicativos. Os dados no banco de dados estão atualmente criptografados em repouso usando uma chave AWS KMS.
### Como um arquiteto de soluções pode habilitar a criptografia em trânsito?

* [X] Baixe os certificados raiz fornecidos pela AWS. Use os certificados ao conectar-se à instância do RDS DB. (*)

### Um novo aplicativo deve ser publicado em várias regiões ao redor do mundo. O Arquiteto precisa garantir que apenas 2 endereços IP precisem ser incluídos na lista de permissões. A solução deve rotear o tráfego de forma inteligente para a menor latência e fornecer failover regional rápido.
### Como isso pode ser alcançado?

* [X] Inicie instâncias do EC2 em várias regiões atrás de um NLB e use o AWS Global Accelerator. (*)
### Uma empresa precisa conectar sua rede de data center local a uma nova nuvem privada virtual (VPC). Há uma conexão de internet simétrica de 100 Mbps na rede do data center. A taxa de transferência de dados para um aplicativo local é de vários gigabytes por dia. O processamento será feito usando um fluxo do Amazon Kinesis Data Firehose.
### O que um arquiteto de soluções deve recomendar para desempenho máximo?

* [X] O Kinesis Data Firehose pode ser conectado à VPC usando o AWS PrivateLink. Instale uma conexão AWS Direct Connect de 1 Gbps entre a rede local e a AWS. Para enviar dados do local para o Kinesis Data Firehose, use o endpoint do PrivateLink. (*)

### Uma empresa executa um grande trabalho de processamento em lote no final de cada trimestre. O trabalho de processamento é executado por 5 dias e usa 15 instâncias do Amazon EC2. O processamento deve ser executado ininterruptamente por 5 horas por dia. A empresa está investigando maneiras de reduzir o custo do trabalho de processamento em lote.
### Qual modelo de precificação a empresa deve escolher?

* [X] Instâncias sob demanda (*)

### Uma organização quer compartilhar atualizações regulares sobre seu trabalho de caridade usando páginas da web estáticas. Espera-se que as páginas gerem uma grande quantidade de visualizações do mundo todo. Os arquivos são armazenados em um bucket do Amazon S3. Um arquiteto de soluções foi solicitado a projetar uma solução eficiente e eficaz.
### Que ação o arquiteto de soluções deve tomar para realizar isso?

* [X] Use o Amazon CloudFront com o bucket S3 como origem. (*)

### Uma empresa administra um site dinâmico que é hospedado em um servidor local nos Estados Unidos. A empresa está se expandindo para a Europa e está investigando como pode otimizar o desempenho do site para usuários europeus. O site deve permanecer nos Estados Unidos. A empresa requer uma solução que possa ser implementada em poucos dias.
### O que um arquiteto de soluções deve recomendar?

* [X] Use o Amazon CloudFront com uma origem personalizada apontando para os servidores locais. (*)

### Uma empresa executa um aplicativo que usa um banco de dados Amazon RDS PostgreSQL. O banco de dados não está criptografado no momento. Um Solutions Architect foi instruído que, devido a novos requisitos de conformidade, todos os dados existentes e novos no banco de dados devem ser criptografados. O banco de dados passa por altos volumes de alterações e nenhum dado pode ser perdido.
### Como o Arquiteto de Soluções pode habilitar a criptografia para o banco de dados sem incorrer em perda de dados?

* [X] Crie um snapshot da instância RDS DB existente. Crie uma cópia criptografada do snapshot. Crie uma nova instância RDS DB a partir do snapshot criptografado e atualize o aplicativo. Use o AWS DMS para sincronizar dados entre os RDS DBs de origem e de destino. (*)

### Uma empresa hospeda um aplicativo em instâncias do Amazon EC2 por trás de Application Load Balancers em várias regiões da AWS. Os direitos de distribuição para o conteúdo exigem que usuários em diferentes geografias recebam conteúdo de regiões específicas.
### Qual configuração atende a esses requisitos?

* [X] Crie registros do Amazon Route 53 com uma política de roteamento de geolocalização. (*)

### O aplicativo de uma empresa está sendo executado em instâncias do Amazon EC2 em uma única região. No caso de um desastre, um arquiteto de soluções precisa garantir que os recursos também possam ser implantados em uma segunda região.
### Que combinação de ações o arquiteto de soluções deve tomar para realizar isso? (Selecione DUAS.)

* [X] Inicie uma nova instância do EC2 a partir de uma Amazon Machine Image (AMI) na segunda região (*)

* [X] Copie uma Amazon Machine Image (AMI) de uma instância EC2 e especifique a segunda região para o destino (*)

### Uma seguradora tem um aplicativo da web que atende usuários no Reino Unido e na Austrália. O aplicativo inclui uma camada de banco de dados usando um banco de dados MySQL hospedado em eu-west-2. A camada da web é executada a partir de eu-west-2 e ap-southeast-2. O roteamento de geoproximidade do Amazon Route 53 é usado para direcionar usuários para a camada da web mais próxima. Foi observado que os usuários australianos recebem tempos de resposta lentos para consultas.
### Quais alterações devem ser feitas na camada do banco de dados para melhorar o desempenho?

* [X] Migre o banco de dados para um banco de dados global Amazon Aurora no modo de compatibilidade MySQL. Configure réplicas de leitura em ap-southeast-2 (*)

### Um aplicativo legado de High Performance Computing (HPC) rigidamente acoplado será migrado para a AWS. Qual tipo de adaptador de rede deve ser usado?

* [X] Adaptador de Tecido Elástico (EFA) (*)

### Uma empresa exige que todas as contas de usuário do AWS IAM tenham requisitos específicos de complexidade e comprimento mínimo de senha.
### Como um arquiteto de soluções deve fazer isso?

* [X] Defina uma política de senha para toda a conta da AWS. (*)

### Uma empresa deseja restringir o acesso à sua tabela Amazon DynamoDB a endereços IP de origem específicos e privados de sua VPC. O que deve ser feito para proteger o acesso à tabela?

* [X] Crie um ponto de extremidade VPC de gateway e adicione uma entrada à tabela de rotas (*)

### Uma empresa implantou um novo site em instâncias do Amazon EC2 por trás de um Application Load Balancer (ALB). O Amazon Route 53 é usado para o serviço DNS. A empresa pediu a um Solutions Architect para criar um site de backup com detalhes de contato de suporte para os quais os usuários serão direcionados automaticamente se o site principal estiver inativo.
### Como o arquiteto de soluções deve implantar esta solução de forma econômica?

* [X] Configure um site estático usando o Amazon S3 e crie uma política de roteamento de failover do Route 53. (*)

### Uma empresa de produção de vídeo está planejando mover algumas de suas cargas de trabalho para a Nuvem AWS. A empresa precisará de cerca de 5 TB de armazenamento para processamento de vídeo com o máximo desempenho de E/S possível. Eles também precisam de mais de 400 TB de armazenamento extremamente durável para armazenar arquivos de vídeo e 800 TB de armazenamento para arquivamento de longo prazo.
### Quais combinações de serviços um Arquiteto de Soluções deve usar para atender a esses requisitos?

* [X] Armazenamento de instância do Amazon EC2 para desempenho máximo, Amazon S3 para armazenamento de dados duráveis ​​e Amazon S3 Glacier para armazenamento de arquivamento. (*)

### Há dois aplicativos em uma empresa: um aplicativo remetente que envia mensagens contendo payloads e um aplicativo de processamento que recebe mensagens contendo payloads. A empresa quer implementar um serviço AWS para manipular mensagens entre esses dois aplicativos diferentes. O aplicativo remetente envia em média 1.000 mensagens a cada hora e as mensagens, dependendo do tipo, às vezes levam até 2 dias para serem processadas. Se as mensagens não forem processadas, elas devem ser retidas para que não afetem o processamento de nenhuma mensagem restante.
### Qual solução atende a esses requisitos e é a MAIS eficiente operacionalmente? 

* [X] Forneça uma fila do Amazon Simple Queue Service (Amazon SQS) para os aplicativos remetente e processador. Configure uma fila de mensagens mortas para coletar mensagens com falha. (*)

### Uma empresa está investigando métodos para reduzir as despesas associadas à infraestrutura de backup local. O Solutions Architect quer reduzir custos eliminando o uso de fitas de backup físicas. É um requisito que os aplicativos e fluxos de trabalho de backup existentes continuem funcionando.
### O que o Arquiteto de Soluções deve recomendar?

* [X] Conecte os aplicativos de backup a um AWS Storage Gateway usando uma biblioteca de fitas virtuais (VTL) iSCSI. (*)

### Uma empresa hospeda um jogo multijogador na AWS. O aplicativo usa instâncias do Amazon EC2 em uma única Zona de Disponibilidade e os usuários se conectam pela Camada 4. O Solutions Architect foi encarregado de tornar a arquitetura altamente disponível e também mais econômica.
### Como o arquiteto de soluções pode atender melhor a esses requisitos? (Selecione DUAS.)

* [X] Configurar um balanceador de carga de rede na frente das instâncias do EC2 (*)

* [X] Configurar um grupo de dimensionamento automático para adicionar ou remover instâncias em várias zonas de disponibilidade automaticamente (*)

### Um farm de servidores de arquivos do Microsoft Windows usa Distributed File System Replication (DFSR) para sincronizar dados em um ambiente local. A infraestrutura está sendo migrada para a Nuvem AWS.
### Qual serviço o arquiteto de soluções deve usar para substituir o farm de servidores de arquivos?

* [X] Amazon FSx (*)

### Uma equipe de topografia está usando uma frota de drones para coletar imagens de canteiros de obras. Os laptops da equipe de topografia não têm capacidade de armazenamento e computação embutida para transferir as imagens e processar os dados. Embora a equipe tenha instâncias do Amazon EC2 para processamento e buckets do Amazon S3 para armazenamento, a conectividade de rede é intermitente e não confiável. As imagens precisam ser processadas para avaliar o progresso de cada canteiro de obras.
### O que um arquiteto de soluções deve recomendar?

* [X] Processe e armazene as imagens usando dispositivos AWS Snowball Edge. (*)

### Uma empresa de serviços financeiros tem um aplicativo da Web com uma camada de aplicativo em execução nos EUA e na Europa. A camada de banco de dados consiste em um banco de dados MySQL em execução no Amazon EC2 em us-west-1. Os usuários são direcionados para a camada de aplicativo mais próxima usando o roteamento baseado em latência do Route 53. Os usuários na Europa relataram desempenho ruim ao executar consultas.
### Quais alterações um arquiteto de soluções deve fazer na camada do banco de dados para melhorar o desempenho?

* [X] Migre o banco de dados para um banco de dados global Amazon Aurora no modo de compatibilidade MySQL. Configure a camada de aplicativo na Europa para usar o endpoint do leitor local. (*)

### Um site é executado em instâncias do Amazon EC2 em um grupo de Auto Scaling por trás de um Application Load Balancer (ALB) que serve como origem para uma distribuição do Amazon CloudFront. Um AWS WAF está sendo usado para proteger contra ataques de injeção de SQL. Uma revisão de logs de segurança revelou um IP malicioso externo que precisa ser bloqueado para acessar o site.
### O que um arquiteto de soluções deve fazer para proteger o aplicativo?

* [X] Modifique a configuração do AWS WAF para adicionar uma condição de correspondência de IP para bloquear o endereço IP malicioso (*)

### Um Solutions Architect implantou um aplicativo em várias instâncias do Amazon EC2 em três sub-redes privadas. O aplicativo deve ser disponibilizado para clientes baseados na Internet com o mínimo de esforço administrativo.
### Como o Arquiteto de Soluções pode disponibilizar o aplicativo na internet?

* [X] Crie um Application Load Balancer e associe três sub-redes públicas das mesmas Availability Zones que as instâncias privadas. Adicione as instâncias privadas ao ALB. (*)

### Uma empresa planeja tornar uma instância do Amazon EC2 Linux indisponível fora do horário comercial para economizar custos. A instância é apoiada por um volume do Amazon EBS. Há um requisito de que o conteúdo da memória da instância deve ser preservado quando ela for tornada indisponível.
### Como um arquiteto de soluções pode atender a esses requisitos?

* [X] Hiberne a instância fora do horário comercial. Inicie a instância novamente quando necessário. (*)

### Um aplicativo em execução em uma instância de contêiner do Amazon ECS usando o tipo de inicialização do EC2 precisa de permissões para gravar dados no Amazon DynamoDB.
### Como você pode atribuir essas permissões apenas à tarefa específica do ECS que está executando o aplicativo?

* [X] Crie uma política do IAM com permissões para o DynamoDB e atribua-a a uma tarefa usando o parâmetro taskRoleArn (*)

### Um Amazon VPC contém várias instâncias do Amazon EC2. As instâncias precisam fazer chamadas de API para o Amazon DynamoDB. Um arquiteto de soluções precisa garantir que as chamadas de API não atravessem a internet.
### Como isso pode ser feito? (Selecione DUAS.)

* [X] Crie um ponto de extremidade de gateway para o DynamoDB (*)

* [X] Crie uma entrada de tabela de rotas para o ponto de extremidade (*)

### Um arquiteto de soluções está criando um aplicativo de envio de documentos para uma escola. O aplicativo usará um bucket do Amazon S3 para armazenamento. A solução deve impedir a exclusão acidental dos documentos e garantir que todas as versões dos documentos estejam disponíveis. Os usuários devem ser capazes de carregar e modificar os documentos.
### Que combinação de ações deve ser tomada para atender a esses requisitos? (Selecione DUAS.)

* [X] Habilitar versionamento no bucket (*)

* [X] Habilitar exclusão de MFA no bucket (*)

### Uma empresa executa um aplicativo em uma instância do Amazon EC2 que requer 250 GB de espaço de armazenamento. O aplicativo não é usado com frequência e tem pequenos picos de uso nas manhãs e tardes dos dias úteis. A E/S do disco pode variar com picos atingindo um máximo de 3.000 IOPS. Um arquiteto de soluções deve recomendar a solução de armazenamento mais econômica que ofereça o desempenho necessário.
### Qual configuração o Arquiteto de Soluções deve recomendar?
### Qual solução o arquiteto de soluções deve recomendar?

* [X] Amazon EBS SSD de uso geral (gp2) (*)

### A camada de banco de dados de um aplicativo da Web está sendo executada em um servidor Windows local. O banco de dados é um banco de dados Microsoft SQL Server. O proprietário do aplicativo gostaria de migrar o banco de dados para uma instância do Amazon RDS.
### Como a migração pode ser executada com o mínimo de esforço administrativo e tempo de inatividade?

* [X] Use o AWS Database Migration Service (DMS) para migrar diretamente o banco de dados para o RDS. (*)

### Uma equipe está planejando executar trabalhos de análise em arquivos de log todos os dias e precisa de uma solução de armazenamento. O tamanho e o número de logs são desconhecidos e os dados persistirão por apenas 24 horas.
### Qual é a solução MAIS econômica?

* [X] Padrão Amazon S3 (*)

### Uma empresa carregou alguns dados altamente críticos para um bucket do Amazon S3. A gerência está preocupada com a disponibilidade dos dados e exige que medidas sejam tomadas para proteger os dados de exclusão acidental. Os dados ainda devem estar acessíveis, e um usuário deve ser capaz de excluí-los intencionalmente.
### Que combinação de etapas um arquiteto de soluções deve seguir para realizar isso? (Selecione DUAS.)

* [X] Habilite o controle de versão no bucket S3. (*)

* [X] Habilite a exclusão de MFA no bucket S3. (*)

### Uma organização tem uma grande quantidade de dados em compartilhamentos de arquivos do Windows (SMB) em seu data center local. A organização gostaria de mover dados para o Amazon S3. Eles gostariam de automatizar a migração de dados por meio de seu link AWS Direct Connect.
### Qual serviço da AWS pode ajudá-los?

* [X] Sincronização de dados da AWS. (*)

### Um aplicativo da web é executado em sub-redes públicas e privadas. A arquitetura do aplicativo consiste em uma camada da web e uma camada de banco de dados em execução em instâncias do Amazon EC2. Ambas as camadas são executadas em uma única Zona de Disponibilidade (AZ).
### Qual combinação de etapas um arquiteto de soluções deve adotar para fornecer alta disponibilidade para esta arquitetura? (Selecione DUAS.)

* [X] Crie um grupo de dimensionamento automático do Amazon EC2 e um balanceador de carga de aplicativos (ALB) abrangendo várias AZs (*)

* [X] Crie novas sub-redes públicas e privadas na mesma VPC, cada uma em uma nova AZ. Migre o banco de dados para uma implantação multi-AZ do Amazon RDS (*)

### Uma empresa de varejo com muitas lojas e depósitos está implementando sensores de IoT para coletar dados de monitoramento de dispositivos em cada local. Os dados serão enviados para a AWS em tempo real. Um arquiteto de soluções deve fornecer uma solução para garantir que os eventos sejam recebidos em ordem para cada dispositivo e garantir que os dados sejam salvos para processamento futuro.
### Qual solução seria MAIS eficiente?

* [X] Use Amazon Kinesis Data Streams para eventos em tempo real com uma chave de partição para cada dispositivo. Use Amazon Kinesis Data Firehose para salvar dados no Amazon S3 (*)

### Um aplicativo de comércio eletrônico consiste em três camadas. A camada da web inclui instâncias EC2 por trás de um Application Load Balancer, a camada intermediária usa instâncias EC2 e uma fila Amazon SQS para processar pedidos, e a camada do banco de dados consiste em uma tabela Auto Scaling DynamoDB. Durante períodos de pico, os clientes reclamaram sobre atrasos no processamento de pedidos. Um Solutions Architect foi encarregado de reduzir os tempos de processamento.
### Qual ação será MAIS eficaz para cumprir esse requisito?

* [X] Use o Amazon EC2 Auto Scaling para dimensionar as instâncias de camada intermediária com base na profundidade da fila do SQS. (*)

### Uma réplica de leitura do Amazon RDS está sendo implantada em uma região separada. O banco de dados mestre não é criptografado, mas todos os dados na nova região devem ser criptografados. Como isso pode ser alcançado?

* [X] Criptografe um instantâneo da instância mestre do banco de dados, crie uma nova instância mestre do banco de dados criptografada e, em seguida, crie uma réplica de leitura criptografada entre regiões (*)

### As instâncias do Amazon EC2 em um ambiente de desenvolvimento são executadas entre 9h e 17h, de segunda a sexta-feira. As instâncias de produção são executadas 24 horas por dia, 7 dias por semana. Quais modelos de precificação devem ser usados ​​para otimizar os custos e garantir que a capacidade esteja disponível? (Selecione DOIS.)

* [X] Reservas de capacidade sob demanda para o ambiente de desenvolvimento (*)

* [X] Use instâncias reservadas para o ambiente de produção (*)

### Uma empresa executa um aplicativo em um data center local que coleta dados ambientais de máquinas de produção. Os dados consistem em arquivos JSON armazenados em armazenamento conectado à rede (NAS) e cerca de 5 TB de dados são coletados a cada dia. A empresa deve carregar esses dados no Amazon S3, onde podem ser processados ​​por um aplicativo de análise. Os dados devem ser transferidos com segurança.
### Qual solução oferece a transferência de dados MAIS confiável e eficiente em termos de tempo?

* [X] AWS DataSync via AWS Direct Connect. (*)

### Uma empresa executa aplicativos em contêineres para muitas cargas de trabalho de aplicativos em um data center local. A empresa está planejando implantar contêineres na AWS e o arquiteto chefe determinou que a mesma configuração e ferramentas administrativas devem ser usadas em todos os ambientes em contêineres. A empresa também deseja permanecer agnóstica em relação à nuvem para se proteger contra o impacto de futuras mudanças na estratégia de nuvem.
### Como um arquiteto de soluções pode projetar uma solução gerenciada que se alinhe ao software de código aberto?

* [X] Inicie os contêineres no Amazon Elastic Kubernetes Service (EKS) e nos nós de trabalho do EKS. (*)

### Um arquiteto de soluções está projetando um novo serviço que usará uma API do Amazon API Gateway no frontend. O serviço precisará persistir dados em um banco de dados de backend usando solicitações de chave-valor. Inicialmente, os requisitos de dados serão em torno de 1 GB e o crescimento futuro é desconhecido. As solicitações podem variar de 0 a mais de 800 solicitações por segundo.
### Qual combinação de serviços da AWS atenderia a esses requisitos? (Selecione DUAS.)

* [X] AWS Lambda (*)

* [X] Amazon DynamoDB (*)

### Um arquiteto de soluções está criando um sistema que executará análises em dados financeiros por várias horas por noite, 5 dias por semana. Espera-se que a análise seja executada pela mesma duração e não possa ser interrompida depois de iniciada. O sistema será necessário por no mínimo 1 ano.
### O que o arquiteto de soluções deve configurar para garantir que as instâncias do EC2 estejam disponíveis quando necessárias?

* [X] Reservas de capacidade sob demanda (*)

### Um aplicativo da web permite que os usuários carreguem fotos e adicionem elementos gráficos a elas. O aplicativo oferece dois níveis de serviço: gratuito e pago. Fotos carregadas por usuários pagos devem ser processadas antes daquelas enviadas usando o nível gratuito. As fotos são carregadas em um bucket do Amazon S3 que usa uma notificação de evento para enviar as informações do trabalho para o Amazon SQS.
### Como um arquiteto de soluções deve configurar a implantação do Amazon SQS para atender a esses requisitos?

* [X] Use uma fila SQS Standard separada para cada nível. Configure instâncias do Amazon EC2 para priorizar a pesquisa para a fila paga em vez da fila gratuita. (*)

### O aplicativo web de uma empresa está usando várias instâncias do Amazon EC2 Linux e armazenando dados em volumes do Amazon EBS. A empresa está procurando uma solução para aumentar a resiliência do aplicativo em caso de falha.
### O que um arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Crie um Application Load Balancer com grupos de Auto Scaling em várias Availability Zones. Armazene dados no Amazon EFS e monte um destino em cada instância (*)

### Uma empresa de comércio eletrônico executa um aplicativo em instâncias do Amazon EC2 em sub-redes públicas e privadas. O aplicativo da web é executado em uma sub-rede pública e o banco de dados é executado em uma sub-rede privada. Ambas as sub-redes públicas e privadas estão em uma única Zona de Disponibilidade.
### Qual combinação de etapas um arquiteto de soluções deve adotar para fornecer alta disponibilidade para esta arquitetura? (Selecione DUAS.)

* [X] Crie novas sub-redes públicas e privadas em uma AZ diferente. Migre o banco de dados para uma implantação multi-AZ do Amazon RDS. (*)

* [X] Crie um grupo de dimensionamento automático do EC2 e um balanceador de carga de aplicativo que abranja várias zonas de disponibilidade. (*)

### Uma empresa oferece um folheto de produto on-line que é entregue de um site estático em execução no Amazon S3. Os clientes da empresa estão principalmente nos Estados Unidos, Canadá e México. A empresa está buscando reduzir de forma econômica a latência para usuários nessas regiões.
### Qual é a solução mais econômica para esses requisitos?

* [X] Crie uma distribuição do Amazon CloudFront e defina a classe de preço para usar apenas EUA, Canadá e México. (*)

### Uma empresa está migrando de uma infraestrutura local para a Nuvem AWS. Um dos aplicativos da empresa armazena arquivos em um farm de servidores de arquivos do Windows que usa Distributed File System Replication (DFSR) para manter os dados sincronizados. Um arquiteto de soluções precisa substituir o farm de servidores de arquivos.
### Qual serviço o arquiteto de soluções deve usar?

* [X] Amazon FSx (*)

### Um arquiteto de soluções está projetando a infraestrutura para executar um aplicativo em instâncias do Amazon EC2. O aplicativo requer alta disponibilidade e deve ser dimensionado dinamicamente com base na demanda para ser econômico.
### O que o arquiteto de soluções deve fazer para atender a esses requisitos?

* [X] Configurar um Application Load Balancer na frente de um grupo de dimensionamento automático para implantar instâncias em várias zonas de disponibilidade (*)

### Um arquiteto de soluções precisa fazer backup de alguns arquivos de log de aplicativo de uma loja de comércio eletrônico on-line para o Amazon S3. Não se sabe com que frequência os logs serão acessados ​​ou quais logs serão mais acessados. O arquiteto de soluções deve manter os custos o mais baixo possível usando a classe de armazenamento S3 apropriada.
### Qual classe de armazenamento S3 deve ser implementada para atender a esses requisitos?

* [X] S3 Intelligent-Tiering (*)

### Um aplicativo está sendo criado para usar instâncias do Amazon EC2 para gerar e armazenar dados. Outro conjunto de instâncias do EC2 analisará e modificará os dados. Os requisitos de armazenamento serão significativos e continuarão a crescer ao longo do tempo. Os arquitetos de aplicativos exigem uma solução de armazenamento.
### Quais ações atenderiam a essas necessidades?

* [X] Armazene os dados em um sistema de arquivos Amazon EFS. Monte o sistema de arquivos nas instâncias do aplicativo. (*)

### Uma organização da AWS tem uma UO com várias contas de membros. A empresa precisa restringir a capacidade de iniciar apenas tipos específicos de instância do Amazon EC2. Como essa política pode ser aplicada em todas as contas com o mínimo de esforço?

* [X] Crie um SCP com uma regra de negação que negue todos os tipos de instância, exceto os específicos (*)

### Uma empresa entrega conteúdo para assinantes distribuídos globalmente a partir de um aplicativo em execução na AWS. O aplicativo usa uma frota de instâncias do Amazon EC2 em uma sub-rede privada atrás de um Application Load Balancer (ALB). Devido a uma atualização nas restrições de direitos autorais, é necessário bloquear o acesso para países específicos.
### Qual é o método MAIS FÁCIL de atender a esse requisito?

* [X] Use o Amazon CloudFront para atender ao aplicativo e negar acesso a países bloqueados (*)

### Um banco de dados persistente deve ser migrado de um servidor local para uma instância do Amazon EC2. O banco de dados requer 64.000 IOPS e, se possível, deve ser armazenado em um único volume do Amazon EBS.
### Qual solução um arquiteto de soluções deve recomendar?

* [X] Crie uma instância do Amazon EC2 baseada em Nitro com um volume Amazon EBS Provisioned IOPS SSD (i01) anexado. Provisione 64.000 IOPS para o volume. (*)

### Uma empresa executa um aplicativo em uma fábrica que tem um pequeno rack de recursos de computação física. O aplicativo armazena dados em um dispositivo de armazenamento conectado à rede (NAS) usando o protocolo NFS. A empresa exige um backup diário externo dos dados do aplicativo.
### Qual solução um Arquiteto de Soluções pode recomendar para atender a esse requisito?

* [X] Use um dispositivo de hardware de gateway de arquivos do AWS Storage Gateway no local para replicar os dados para o Amazon S3. (*)

### Uma empresa executa um aplicativo da Web que fornece atualizações meteorológicas. O aplicativo é executado em uma frota de instâncias do Amazon EC2 em um grupo de dimensionamento automático Multi-AZ atrás de um Application Load Balancer (ALB). As instâncias armazenam dados em um banco de dados Amazon Aurora. Um arquiteto de soluções precisa tornar o aplicativo mais resiliente a aumentos esporádicos nas taxas de solicitação.
### Qual arquitetura o arquiteto de soluções deve implementar? (Selecione DUAS.)

* [X] Adicionar réplicas do Amazon Aurora (*)

* [X] Adicione uma distribuição do Amazon CloudFront na frente do ALB (*)

### Uma empresa executa um aplicativo em seis servidores de aplicativos da Web em um grupo de Auto Scaling do Amazon EC2 em uma única Zona de Disponibilidade. O aplicativo é frontado por um Application Load Balancer (ALB). Um Solutions Architect precisa modificar a infraestrutura para ser altamente disponível sem fazer nenhuma modificação no aplicativo.
### Qual arquitetura o arquiteto de soluções deve escolher para permitir alta disponibilidade?

* [X] Modifique o grupo de dimensionamento automático para usar duas instâncias em cada uma das três zonas de disponibilidade. (*)

### Uma empresa está implantando uma frota de instâncias do Amazon EC2 executando Linux em várias Zonas de Disponibilidade dentro de uma Região da AWS. O aplicativo requer uma solução de armazenamento de dados que possa ser acessada por todas as instâncias do EC2 simultaneamente. A solução deve ser altamente escalável e fácil de implementar. O armazenamento deve ser montado usando o protocolo NFS.
### Qual solução atende a esses requisitos?

* [X] Crie um sistema de arquivos Amazon EFS com alvos de montagem em cada Availability Zone. Configure as instâncias do aplicativo para montar o sistema de arquivos. (*)

### Uma empresa tem duas contas para executar testes e cada conta tem uma única VPC: VPC-TEST1 e VPC-TEST2. A equipe de operações requer um método de cópia segura de arquivos entre instâncias do Amazon EC2 nessas VPCs. A conectividade não deve ter nenhum ponto único de falha ou restrições de largura de banda.
### Qual solução um arquiteto de soluções deve recomendar?

* [X] Crie uma conexão de peering de VPC entre VPC-TEST1 e VPC-TEST2. (*)

### Um novo aplicativo será executado em várias tarefas do Amazon ECS. A lógica do aplicativo front-end processará dados e, em seguida, passará esses dados para uma tarefa do ECS back-end para executar processamento adicional e gravar os dados em um datastore. O Architect gostaria de reduzir as interdependências para que as falhas não afetem outros componentes.
### Qual solução o arquiteto deve usar?

* [X] Crie uma fila do Amazon SQS e configure o front-end para adicionar mensagens à fila e o back-end para pesquisar mensagens na fila (*)

### Um desenvolvedor criou um aplicativo que usa o Amazon EC2 e uma instância de banco de dados MySQL do Amazon RDS. O desenvolvedor armazenou o nome de usuário e a senha do banco de dados em um arquivo de configuração no volume EBS raiz da instância do aplicativo EC2. Um Solutions Architect foi solicitado a projetar uma solução mais segura.
### O que o Arquiteto de Soluções deve fazer para atender a esse requisito?

* [X] Crie uma função IAM com permissão para acessar o banco de dados. Anexe essa função IAM à instância EC2. (*)

### Uma empresa está trabalhando com um parceiro estratégico que tem um aplicativo que deve ser capaz de enviar mensagens para uma das filas do Amazon SQS da empresa. A empresa parceira tem sua própria conta AWS.
### Como um arquiteto de soluções pode fornecer acesso de privilégios mínimos ao parceiro?

* [X] Atualize a política de permissão na fila SQS para conceder a permissão sqs:SendMessage à conta AWS do parceiro. (*)

### Um Solutions Architect foi encarregado de reimplantar um aplicativo em execução na AWS para habilitar alta disponibilidade. O aplicativo processa mensagens que são recebidas em uma fila ActiveMQ em execução em uma única instância do Amazon EC2. As mensagens são então processadas por um aplicativo consumidor em execução no Amazon EC2. Após processar as mensagens, o aplicativo consumidor grava os resultados em um banco de dados MySQL em execução no Amazon EC2.
### Qual arquitetura oferece maior disponibilidade e baixa complexidade operacional?

* [X] Implante o Amazon MQ com brokers ativos/em espera configurados em duas Zonas de Disponibilidade. Crie um grupo de Auto Scaling para as instâncias EC2 do consumidor em duas Zonas de Disponibilidade. Use um banco de dados MySQL do Amazon RDS com Multi-AZ habilitado. (*)

### A capacidade de armazenamento se tornou um problema para uma empresa que executa servidores de aplicativos no local. Os servidores são conectados a uma combinação de soluções de armazenamento em bloco e armazenamento NFS. A empresa requer uma solução que suporte cache local sem reestruturar seus aplicativos existentes.
### Que combinação de mudanças a empresa pode fazer para atender a esses requisitos? (Selecione DUAS.)

* [X] Use um gateway de volume do AWS Storage Gateway para substituir o armazenamento em bloco. (*)

* [X] Use um gateway de arquivo do AWS Storage Gateway para substituir o armazenamento NFS. (*)

### Um bucket do Amazon S3 na região us-east-1 hospeda o conteúdo estático do site de uma empresa. O conteúdo é disponibilizado por meio de uma origem do Amazon CloudFront apontando para esse bucket. Uma segunda cópia do bucket é criada na região ap-southeast-1 usando replicação entre regiões. O arquiteto-chefe de soluções quer uma solução que forneça maior disponibilidade para o site.
### Qual combinação de ações um arquiteto de soluções deve tomar para aumentar a disponibilidade? (Selecione DUAS.)

* [X] Usando o bucket us-east-1 como o bucket primário e o bucket ap-southeast-1 como o bucket secundário, crie um grupo de origem do CloudFront. (*)

* [X] Adicione uma origem para ap-southeast-1 ao CloudFront. (*)

###

* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
* [X] Use AWS Secrets Manager. Ative a rotação automática. (*)
