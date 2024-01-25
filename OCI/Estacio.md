
#### SCRUM ####
####XP e Kanban são práticas de gerenciamento de projetos de software populares entre praticantes do desenvolvimento ágil.
###Um aspecto de divergência entre as duas práticas é:

* [X] processo iterativo. (*)

####    Em relação aos requisitos, qual é a principal diferença entre uma abordagem preditiva e uma ágil?

* [X] Na abordagem preditiva, os requisitos são definidos previamente, antes do início do desenvolvimento, na abordagem ágil, os requisitos são elaborados com frequência durante a entrega. (*)

#### (MPE-PA / 2012 - adaptada) A metodologia ágil Extreme Programming (XP) baseia-se em 14 práticas, algumas das quais são adotadas há muitos anos na indústria de software. A prática na qual se focaliza o aperfeiçoamento do projeto de software e que está presente em todo o desenvolvimento é chamada de:
* [X] refatoração. (*)

#### Qual alternativa contém somente tópicos tratados na seção "um sistema de entrega de valor" do padrão de gerenciamento de projetos do Guia PMBOK?

* [X] Governança, funções associadas a projetos, ambiente do projeto e gerenciamento de produto. (*)


#### Independentemente da área de atuação profissional, qualidade e capricho são características valorizadas no fluxo de trabalho. Com esses aspectos em mente, quando devemos levar em conta a qualidade?

* [X] Em cada ciclo, desde a primeira etapa. (*)

#### Uma das formas mais eficientes para estabelecer a missão da equipe é pelo sistema OKR, amplamente utilizado por empresas como Google, LinkedIn e Spotify. Qual alternativa melhor descreve o que deve conter em um objetivo segundo o OKR?

* [X] O objetivo deve ser curto, inspirador e envolvente, além de motivar e desafiar a equipe. (*)

#### Acerca dos métodos ágeis, assinale a opção que completa corretamente a lacuna da sentença abaixo.
#_______________ é organizado por colunas que representam um fluxo trabalho pelo qual passam itens ou tarefas desenvolvidas. É visual e as atividades ficarão explícitas à todos os membros de um time.

* [X] Quadro kanban (*)


####   O Guia PMBOK é um framework que fornece princípios e domínios de desempenho que podem ser usados pelos métodos ágeis com o intuito de entregar valor nos projetos. Quais são os domínios de desempenho do Guia PMBOK?

* [X] Partes interessadas, Equipe, Abordagem de desenvolvimento e Ciclo de vida, Planejamento, Trabalho do projeto, Entrega, Medição, Incerteza. (*)

#### A metodologia XP surgiu no final da década de 90, após o início da Internet, levando a mudanças significativas no ciclo de desenvolvimento de software. Qual dos seguintes aspectos NÃO é uma prática de Programação Extrema?

* [X] Capacitar clientes. (*)


#### Independentemente do método ágil adotado por uma organização, imprevistos podem acontecer e será necessário lidar com as eventuais mudanças. Acerca do Guia PMBOK, qual é o princípio da Mudança?

* [X] Aceite a mudança para alcançar o futuro estado previsto. (*)


####    23: Security-Data

####    As an administrator for a database system in OCI, you need to create credentials for a new user. How can you store these credentials securely to prevent unauthorized access? Which is the best option?
* [ ] Store the credentials in a separate database system.
* [ ] Store the credentials in a code or configuration file.
* [X] Store the credentials in OCI Vault as a secret.
* [ ] Use a third-party service to store the credentials.

####    As a security analyst for a financial company, you are tasked with ensuring the confidentiality and integrity of sensitive data. You need to decide which encryption method to use for protecting the company's data. Which two of the following statements about asymmetric and symmetric key encryption are true?
* [X] Asymmetric encryption uses two keys, one for encryption and another for decryption.
* [ ] Asymmetric encryption uses a single key to encrypt and decrypt data.
* [ ] Symmetric encryption uses two keys to perform the encryption.
* [X] Symmetric encryption uses a single key to encrypt and decrypt data.

####    Which statement about key rotation in OCI Vault is true?
* [X] Key rotation limits data encrypted or signed by one key version, reducing risk if a key is compromised.
* [ ] After rotating a key, the older key version can still be used for encryption purposes.
* [ ] Key rotation is not necessary since the keys are automatically assigned unique identifiers.
* [ ] Only symmetric keys can be rotated in OCI Vault.

####    Which of the following encryption algorithms are supported by the OCI Vault service?
* [ ] Elliptic curve digital signature algorithm (ECDSA)
* [X] All of the mentioned algorithms
* [ ] Rivest-Shamir-Adleman (RSA) algorithm
* [ ] Advanced Encryption Standard (AES)

####    What is the purpose of Oracle Cloud Infrastructure OCI Vault—Key Management?
* [X] To provide centralized management of encryption keys and secrets across a range of OCI services and applications
* [ ] To automate administrative tasks such as hardware provisioning and software patching
* [ ] To manage and control access to data across multiple cloud providers
* [ ] To protect data against cyberattacks and malicious actors

#### 25: Observability and Management

