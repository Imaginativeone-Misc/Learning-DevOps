# Learning DevOps

## Beginning Info

- Table of Contents
- Preface
- Who this book is for
- What this book covers
- To get the most out of this book
- Download the example code files
- Download the color images
- Code in Action
- Conventions used
- Get in touch
- Reviews
## Section 1: DevOps and Infrastructure as Code
- [ ] Chapter 01: DevOps Culture and Practices
  - [ ] Getting started with DevOps
  - [ ] Implementing CI/CD and continuous deployment
  - [ ] Continuous integration (CI)
  - [ ] Implementing CI
  - [ ] Continuous delivery (CD)
  - [ ] Continuous deployment
  - [ ] Understanding IaC practices
  - [ ] The benefits of IaC
  - [ ] IaC languages and tools
  - [ ] Scripting types
  - [ ] Declarative types
  - [ ] The IaC&#xA0;topology
  - [ ] The deployment and provisioning of the infrastructure
  - [ ] Server configuration
  - [ ] Immutable infrastructure with containers
  - [ ] Configuration and deployment in Kubernetes
  - [ ] IaC best practices
  - [ ] Summary
  - [ ] Questions
  - [ ] Further reading
- [ ] Provisioning Cloud Infrastructure with Terraform
Technical requirements
Installing Terraform
Manual installation
Installation by script
Installing Terraform by script on&#xA0;Linux
Installing Terraform by script on Windows
Installing Terraform by script on macOS
Integrating Terraform with Azure Cloud Shell
Configuring Terraform for Azure
Creating the Azure SP
Configuring the Terraform provider
Terraform configuration for local development and testing
Writing a Terraform script to deploy Azure infrastructure
Following some Terraform good practices
Better visibility with the separation of files
Protection of sensitive data
Dynamizing the code with variables and interpolation functions
Deploying the infrastructure with Terraform
Initialization
Previewing changes
Applying the changes
Terraform command lines and life cycle
Using destroy to better rebuild
Formatting and validating the code
Formatting the code
Validating the code
Terraform's life cycle in a CI/CD process
Protecting tfstate in a remote backend
Summary
Questions
Further reading
Using Ansible for Configuring IaaS Infrastructure
Technical requirements
Installing Ansible
Installing Ansible with a script
Integrating Ansible into Azure Cloud Shell
Ansible artifacts
Configuring Ansible
Creating an inventory for targeting Ansible hosts
The inventory file
Configuring hosts in the inventory
Testing the inventory
Writing the first playbook
Writing a basic playbook
Understanding Ansible modules
Improving your playbooks with roles
Executing Ansible
Using the preview or dry run option
Increasing the log level output
Protecting data with Ansible Vault
Using variables in Ansible for better configuration
Protecting sensitive data with Ansible Vault
Using a dynamic inventory for Azure infrastructure
Summary
Questions
Further reading
Optimizing Infrastructure Deployment with Packer
Technical requirements
An overview of Packer
Installing Packer&#xA0;
Installing manually&#xA0;
Installing by script
Installing Packer by script on Linux
Installing Packer by script on Windows
Installing Packer by script on macOS
Integrating Packer with Azure Cloud Shell
Checking the Packer installation
Creating Packer templates for Azure VMs with scripts
The structure of the Packer template
The builders section
The provisioners section
The variables section
Building an Azure image with the Packer template
Using Ansible in a Packer template
Writing the Ansible playbook
Integrating an Ansible playbook in a Packer template
Executing Packer&#xA0;
Configuring Packer to authenticate to Azure
Checking the validity of the Packer template
Running Packer to generate our VM image
Using a Packer image with Terraform
Summary
Questions
Further reading
Section 2: DevOps CI/CD Pipeline
Managing Your Source Code with Git
Technical requirements
Overviewing Git and its command lines
Git installation
Configuration Git
Git vocabulary
Git command lines
Retrieving a remote repository
Initializing a local repository
Configuring a local repository
Adding a file for the next commit
Creating a commit
Updating the remote repository
Synchronizing the local repository from the remote
Managing branches
Understanding the Git process and GitFlow pattern
Starting with the Git process
Creating and configuring a Git repository
Committing the code
Archiving on the remote repository
Cloning the repository
The code update
Retrieving updates
Isolating your code with branches
Branching strategy with GitFlow
The GitFlow pattern
GitFlow tools
Summary
Questions
Further reading
Continuous Integration and Continuous Delivery
Technical requirements
The CI/CD principles
Continuous integration (CI)
Continuous delivery (CD)
Using a package manager
Private NuGet and npm repository
Nexus Repository OSS
Azure Artifacts
Using Jenkins
Installing and configuring&#xA0;Jenkins
Configuring a GitHub webhook
Configuring a Jenkins CI job
Executing the Jenkins job
Using Azure Pipelines
Versioning of the code with Git in Azure Repos
Creating the CI pipeline
Creating the CD pipeline: the release
Using GitLab CI
Authentication at GitLab
Creating a new project and managing your code source
Creating the CI pipeline
Accessing the CI pipeline execution details
Summary
Questions
Further reading
Section 3: Containerized Applications with Docker and Kubernetes
Containerizing Your Application with Docker
Technical requirements
Installing Docker
Registering on Docker Hub
Docker installation
An overview of Docker's elements
Creating a Dockerfile
Writing a Dockerfile
Dockerfile instructions overview
Building and running a container on a local machine
Building a Docker image
Instantiating a new container of an image
Testing a container locally
Pushing an image to Docker Hub
Deploying a container to ACI with a CI/CD pipeline
The Terraform code for ACI
Creating a CI/CD pipeline for the container
Summary
Questions
Further reading
Managing Containers Effectively with Kubernetes
Technical requirements
Installing Kubernetes
Kubernetes architecture overview
Installing Kubernetes on a local machine
Installing the Kubernetes dashboard
First example of Kubernetes application deployment
Using HELM as a package manager
Using AKS
Creating an AKS service
Configuring kubectl for AKS
Advantages of AKS
Creating a CI/CD pipeline for Kubernetes with Azure Pipelines
The build and push of the image in the Docker Hub
Automatic deployment of the application in Kubernetes
Summary
Questions
Further reading
Section 4: Testing Your Application
Testing APIs with Postman
Technical requirements
Creating a Postman collection with requests
Installation of Postman
Creating&#xA0;a collection
Creating our first request
Using environments and variables to dynamize requests
Writing Postman tests
Executing Postman request tests locally
Understanding the Newman concept
Preparing Postman collections for Newman
Exporting the collection
Exporting the environments
Running the Newman command line
Integration of Newman in the CI/CD pipeline process
Build and release configuration
Npm install
Npm run newman
Publish test results
The pipeline execution
Summary
Questions
Further reading
Static Code Analysis with SonarQube
Technical requirements
Exploring SonarQube&#xA0;
Installing SonarQube
Overview of the SonarQube architecture
Installing SonarQube
Manual installation of SonarQube
Installation via Docker
Installation in Azure
Real-time analysis with SonarLint
Executing SonarQube in continuous integration
Configuring SonarQube
Creating a CI pipeline for SonarQube in Azure Pipelines
Summary
Questions
Further reading
Security and Performance Tests
Technical requirements
Applying web security and penetration testing with ZAP
Using ZAP for security testing
Ways to automate the execution of ZAP
Running performance tests with Postman
Summary
Questions
Further reading
Section 5: Taking DevOps Further
Security in the DevOps Process with DevSecOps
Technical requirements
Testing Azure infrastructure compliance with Chef&#xA0;InSpec
Overview of InSpec
Installing InSpec
Configuring Azure for InSpec
Writing InSpec tests
Creating an InSpec profile file
Writing compliance InSpec tests
Executing InSpec
Using the Secure DevOps Kit for Azure
Installing the Azure DevOps Security Kit
Checking the Azure security using AzSK
Integrating AzSK in Azure Pipelines
Preserving data&#xA0;with HashiCorp's Vault
Installing Vault locally
Starting the Vault server
Writing secrets in Vault
Reading secrets in Vault
Using the Vault UI web interface
Getting Vault secrets in Terraform
Summary
Questions
Further reading
Reducing Deployment Downtime
Technical requirements
Reducing deployment&#xA0;downtime with Terraform
Understanding blue-green deployment concepts and patterns
Using blue-green deployment to improve the production environment
Understanding the canary release pattern
Exploring the dark launch pattern
Applying blue-green deployments on Azure
Using App Service with slots
Using Azure Traffic Manager
Introducing feature flags
Using an open source framework for feature flags
Using the LaunchDarkly solution
Summary
Questions
Further reading
DevOps for Open Source Projects
Technical requirements
Storing the source code in GitHub
Creating a new repository on GitHub
Contributing to the GitHub project
Contributing using pull requests
Managing the changelog and release notes
Sharing binaries in GitHub releases
Using Travis CI for continuous integration
Getting started with GitHub Actions
Analyzing code with SonarCloud
Detecting security vulnerabilities with WhiteSource Bolt
Summary
Questions
Further reading
DevOps Best Practices
Automating everything
Choosing the right tool
Writing all your configuration in code
Designing the system&#xA0;architecture
Building a good CI/CD pipeline
Integrating tests
Applying security with DevSecOps
Monitoring your system
Evolving project management
Summary
Questions
Further reading
Assessments
Chapter 1: DevOps Culture and Practices
Chapter 2:&#xA0;Provisioning Cloud Infrastructure with Terraform
Chapter 3:&#xA0;Using Ansible for Configuring IaaS Infrastructure
Chapter 4:&#xA0;Optimizing Infrastructure Deployment with Packer
Chapter 5: Managing Your Source Code with Git
Chapter 6:&#xA0;Continuous Integration and Continuous Delivery
Chapter 7:&#xA0;Containerizing Your Application with Docker
Chapter 8:&#xA0;Managing Containers Effectively with Kubernetes
Chapter 9:&#xA0;Testing APIs with Postman
Chapter 10:&#xA0;Static Code Analysis with SonarQube
Chapter 11:&#xA0;Security and Performance Tests
Chapter 12:&#xA0;Security in the DevOps Process with DevSecOps
Chapter 13: Reducing Deployment Downtime
Chapter 14:&#xA0;DevOps for Open Source Projects
Chapter 15:&#xA0;DevOps Best Practices
Other Books You May Enjoy
Leave a review - let other readers know what you think
