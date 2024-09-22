# Installation of Apache CloudStack by Dockers 🐳

Apache CloudStack is an open-source cloud management platform designed to deploy and manage large networks of virtual machines, providing Infrastructure as a Service (IaaS) capabilities. CloudStack is commonly used by service providers and enterprises looking to build large-scale cloud infrastructures similar to AWS, Google Cloud, or Azure but in a self-managed environment.

# Features
<ul> 
     <li>Multi-Tenant Support</li> 
     <li>Elastic Load Balancing</li>
     <li>Snapshot and Backup Management</li>
     <li>Network-as-a-Service (NaaS)</li>
     <li>Hypervisor Agnostic</li>
     <li>API and CLI Support</li>
     <li>Web-based User Interface</li>
     <li>RESTful API</li>
     <li>High Availability (HA)</li>
     <li>Resource Management (Compute, Storage, Network)</li>
     <li>Scalability and Elasticity</li>
     <li>Role-Based Access Control</li>
     <li>Virtual Machine Orchestration</li>
     <li>Open-Source and Extensible</li>
</ul>

### This particluar repository focuses installating of Apache Web Server on Linux OS

# Process of Installation

### 1. ~ sudo apt update :  updates the package lists for available packages and their versions, but it does not install or upgrade any packages.

### 2. ~ sudo apt install apt-transport-https ca-certificates curl software-properties-common : installs the necessary packages to enable HTTPS for APT, manage SSL certificates, download files using curl, and add/manage software repositories.

### 3. ~ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -  : downloads the Docker GPG key and adds it to the system's list of trusted keys for verifying Docker packages.

### 4. ~ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" : adds the Docker repository for Ubuntu Focal (20.04) to the system's APT sources for downloading and installing Docker packages.

### 5. ~ apt-cache policy docker-ce : displays the installed version (if any) and available versions of the Docker CE (Community Edition) package, along with information about the repository sources from which Docker can be installed.

### 6. ~ sudo apt install docker-ce : installs Docker Community Edition (Docker CE) on the system from the available package repositories.

### 7. ~ sudo systemctl status docker : displays the current status of the Docker service, showing whether it is active (running), inactive, or failed, along with additional service information and logs.

### 8. ~ docker : displays a list of available Docker commands and options, providing an overview of how to use Docker's command-line interface (CLI).

### 9. ~ sudo docker info : displays detailed information about the Docker installation, including system-wide data like the number of containers, images, storage driver, and Docker's configuration.

### 10. ~ sudo docker run hello-world : downloads and runs the "hello-world" Docker image, which serves as a test to verify that Docker is installed and working correctly by displaying a message.

### 11. ~ sudo docker ps -l : shows the most recently created container, including its ID, image name, command, creation time, status, and assigned name. In this case, it indicates that the "hello-world" container exited successfully shortly after running.

### 12. ~ sudo docker run --name cloudstack-simulator -p 8080:5050 -d apache/cloudstacksimulator : runs a Docker container named "cloudstack-simulator" from the "apache/cloudstacksimulator" image, mapping port 8080 on the host to port 5050 in the container, and runs it in detached mode (in the background).

### 13. ~ sudo docker ps -l : To check info & installation about apache cloudstack container 