####    You are tasked to review and run routine checks for Alarms configured in the Oracle Cloud Infrastructure environment. To choose notification methods, which configuration should be updated?
* [ ] Grouping Function
* [ ] Streaming
* [X] Notification Topics (*)
* [ ] Oracle Function

####    You want to filter aggregated data by a specific resource ID. What is used in Basic and Advanced Modes to achieve this?
* [ ] Comparison Operator
* [X] Dimension (*)
* [ ] PostMetricData API
* [ ] Statistic
* [ ] Resolution

####    What is the maximum duration of Alarm history stored for the Monitoring service?
* [ ] 6 months
* [X] 90 days (*)
* [ ] 30 days
* [ ] 60 days
* [ ] 1 year

####    Which three are mandatory components for defining a metric query?
* [ ] Grouping
* [X] Metric (*)
* [X] Interval (*)
* [X] Statistic (*)
* [ ] Dimension

####    Which component controls the length of each time window in a metric query?
* [ ] Dimension
* [X] Interval (*)
* [ ] Namespace
* [ ] Statistic
* [ ] Resolution

#### 26: Observability and Management - Logging

####    You have a requirement to collect custom logs from an on-premises external application and archive low-priority log data into Object Storage buckets. Which two of the following options are involved in achieving this?
* [ ] Cloud Agent Plugin
* [ ] Topics
* [ ] Monitoring Alarms
* [X] Fluentd Agent (*)
* [X] Service Connectors (*)

####    Which statement best describes the purpose of a log group in the OCI Logging service?
* [ ] A log group is used to filter log data collected from a specific log source.
* [ ] A log group is used to archive log data collected from a specific log source.
* [ ] A log group is used to define the format of log data collected from a specific log source.
* [X] A log group is used to organize log data from multiple log sources that share common properties. (*)

####    In OCI Logging service, an Agent Configuration is created to enable Custom log ingestion from Compute Instances. As part of the Agent Configuration, which of the following is selected to choose Instances to ingest logs from the Compartment?
* [ ] Log Inputs
* [ ] Parsers
* [X] Host Group (*)
* [ ] Log Destination
* [ ] Security List

####    Which two are log categories of Object Storage Service Logs?
* [ ] Deployment Events
* [X] Write Access Events (*)
* [X] Read Access Events (*)
* [ ] Archive Events
* [ ] Total Usage Events

####    Which three types of logs are used by the Logging service?
* [ ] Alert Logs
* [X] Custom Logs (*)
* [X] Audit Logs (*)
* [ ] Archive Logs
* [X] Service Logs (*)
* [ ] Trace Logs

####    Compartment A is a child compartment of root.Compartment B is a child compartment of Compartment A.Compartment C is a child compartment of Compartment B.You have attached the following policy to Compartment A.Allow group NetworkAdmins to manage virtual-network-family in Compartment A.For which compartments can a user of the NetworkAdmins group manage VCNs?
* [X] Compartment A, Compartment B, and Compartment C only (*)
* [ ] Root compartment, Compartment A, Compartment B, and Compartment C
* [ ] Compartment B and Compartment C only
* [ ] Compartment A only

####    Your application or workload includes big data, analytics, media processing, or content management. You require Portable Operating System Interface (POSIX)-compliant file system access semantics and concurrently accessible storage. Which storage service must you use?
* [ ] Object Storage
* [ ] Block Storage
* [X] File Storage (*)
* [ ] Vault Storage

####    Which gateway allows resources within a VCN to communicate with the Internet but prevents any inbound traffic?
* [ ] Service gateway
* [ ] Internet gateway
* [ ] Dynamic routing gateway
* [X] NAT gateway (*)
####    Which three statements about compartments are true?
* [ ] You cannot control the type of resources that can be created within a compartment.
* [ ] Multiple compartments can share a single resource.
* [X] Compartments can be nested. (*)
* [X] You can set a budget on a compartment so that you are notified as soon as the budget is exceeded. (*)
* [X] One compartment can have resources from multiple regions. (*)

