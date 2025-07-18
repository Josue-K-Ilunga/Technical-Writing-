# Standard Operating Procedure to Set Up a Virtual Linux Server for Web Application Testing  


#### PURPOSE OF THE DOCUMENT
This document defines the standard and procedures to be used while setting up a virtual Linux Server for Web Application testing, while complying with best practices and company policies.

#### AUDIENCE
This document is designed for web developers, software engineers, and other staff members responsible for testing web applications.

#### APPROVAL TABLE
| Version      | Date         | Name         | Designation  |
|--------------|--------------|--------------|--------------|
| 1.0          | 2025-01-25   | Alex Carlo   | Author       |
| 1.1          | 2025-03-12   | Bob Keba     | Reviewer     |
| 1.3          | 2025-06-07   | Alan Ika     | Approver     |

#### ACCOUNTABILITY MATRIX



#### SCOPE
This Standard Operating Procedure outlines the following steps for setting up a virtual Linux server to test Web applications. 
1.	Virtual Machine Preparation
2.	Linux Server Configuration.
3.	Web Server Configuration.
4.	Testing environment preparation.
5.	Documentation of the Testing environment for future reference.

#### EXECUTION STEPS
##### Step 1: Virtual Linux Server Preparation
###### Step 1.1: Identify Purpose and Requirements
* Hypervisor / Virtualization Platform: VMware vSphere/Workstation are the ones to be considered.
* Install the hypervisor on the host system
###### Step 1.2: Create a New Virtual Machine (VM)
* Resource Allocation: CPU and Number of Cores: 4, RAM: 8Ghz, Disk size: 20GB
* Operating System: Attach the Linux ISO file (RHEL) as a virtual CD/DVD.
##### Step 2: Linux Server Configuration.
###### Step 2.1: Configure Virtual Machine Settings
* Choose language/region: English Canada/Winnipeg
* Create an admin user: (Username: Administrator, Password: admin123)
* Set hostname and IP address: (Hostname: Server-Test-Web#) IP Address: IP address 
* Complete installation and reboot
###### Step 2.2: Network Settings
* Configure network connectivity: Use NAT
* Assign IP Address: Use IP address in the range 10.10.10.10/24 - 10.10.10.20/24)
###### Step 2.3: Secure the Server
* Update the system: Run the command (sudo dnf update)
* Set up SSH access securely: Disable root login over SSH and use public key authentication
##### Step 3: Web Server Installation.
###### Step 3.1: Install a Web Server
* Install Apache Server: Run the command (sudo dnf install httpd )
##### Step 4: Testing environment preparation
###### Step 4.1: Install and configure a few key components
* Install a Programming Language Support: Install PHP (sudo apt install php libapache2-mod-php php-mysql)
* Install a database backend: Install MySQL (sudo apt install mysql-server)
##### Step 5: Documentation of the Testing environment for future reference.
###### Step 5.1: Document Web Application Test Details
* Record all relevant details, including configurations, settings, and allocated resources.
###### Step 5.2: Knowledge Transfer
* Provide information for knowledge transfer to relevant teams.

#### REVISION HISTORY
| Version      | Date         | Changes Made by | Summary of Changes                      |
|--------------|--------------|-----------------|-----------------------------------------|
| 1.0          | 2025-01-25   | Alex Carlo      | Initial Release of Document             |
| 1.4          | 2025-07-10   | Bob Keba        | Execution Steps/Secure the server added |













