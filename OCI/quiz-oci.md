
####    20: Security-Operations
####    Maximum Security Zone is a custom recipe created by the user to fit their specific needs.
* [X] Security Zones provide active enforcement of resource-based security policies to prevent security misconfigurations. (*)
* [ ] Custom Security Zone policy sets are predefined templates that cannot be modified.
* [ ] Security Zones can only be used to monitor the security posture of infrastructure and applications.

####    Which option accurately describes the primary purpose of the Cloud Event rule in the Responder recipe of Oracle Cloud Guard?
* [ ] Configuring service level IAM policies for Cloud Guard
* [ ] Attaching the Responder recipe to a corresponding target or targets
* [X] Emitting problem details to the Events service for notifications (*)
* [ ] Disabling a detected problem within the target

####    you want to restrict users from creating public buckets in Object Storage and if some user tries to create they should receive an error message. What would you use to configure this?
* [ ] Cloud Advisor
* [ ] Security Advisor
* [X] Security Zone (*)
* [ ] Cloud Guard
* [ ] Data Safe

####    Which three are a customer's responsibilities in the shared responsibilities model for security?
* [ ] Hypervisor security
* [X] Data classification and compliance (*)
* [X] Client and endpoint protection (*)
* [X] Patching operating systems of compute instances (*)
* [ ] Physical security

####    You would like to examine your resources for security weakness related to configuration and upon detection suggest, assist, or take corrective actions. Which Oracle Cloud Infrastructure (OCI) security service should you use?
* [ ] OCI Certificates
* [X] Cloud Guard (*)
* [ ] Vault 
* [ ] Audit 

####    22: Security-Platform

####    Which OCI Security service protects web applications and APIs from common web exploits that can affect availability or security?
* [X] OCI Web Application Firewall (*)
* [ ] OCI Threat Intelligence
* [ ] OCI Security Zones
* [ ] OCI Network Firewall

####    Which of the following statements best explains why a dynamic group is needed for Certificate Authority creation in OCI Certificates service?
* [X] A dynamic group is necessary to allow the Certificate Authority to make API calls to Vault or Object Storage services. (*)
* [ ] A dynamic group is not necessary for creating a Certificate Authority.
* [ ] A dynamic group is necessary to create TLS certificates after the Certificate Authority is created.
* [ ] A dynamic group is necessary to manage the Certificate Authority's revocation list.

####    What is the purpose of the Vulnerability Scanning service in Oracle Cloud Infrastructure?
* [ ] To perform network scans of all public-facing IPs on the targeted instances
* [X] To identify and prioritize vulnerabilities in OCI compute instances and containers (*)
* [ ] To provide remediation actions for customers to address vulnerabilities
* [ ] To scan and report on the health of OCI compute instances and containers

####    Which type of rule do you need to configure in OCI WAF to protect your web applications from various types of threats like SQL injection, cross-site scripting, and HTML injection?
* [ ] Rate limiting rule
* [X] Protection rule (*)
* [ ] Access control rule
* [ ] Bot management

####    Which of the following can you do using Oracle Cloud Infrastructure Certificates service?
* [ ] Import certificates issued by a third-party CA.
* [ ] Create and manage certificate authorities (CAs), certificates, and CA bundles.
* [X] All of the above (*)
* [ ] Configure rules to automatically renew certificates.

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