####    Which OCI networking method must you use to divide your network into multiple VCNs based on departments, with each VCN having direct, private access to the others while avoiding traffic flowing over the Internet or through your on-premises network?
* [ ] FastConnect
* [ ] NAT gateway
* [X] VCN peering (*)
* [ ] Site-to-Site VPN
####    Which two statements about local VCN peering are true?
* [ ] The two VCNs must have overlapping CIDRs.
* [X] You can use a single DRG for local peering. (*)
* [X] The VCNs can be in different Oracle Cloud Infrastructure tenancies but in the same region. (*)
* [ ] It uses an Internet gateway.
####    You have two objects in a bucket: Object X and Object Y. Object X was last modified 14 months ago and Object Y was last modified 3 months ago. You create a retention rule with a duration of 1 year. Which two statements are true?
* [X] Object Y cannot be modified or deleted for the next 9 months. (*)
* [ ] Object X cannot be modified or deleted for the next 2 months.
* [ ] Object Y can be modified or deleted immediately.
* [X] Object X can be modified or deleted immediately. (*)
####    Which two statements about boot volumes are true?
* [ ] You cannot group boot volumes with block volumes into the same volume group
* [ ] When you terminate your instance, you can keep the associated boot volume and use it to launch a new instance, but it must be of the same shape and size as the original instance.
* [X] When you terminate the instance, you can preserve the boot volume and its data. (*)
* [X] When you launch a virtual machine (VM) or bare metal instance based on a platform image or custom image, a new boot volume for the instance is created in the same compartment. (*)
####    Which policy is automatically applied when you create a cloud account?
* [ ] Allow Group Administrator to manage all-resources in all-domains
* [ ] Allow Group Administrator to manage all-resources in all-compartments
* [X] Allow Group Administrator to manage all-resources in tenancy (*)
* [ ] Allow Group Administrator to manage all-resources in regions
####    Which two statements about auth tokens are true?
* [ ] They expire after 14 days by default.
* [ ] They make use of a public key/private key pair.
* [X] Every user can generate up to two auth tokens. (*)
* [X] They can be used to authenticate third-party APIs. (*)
####    Which Oracle-defined backup policy includes weekly incremental backups that run on Sundays, monthly incremental backups that run on the first day of the month and, also includes incremental backups that run annually during the first part of January and are retained for five years?
* [ ] Bronze policy
* [ ] Gold policy
* [ ] Platinum policy
* [X] Silver policy (*)
####    Examine this policy-Allow group GroupMgr to manage volumes in tenancy where request.permission != 'VOLUME_DELETE', Which three actions can a user belonging to the GroupMgr group perform?
* [X] Update volumes. (*)
* [ ] Delete volumes.
* [X] Move volumes. (*)
* [X] Create volumes. (*)
####    Which network security service allows you to separate the VCN's subnet architecture from your application security requirements?
* [X] Network security groups (*)
* [ ] Flow logs
* [ ] Security lists
* [ ] Access control
####    At which level are retention rules configured in the Object Storage service?
* [ ] Object level
* [X] Bucket level (*)
* [ ] Compartment level
* [ ] Namespace level
####    For maximum cost efficiency, when launching compute instances, which capacity type must you select for workloads that run periodically or for short periods of time and don't require continuous availability?
* [ ] On-demand capacity
* [X] Preemptible capacity (*)
* [ ] Dedicated host
* [ ] Capacity reservation
####    Which three components are managed by the customer and not by Oracle in a shared security model of OCI?
* [X] Data (*)
* [X] Accounts and identities (*)
* [ ] Physical hosts
* [X] Application (*)
* [ ] Physical networks
####    When triggered, an alarm sends an alarm message to the configured topic. In which service is the topic configured?
* [X] Notifications (*)
* [ ] Management
* [ ] Synchronization
* [ ] Monitoring
####    What is the allowable VCN size range?
* [ ] /8 through /16
* [ ] /8 through /24
* [ ] /0 through /32
* [X] /16 through /30 (*)
####    An instance running in a development compartment needs to make API calls to other OCI services. How can you achieve this without configuring user credentials or setting up a configuration file?
* [ ] Create a dynamic group with matching rules to include your instance.
* [X] Create a dynamic group with matching rules to include your instance and write a policy for this dynamic group. (*)
* [ ] Instances can automatically make calls to other OCI services; hence, no configuration is needed.
* [ ] The requirement cannot be achieved by configuring user credentials or setting up a configuration file.
####    You have enabled versioning for a bucket. What happens when you upload an object with the same name as an existing object?
* [ ] The existing object is moved to a different bucket which has been marked for archival.
* [ ] The object is overwritten and the overwritten object is not retained or recoverable.
* [ ] It returns an error.
* [X] The existing object becomes a previous version and the newly uploaded object becomes the latest version. (*)
####    Which two connectivity options can you use to give your virtual cloud network (VCN) access to the Internet?
* [ ] Service gateway
* [X] NAT gateway (*)
* [X] Internet gateway (*)
* [ ] FastConnect
####    Which two statements about Compute Autoscaling are true?
* [ ] Metric-based autoscaling relies on performance metrics that are collected by the Tracking service.
* [ ] For autoscaling to work, you must configure a load balancer.
* [X] An autoscaling configuration can include one or more autoscaling policies. (*)
* [X] Each instance pool can have only one autoscaling configuration. (*)
####    What happens to traffic if there is no route rule that matches the network traffic you intend to route outside the VCN?
* [ ] It is sent over FastConnect.
* [X] It is dropped. (*)
* [ ] It is sent over the Internet gateway.
* [ ] It is sent over the NAT gateway.
####    You want a specific set of users, who do not have IAM user credentials, to access a bucket for a duration of two days. Which mechanism can help you achieve this?
* [ ] Creating an auto config file
* [ ] Converting the bucket to a public bucket
* [ ] Moving the bucket to an archive tier
* [X] Creating pre-authenticated requests (*)
####    Which two statements about application-based load balancers are true?
* [ ] They act only on the TCP layer variables.
* [ ] They are based on IP address and destination ports only.
* [X] They perform content-based routing. (*)
* [X] They support both HTTP and HTTPS. (*)
####    Which Object Storage tier would you use for data that you need to access quickly, immediately, and frequently?
* [ ] High Performance tier
* [X] Standard tier (*)
* [ ] Archive tier
* [ ] Ultra High Performance tier
* [ ] Infrequent Access tier
####    When you create a block volume, what is its default performance level?
* [X] Balanced (*)
* [ ] Lower Cost
* [ ] Ultra High Performance
* [ ] Higher Performance
####    When you enable Auto-Tiering, objects larger than 1 MiB are automatically moved from the Standard tier to which tier?
* [ ] Archive tier
* [X] Infrequent Access tier (*)
* [ ] Backup tier
* [ ] Redundancy tier
####    Which Traffic Management Steering policy distributes DNS traffic to different endpoints based on the location of the end user?
* [ ] ASN steering
* [X] Geolocation steering (*)
* [ ] IP prefix steering
* [ ] Load balancer
####    Which type of logs are emitted by API gateways, Events, and Object Storage?
* [X] Service logs (*)
* [ ] Custom logs
* [ ] Audit logs
* [ ] Archive logs
####    Which three encryption algorithms are supported by OCI Vault?
* [ ] IDEA
* [X] AES (*)
* [X] ECDSA (*)
* [X] RSA (*)
* [ ] HMAC
####    Which protocol is used by FastConnect?
* [ ] IPSec
* [X] BGP (*)
* [ ] OSPF
* [ ] DNS routing
####    Which OCI security service can you use to ensure that unwanted bots are mitigated while desirable bots are allowed to enter?
* [ ] Data Vault
* [X] Web Application Firewall (*)
* [ ] Cloud Guard
* [ ] Security Zone
####    Which two statements about a block volume clone are true?
* [X] It creates a single point-in-time copy of a volume without having to go through the backup and restore process. (*)
* [ ] It makes use of Object Storage.
* [X] You can clone a volume group. (*)
* [ ] It is slower than a block volume backup.
####    Which block volume performance level is recommended for throughput-intensive workloads with large sequential I/O, such as streaming, log processing, and data warehouses?
* [ ] Balanced
* [ ] Ultra High Performance
* [X] Lower Cost (*)
* [ ] Higher Performance
####    Which two statements about Object Storage are true?
* [X] It supports private access from Oracle Cloud Infrastructure resources in a VCN through a service gateway. (*)
* [ ] You can back up a DB system to Object Storage only via the Internet.
* [X] It is a regional service and is not tied to any specific compute instance. (*)
* [ ] Archive is the default tier for Object Storage buckets.
####    Which two statements about cloning a file system are true?
* [X] You can only create a clone in the same availability domain as its parent file system. (*)
* [ ] You can clone a parent file system, but you cannot create a clone of a clone.
* [X] File system properties, such as compartment, tags, display name, keys, and mount target export information, are not copied over from the parent. (*)
* [ ] You can also create a clone in a different availability domain to its parent file system.
####    You want to forbid the creation of public buckets in Object Storage. Which OCI security service can you use to achieve this?
* [ ] Web Application Firewall
* [ ] Vault
* [ ] Service Mesh
* [X] Security Zones (*)
####    Which two statements about security lists are true?
* [ ] Each subnet can have only one security list associated with it.
* [ ] They are applied to a group of VNICs of your choice instead of all the VNICs in a given subnet.
* [X] The default security list does not include a rule to allow ping requests. (*)
* [X] The default security list allows TCP traffic on destination port 22 (SSH) from authorized source IP addresses and any source port. (*)
####    Which two statements about private IP objects are true?
* [ ] Each instance receives a primary private IP object and a secondary private IP object at launch.
* [ ] Secondary private IPs must be manually deleted when you terminate the mapped instance.
* [X] You can add a secondary private IP to either the primary VNIC or a secondary VNIC of an instance after it's launched. (*)
* [X] A private IP can have a public IP assigned to it. (*)
####    What is used to specify the actions that Cloud Guard can take when detectors identify problems?
* [X] Responder (*)
* [ ] Alarms
* [ ] Metrics
* [ ] Threshold
####    You want users of the NetworkAdmins group to manage a cloud network in any compartment of a tenancy. What must you allow the NetworkAdmins group to do?
* [X] Manage virtual-network-family in tenancy. (*)
* [ ] Manage network-catalog-listing in tenancy.
* [ ] Use virtual-network-family in compartment XYZ.
* [ ] Manage instance-family in compartment ABC.
####    Which four layers of access control are used by the File Storage service?
* [X] NFS v.3 UNIX security (*)
* [ ] Key management
* [X] Network security (*)
* [ ] Web Application Firewall
* [X] NFS export option (*)
* [X] Oracle Cloud Infrastructure (OCI) policy (*)
* [ ] OCI Vault
####    Which two statements about Site-to-Site VPN are true?
* [ ] You cannot use multiple site-to-site connections between your on-premises network and virtual cloud network (VCN).
* [X] It provides a site-to-site IPSec connection between your on-premises network and your virtual cloud network (VCN). (*)
* [ ] The communication between the source and destination sites is unencrypted.
* [X] It encrypts IP traffic before the packets are transferred from the source to the destination and decrypts the traffic when it arrives. (*)










