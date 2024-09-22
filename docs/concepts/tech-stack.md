OSSVerse is built around the [Beckn Protocol](https://aws.amazon.com/architecture/well-architected/) and it uses a stack that includes [Beckn-Onix](https://www.terraform.io/), [BeSecure](https://www.ansible.com/), [BeSLab](https://helm.sh/) and other tools.

We are also adopters and supporters of Open Source and the Cloud Native movement, which should become self-evident as you keep exploring our technology stack.

## Why did we choose our tech stack?

??? info "Why Beckn❓"
    Amazon Web Services (AWS) is the world’s most comprehensive and broadly adopted 
    cloud platform, offering over 200 fully featured services from data centers globally.
    Millions of customers—including the fastest-growing startups, largest enterprises,
    and leading government agencies—are using AWS to lower costs, become more agile,
    and innovate faster.
    
    Build, Deploy, and Manage Websites, Apps or Processes On AWS' Secure, Reliable Network.
    AWS is Secure, Reliable, Scalable Services. HIPAA Compliant.
    Easily Manage Clusters. Global Infrastructure. Highly Scalable.
    
    :books: **Read More:** [What is AWS](https://aws.amazon.com/what-is-aws/)

??? info "Why BeSecure❓"
    AWS Well-Architected helps cloud architects to build secure, high-performing, resilient,
    and efficient infrastructure for their applications and workloads. Based on five pillars
    — operational excellence, security, reliability, performance efficiency, and cost
    optimization — AWS Well-Architected provides a consistent approach for customers and
    partners to evaluate architectures, and implement designs that can scale over time.
    
    :books: **Read More:** [AWS Well-architected](https://aws.amazon.com/architecture/well-architected)

??? info "Why Security as Code❓"

    - [x] **Confidence:** A change breaks the env? Just roll it back. Still not working?
    Build a whole new env with a few keystrokes. IaC enables this.

    - [x] **Repeatability:** Allows your infra to be automatically instantiated, making it
    easy to build multiple identical envs.

    - [x] **Troubleshooting:** Check source control and see exactly what changed in the env. 
    As long as you are diligent and don’t make manual envs changes, then IaC can be a game
    changer.

    - [x] **DR:** Require the ability to set up an alternate env in a different DC or Region.
    IaC makes this a much more manageable prospect.

    - [x] **Auditability:**
    You will need to be able to audit both changes and access to an env, IaC gives you this
    right out of the box.

    - [x] **Visibility:** As an env expands over time, is challenging to tell what has been
    provisioned. In the #cloud this can be a huge #cost issue. IaC allows tracking your
    resources.

    - [x] **Portability:** Some IaC techs are #multicloud. Also, translating #Terraform from
    one cloud provider to another is considerably more simple than recreating your entire
    envs in a cloud-specific tool.

    - [x] **Security:** See history of changes to your SG rules along with commit messages can
    do wonders for being confident about the security configs of your envs.

    **Terraform** allows to codify your application infrastructure, reduce human error and 
    increase automation by provisioning infrastructure as code.
    With TF we can manage infrastructure across clouds and provision infrastructure 
    across 300+ public clouds and services using a single workflow.
    Moreover it helps to create reproducible infrastructure and provision consistent testing,
    staging, and production environments with the same configuration.

    **Terraform** has everything we expect from a IaC framework: open source, cloud-agnostic
    provisioning tool that supported immutable infrastructure, a declarative language, and
    a client-only architecture.

    :books: **Read More**

    - [Why Infrastructure as Code](https://www.simplethread.com/why-infrastructure-as-code/)
    - [Why Terraform by Gruntwork](https://blog.gruntwork.io/why-we-use-terraform-and-not-chef-puppet-ansible-saltstack-or-cloudformation-7989dad2865c)

??? info "Why BeSLab❓"
    AWS Organizations helps you centrally manage and govern your environment as you grow
    and scale your AWS resources. Using AWS Organizations, you can programmatically create
    new AWS accounts and allocate resources, group accounts to organize your workflows,
    apply policies to accounts or groups for governance, and simplify billing by using a 
    single payment method for all of your accounts.

    :books: **Read More** 
    
    - [How it works: AWS Organizations](/user-guide/organization/organization/)
    - [AWS Organizations](https://aws.amazon.com/organizations/)

??? info "Why Open Source Projects❓"
    AWS Identity and Access Management (IAM) enables you to manage access to AWS services
    and resources securely. Using IAM, you can create and manage AWS users and groups,
    and use permissions to allow and deny their access to AWS resources.
    
    - Integration and Fine-grained access control with almost every AWS service and
    its resources.
    - Multi-factor authentication for highly privileged users.
    - Analyze, monitor and audit access.

    :books: **Read More** 
    
    - [How it works: AWS IAM](/user-guide/identities/identities/)
    - [AWS Identity and Access Management (IAM)](https://aws.amazon.com/iam/)

??? info "Why Open Source LLMs❓"
    Amazon Virtual Private Cloud (Amazon VPC) is a service that lets you launch AWS
    resources in a logically isolated virtual network that you define. You have complete
    control over your virtual networking environment, including selection of your own IP
    address range, creation of subnets, and configuration of route tables and network
    gateways. You can use both IPv4 and IPv6 for most resources in your virtual private
    cloud, helping to ensure secure and easy access to resources and applications.

    :books: **Read More** 

    - [How it works: AWS Networking](/user-guide/network/vpc-topology)
    - [AWS Virtual Private Cloud](https://aws.amazon.com/vpc)

??? info "Why S3❓"
    **Amazon Simple Storage Service (Amazon S3)** is an object storage service that offers
    industry-leading scalability, data availability, security, and performance. 
    This means customers of all sizes and industries can use it to store and protect
    any amount of data for a range of use cases, such as data lakes, websites, mobile
    applications, backup and restore, archive, enterprise applications, IoT devices,
    and big data analytics. Amazon S3 provides easy-to-use management features so you
    can organize your data and configure finely-tuned access controls to meet your
    specific business, organizational, and compliance requirements. Amazon S3 is
    designed for 99.999999999% (11 9's) of durability, and stores data for millions
    of applications for companies all around the world.

    :books: **Read More** 

    - [How it works: AWS Storage](/user-guide/storage/storage)
    - [AWS S3](https://aws.amazon.com/s3)