####    More Questions  ####

####    Which resource do you manage in an lnfrastructure-as-a-service (laaS) offering?
* [X] Operating System
* [ ] Server
* [ ] Networking
* [ ] Storage

####   What does compute instance vertical scaling mean?
 * [ ] Adding additional compute instances
 * [ ] Providing Fault tolerance
 * [X] Changing to a larger or smaller shape
 * [ ] Enabling Disaster recovery

 ####   Which Oracle Cloud lnfrastructure capability can be used to protect against power failures within an Availability Domain?
 * [ ] Data Plane
 * [ ] Service Cells
 * [ ] Top of Rack Switch
 * [X] Fault Domains

 ####   Which is Oracle's responsibility according to the Oracle Cloud lnfrastructure (OCI) shared security model?
* [ ] Configuring OCI services securely
* [X] Security of data-center facilities
* [ ] Securing application workloads
* [ ] Data classification and compliance

####    Which kind of scalling is supported by vitual machine in Oracle Cloud Infrastructure?
* [ ] Only scalling up or down
* [ ] Only scalling out
* [X] Scalling up or down, and scalling in or out
* [ ] Only scalling in

####    Which statement below is not true for Oracle Cloud lnfrastructure compartments?
* [ ] Resources can be moved from one compartment to another
* [X] Compartments cannot be nested
* [ ] Resources and compartments can be added and deleted anytime
* [ ] Each OCI resource belongs to a single compartment

####    Which Oracle Cloud Infrastructure Identity and Access Management capability helps you to categorize multiple users into teams?
* [ ] Dynamic Groups
* [ ] Policies
* [X] Groups
* [ ] Users
* [ ] Principals

####    Which statement below is not recommended by Oracle?
* [ ] Create resources inside compartments
* [ ] Create users and add them into group
* [X] Create resources in the root compartment
* [ ] Adding policies to tenancy or compartment

####    Which of bellow are IAM components? (Choose 3)
* [ ] Regional Subnet
* [ ] Rules
* [X] Users
* [X] Policies
* [X] Dynamic Groups
* [ ] Compute Instances
* [ ] Virtual Cloud Network

####    Oracle Cloud Infrastructure Budgets can be set on which option?
* [X] Compartment
* [ ] Variables
* [ ] Regions
* [ ] Policies

####    What purpose does an Oracle Cloud lnfrastructure (OCI) NAT Gateway serve?
* [ ] Enables OCI compute instances to privately connect to OCI Object Storage
* [ ] Enables OCI compute instances to connect to the Internet
* [ ] Enables OCI compute instances to connect to on-premises environments
* [X] Enables OCI compute instances in a private subnet reach the Internet

####    You need to provide quickly a POC (proof of concept) between On-Premises and OCI. Which OCI services should you implement?
* [X] IPSec VPN
* [ ] FastConnect
* [ ] VCN Peering
* [ ] Internet Gateway

####    What purpose does an Oracle Cloud lnfrastructure (OCI) Dynamic Routing Gateway serve?
* [ ] Enables OCI compute instances to privately connect to OCI Object Storage
* [ ] Enables OCI compute instances to connect to the Internet
* [X] Enables OCI compute instances to connect to on-premises environments
* [ ] Enables OCI compute instances to be reached from the Internet

####    A customer wants to dedicated connection with minimal network latency from their on-premises data center to Oracle Cloud Infastructure (OCI). Which service should they choose?
* [X] OCI FastConnect
* [ ] IPSec Virtual Private Network
* [ ] Oracle Cloud Network Remote Peering
* [ ] Public Internet

####    Which OCI service would you use to distribute incoming traffic between a set of web servers?
* [ ] Internet Gateway
* [X] Public Load Balancer
* [ ] Autoscaling
* [ ] Private Load Balancer

####    You are running several Linux based operating systems in your on-premises environment that you want to import to OCI as custom images. You can launch your imported images as OCI compute Virtual Machines. Which TWO modes below can be used to launch these imported Linux VMs?
* [ ] Native
* [ ] Mixed
* [X] Paravirtualized
* [X] Emulated

####    What is TRUE regards to delete instance in OCI?
* [ ] The instance needs to be stopped first, and then terminated.
* [ ] The boot volume is always deleted.
* [ ] All block volumes attached to the instance are terminated.
* [X] Users can preserve the boot volume associated with the instance.

####    Which statement is correct regarding the oracle cloud infrastructure Compute services?
* [ ] You cannot attach a block volume to a compute instance
* [X] You can launch either virtual machines or bare metal instances
* [ ] You can attach a maximum of one public to each compute instance
* [ ] When you stop a compute instance, all data on the boot volume is lost

####    Which TWO resources reside exclusively in a single availability domain?
* [X] Compute instance;
* [ ] Object Storage;
* [ ] Groups;
* [X] Block Volume;
* [ ] Web Application Firewall Policy;

####    Which statement is TRUE for an oracle cloud Infrastructure (OCI) compute instance?
* [X] Compute instance always get a private IP address
* [ ] Compute instance cannot leverage auto scaling feature
* [ ] Compute instance always get a public IP address
* [ ] Compute instance does not use a boot volume

####    You have an application running on Oracle Cloud Infrastructure. You identified that the read and write operations are slowing your application down enough to impair user access. The application is currently using a VM.Standard1.2 compute without any block storage attached to it. Which TWO options allow you to increase disk performance? (Choose TWO.)
* [X] Terminate the compute instance preserving the boot volume. Create a new compute instance using a VM.DenseIO shape using the boot volume preserved.
* [X] Terminate the compute instance preserving the boot volume. Create a new compute instance using a VM Standard shape and attach a new block volume to host your application.
* [ ] Create a backup of the boot volume. Create a new compute instance using a VM Dense IO shape and restore the backup.
* [ ] Terminate the compute instance and create a backup of the boot volume. Create a new compute instance using a VM Dense IO shape and restore the backup.

####    Your on-premises hosted application uses Oracle database server. Your database administrator must have access to the database server for managing the application. Your database server is sized for seasonal peak workloads which results in high licensing costs. You want to move your application to Oracle Cloud Infrastructure (OCI) to take advantage of CPU scaling options. Which database offering on OCI would you select?
* [X] Bare Metal DB systems
* [ ] VM DB systems
* [ ] Autonomous Transactions Processing (ATP)
* [ ] Autonomous Data Warehouse (ADW)

####    Which TWO are a valid image source when launching a new compute instance? (Choose TWO.)
* [ ] Bare Metal instance
* [ ] Object Storage
* [X] Custom Image
* [X] Boot Volume

####    What characteristics are defined in an Oracle Cloud Infrastructure Compute shape?
* [ ] Number of vCPU, amount of LAN bandwidth.
* [ ] Public or private visibility of the Compute Instance
* [X] Number of OCPU, amount of LAN bandwidth
* [ ] Availability Domains and Fault Domains locations

####    You have deployed a compute instance (VM.Standard2.24) to run an Oracle database. With this set up, you run into some performance issues and want to leverage an OCI Dense IO shape (VM.DenseI02.24), with which you get 25.6 TB local NVMe SSD. You do not want to lose the configuration changes you made to the instance. Which of the following TWO steps ARE NOT required to make this transition?
* [X] Terminate the VM.Standard2.24 instance and do not preserve the boot volume.
* [ ] Create a new instance using the VM.DenseIO2.24 shape using the preserved boot volume and move the Oracle Database data to NVMe disks.
* [ ] Terminate the VM.Standard2.24 instance and preserve the boot volume.
* [X] Create a new instance using a VM.DenseI02.24 shape using the preserved boot volume and move the Oracle Database data to block volumes.

####    You deployed a compute instance (VM.Standard2.16) to run a SQL database. After a few weeks, you need to increase disk performance by using NVMe disks; the number of CPUs will not change. As a first step you terminate the instance and preserve the boot volume. What is the next step?
* [ ] Create a new instance using a VM.DenseIO2.16 shape using the preserved boot volume and move the SQL Database data to block volume.
* [ ] Create a new instance using a VM.DenseIO2.8 shape using the preserved boot volume and move the SQL Database data to NVMe disks.
* [ ] Create a new instance using a VM.Standard1.16 shape using the preserved boot volume and move the SQL Database data to NVMe disks.
* [X] Create a new instance using a VM.DenseIO2.16 shape using the preserved boot volume move the SQL Database data to NVMe disks.

####    Which TWO statements are true about restoring a block volume from a manual or policy based block volume backup?
* [X] It can be restored as new volumes with different sizes from the backups.
* [ ] It can be restored as a new volume to any AD across different regions.
* [ ] It must be restored as a new volume to the same availability domain (AD) on which the original block volume backup resides.
* [X] It can be restored as a new volume to any AD in the same region.

####    Which Oracle Cloud Infrastructure storage service can provide a shared file system across multiple compute instance?
* [ ] Local NVMe
* [ ] Object Storage
* [ ] Archive Storage
* [X] File Storage

####    A customer wants to use Oracle Cloud Infrastructure (OCI) for starring application backups which can be stored for months but retrieved immediately based on business needs. Which OCI storage service can be used to meet this requirement?
* [ ] Block volume
* [ ] Archive storage
* [X] Object storage (standard)
* [ ] File storage

####    What offers the lowest pricing for storage (per GB)?
* [X] Oracle Cloud Infrastructure Archive Storage
* [ ] Oracle Cloud Infrastructure block volume
* [ ] Oracle Cloud Infrastructure File Storage
* [ ] Oracle Cloud Infrastructure Object Storage (standard tier)

####    A customer is looking to migrate their old database backups from their on-premises data center to Oracle Cloud Infrastructure (OCI). Which OCI service is the most cost effective?
* [X] Archive Storage
* [ ] Object Storage
* [ ] Block Volume
* [ ] File Storage

####    Which service would you use if your big data workload required shared access and NFS-based connectivity?
* [ ] Block Volume
* [ ] Archive Storage
* [ ] Object Storage
* [X] File Storage

####    In what TWO ways does Oracle Cloud Infrastructure (OCI) File Storage Service differ from OCI Object Storage and Block Volume services?
* [ ] File storage mount target does not provide a private IP address, while the object storage bucket provides one.
* [X] File Storage uses the network file system (NFS) protocol, whereas block volume uses ISCSI.
* [ ] Block volume service is NVMe based, while file storage service is not.
* [X] You can move object storage buckets, block volumes and file storage mount targets between compartments

####    You have multiple applications installed on a compute Instance and these applications generate a large amount of log files. These log files must reside on the boot volume for a minimum of 15 days. Any files over 15 days do not have to reside on boot volume but still must be retained for at least 60 days. The 60-day retention requirement is causing an issue with available disk space. What are the TWO recommended methods to provide additional boot volume space for this compute instance?
* [ ] Terminate the instance while preserving the boot volume. Create a new instance from the boot volume and select a DenseIO shape to take advantage of local NVMe storage.
* [X] Create an object storage bucket and use a script that runs daily to move log files older than 15 days to the bucket.
* [ ] Create and attach a block volume to the compute instance and copy the log files.
* [X] Create a custom image and launch a new compute instance with a larger boot volume size.
* [ ] Write a custom script to remove the log files on a daily basis and free up the space on the boot volume.

####    You are designing a lab exercise for your team that has a large number of graphics with large file sizes. The application becomes unresponsive if the graphics are embedded in the application. You have uploaded the graphics to Oracle Cloud Infrastructure and only added the URL in the application. You need to ensure these graphics are accessible without requiring any authentication for an extended period of time. How can you achieve these requirements?
* [ ] Create pre-authenticated requests (PAR) and specify 00:00:0000 as the expiration time.
* [ ] Make the object storage bucket private and all objects public and use the URL found in the Object "Details".
* [X] Make the object storage bucket public and use the URL found in the Object "Details".
* [ ] Create pre-authenticated requests (PAR) and do not specify an expiration date.

####    Your organization has deployed a large, complex application across multiple compute instances in Oracle Cloud Infrastructure (OCI). These compute instances also have block volume storage attached to them. You want to create a time consistent backup of this block volume storage. Which implementation strategy should be used?
* [ ] Create a manual backup of each volume.
* [ ] Use scripts available in OCI to backup block volume storage.
* [ ] Group volumes in a volume group first and then use available scripts in OCI.
* [X] Group volumes in a volume group and create a manual backup of the volume group.

####    You are about to deploy an e-business application on Oracle Cloud Infrastructure and one of the requirements is to use a shared file system that supports the NFS protocol. Which storage service would meet this requirement?
* [ ] Object Storage
* [ ] Block Volume
* [ ] Data Transfer appliance
* [X] File Storage

####    Which TWO statements are true about an Oracle Cloud Infrastructure object storage bucket? (Choose TWO.)
* [ ] You can associate a bucket with multiple compartments.
* [ ] You cannot change a bucket from private to public after it is created.
* [X] You can associate a bucket with only a single compartment.
* [X] You cannot edit or append data to an object, but you can replace the entire object.

####    What is a valid option when exporting a custom image?
* [X] Object Storage URL
* [ ] Archive Storage URL
* [ ] File Storage service
* [ ] Block Volume

####    You have one database style application that frequently makes many random reads and writes across the dataset. Which storage offering supports this application?
* [X] Block Volume service
* [ ] File Storage service
* [ ] Object Storage service
* [ ] Archive storage service

####    You are designing a shared storage solution for your company in Oracle Cloud Infrastructure. The proposed storage solution should allow users to create a hierarchical structure (similar to the directory structure in Linux or Windows based systems). The solution should provide data encryption and a large amount of storage space. Which would be the best implementation strategy?
* [ ] Use block storage. Create and attach a large block storage volume to one compute instance. Assign a public IP to the compute instance. Store data on the block storage and access it by connecting to the compute instance.
* [ ] Use object storage. Create a single namespace and multiple buckets to create the hierarchical directory structure.
* [ ] Use object storage. Create multiple namespaces with one bucket each. Make the buckets publicly accessible.
* [X] Use file storage service. Create a file system and a mount target. Share the private IP of the mount target.

####    You have provisioned an Autonomous Transaction Processing (ATP) database and logged into the ATP service console. What are three abilities that can be performed from this service console? (Choose THREE).
* [ ] Scale up/down the CPUs
* [ ] Create ATP database users
* [X] Reset the admin password
* [X] Set resource management rules
* [X] Monitor database activity and SQL queries

####    What is a key benefit of Oracle Cloud Infrastructure Virtual Machine DB Systems?
* [ ] Automated Database Memory
* [ ] Automated backups to OCI Block Volumes
* [X] Support for RAC DB systems/Fast Provisioning/ Scale up Block Storage Anytime
* [ ] You need to create virtualization

####    You want to leverage a managed Real Application Cluster (RAC) offering in Oracle Cloud Infrastructure. which OCI Managed database service would you choose?
* [ ] Autonomous Transaction Processing (shared)
* [ ] Autonomous Data Warehousing (shared)
* [X] VM DB Systems
* [ ] Bare Metal DB Systems

####    Which of the following TWO tasks can be performed in the Oracle Cloud Infrastructure Console for Autonomous Data Warehouse?
* [ ] Adjust Network Bandwidth
* [ ] Scale up/down Memory
* [X] Increase Storage allocated for Database
* [X] Scale up/down CPU

####    Which TWO Oracle Cloud Infrastructure database services allow you to dynamically scale CPU and storage?
* [ ] Bare metal DB system
* [ ] Virtual machine DB system
* [X] Autonomous Data Warehouse (ADW)
* [X] Autonomous Transaction Processing (ATP)
####    Which SLA types is not offered by Oracle Cloud lnfrastructure compute service?
* [X] Service Plane
* [ ] Control Plane 
* [ ] Data Plane
* [ ] Performance
####    Which TWO OCI resources can be used to group expenses?
* [X] Tags
* [ ] Users
* [ ] Policies
* [ ] Groups
* [X] Compartmens
####    Which TWO situations incur costs within Oracle Cloud lnfrastructure?
* [ ] Transferring data from one instance to another within the same Availability Domain
* [ ] Transferring data from one instance to another across different Availability Domains in a region
* [X] Transferring data across regions
* [X] Data egress to the Internet
####    Which security service is offered by Oracle Cloud lnfrastructure?
* [X] Key Management
* [ ] Managed Active Directory
* [ ] Managed lntrusion Detection
* [ ] Certificate Management System
####    Which is not considered security resource within Oracle Cloud Infrastructure (OCI)?
* [ ] Web Application Firewall
* [ ] Security Rules
* [X] File Storage Services
* [ ] Network Security Groups












#### Patric Test OCI 2023 Architect Associate 1Z0-1072-23   ####

####    You are part of a team that manages a set of workload instances running in an on-premises environment. The Architect team is tasked with designing and configuring Oracle Cloud Infrastructure (OCI) Logging service to collect logs from these instances. There is a requirement to archive Info-level logging data of these instances into the OCI Object Storage. Which TWO features of OCI can help you achieve this?
* [X] Service Connectors
* [ ] Grouping Function
* [X] Agent Configuration
* [ ] ObjectCollectionRule
* [ ] Cloud Agent Plugin

####    You plan to launch a VM instance with the VM.Standard2.24 shape and Oracle Linux 8 platform image. You want to protect your VM instance from low-level threats, such as rootkits and bootkits that can infect the firmware and operating system and are difficult to detect.
* [ ] Create a burstable instance
* [ ] Use in-transit encryption
* [X] Create a shielded instance
* [ ] Use Vulnerability Scanning Service

####    What security consideration should you be mindful of before performing a database migration?
* [ ] Migration can only be done in the web-based interface of Oracle
* [ ] Encrypt all files that are used for migration
* [X] Backup and restore your TDE wallets from the source to the target database
* [ ] Place the database in the restricted mode so that no one accesses it during migration

####    A few Object Storage buckets in your Oracle Cloud Infrastructure (OCI) tenancy should remain public, and yet you do not want the Cloud Guard service to detect these as problems. In which TWO ways would you address this requirement?
* [ ] Cloud Guard will keep detection ot because a public bucket is a security risk
* [X] Dismiss the problems associated with those resources
* [ ] Resolve or remediate those problems and you should not see Cloud Guard triggering on the resources ever again
* [X] Fix the base line by configuring Conditional Groups for the detector

####    You plan to upload a large file (3 TiB) to Oracle Cloud Infrastructure (OCI) Object Storage. You would like to minimize the impact of network failures while uploading, and therefore you decide to use the multipart upload capability. Which TWO statements are true about performing a multipart upload using the Multipart Upload API?
* [X] When you split the object into individual parts, each part can be as large as 50 GiB
* [ ] You do not need to split the object into parts. Object Storage splits the object into parts and uploads all of the parts automatically
* [X] While a multipart upload is still active, you can keep adding parts as long as the total number is less than 10,000
* [ ] You do not have to commit the uploaded all the object parts

####    You need to implement automatic backups for your database system. You can easily check “Enable Automatic Backup” in the web console. Before you do that though, you need to have which of the following TWO prerequisites in place?
* [ ] Private SSH Key to the database
* [X] Access to the OCI Object Storage service
* [X] Connectivity to Swift endpoints
* [ ] VCN configured with VPN for secure access to the Oracle Cloud Infrastructure (OCI) Object Storage service

####    Which THREE protocols are supported by the Oracle Cloud Infrastructure (OCI) Network Load Balancer?
* [ ] HTTP
* [X] TCP
* [X] ICMP
* [X] UDP
* [ ] iSCSI
* [ ] BGP

####    Which of the following statements is true about cloning a volume in the Oracle Cloud Infrastructure (OCI) Block Volume service?
