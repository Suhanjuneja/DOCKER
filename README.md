# *DOCKER*

Docker is an open-source platform designed to automate the deployment, scaling, and management of applications within lightweight, portable containers. These containers encapsulate an application and its dependencies, ensuring consistent environments across development, testing, and production stages. Unlike traditional virtual machines, Docker containers share the host operating system's kernel, making them more efficient in terms of resource usage and startup time.

![image alt](https://github.com/Suhanjuneja/DOCKER/blob/6d1dfccac0a1da011672bf37cbb859578fefaf88/DOCKER.png)

**Docker has several key features and functions that enhance application development and deployment. Here are some of the most notable:**

 - **Containerization**: Docker packages applications and their dependencies into containers, ensuring consistent environments across different stages of development.

 - **Portability**: Containers can run on any system that supports Docker, regardless of the underlying infrastructure, making it easy to move applications between environments.

- **Isolation**: Each container runs in its own isolated environment, reducing conflicts and enhancing security by limiting access to resources.

- **Lightweigh**t: Docker containers share the host OS kernel, making them more efficient in terms of resource utilization compared to traditional virtual machines.

- **Version Control**: Docker images can be versioned, allowing developers to track changes and revert to previous versions easily.

- **Docker Hub**: A cloud-based registry for sharing Docker images, enabling easy access to pre-built images and collaborative development. 
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

   # *NGINX*

   NGINX is a high-performance web server, reverse proxy server, and load balancer designed to handle high traffic and concurrent connections efficiently. Originally created to address the C10K problem (the challenge of handling 10,000 concurrent connections), NGINX is now widely used for serving static content, managing dynamic content, and improving the performance of web applications.

![image alt](https://github.com/Suhanjuneja/DOCKER/blob/fe7c23ea21d90ec2212d9a635f32787397899c24/nginx.png)

   **Key Features**:

-   **Reverse Proxy**: NGINX can act as a reverse proxy, forwarding client requests to backend servers, improving security and scalability.

- **Load Balancing**: It distributes incoming traffic across multiple servers, optimizing resource use and enhancing application reliability.

- **Static Content Serving**: NGINX excels at serving static files (like images, CSS, and JavaScript) efficiently, reducing the load on application servers.

- **SSL/TLS Termination**: It can handle SSL/TLS encryption, offloading this resource-intensive task from backend servers.

- **Caching**: NGINX supports caching mechanisms to speed up response times and reduce load on upstream servers.

- **High Availability**: It can be configured for failover and redundancy, ensuring continuous service availability.

- **Configurability**: NGINX uses a simple and flexible configuration file, making it easy to set up and customize.

![image aly](https://github.com/Suhanjuneja/DOCKER/blob/b1e6af675ee9810de3b7158452b0ed9c1bd00ddf/NGINX-Professional-Services-Consulting-Support-1.png)

------------------------------------------------------------------------------------------------------------------------------------------------------------------


# *HOW TO INSTALL NGINX*

In this tutorial, we’ll show you how to install NGINX on Linux. Open your Linux machine and run an update using the command below:

     sudo apt-get update  

Next, run this command:

sudo apt-get install nginx

Then, enable your firewall with the following:

sudo ufw enable

To verify NGINX is installed, run the following:

nginx -v

You can run the command below to find out if NGINX is running:

sudo ufw status

After running this command, you should see the following:

status: active

To check whether your NGINX server is working fine, run the following:

sudo systemctl status nginx

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# *HOW TO INSTALL DOCKER*

To install Docker on a remote server using PuTTY, you'll first need to ensure you have access to a Linux server (like Ubuntu, CentOS, etc.) via SSH. Here's a step-by-step guide:

Step 1: Connect to Your Server

Open PuTTY.

Enter the hostname or IP address of your server.
Click "Open" to initiate the connection.
Log in with your username and password.
Step 2: Update Your Package Index
Before installing Docker, it’s a good idea to update the package index:

sudo apt update
Step 3: Install Prerequisites
For Ubuntu, install the required packages:

sudo apt install apt-transport-https ca-certificates curl software-properties-common
For CentOS, run:

sudo yum install -y yum-utils
Step 4: Add Docker’s Official GPG Key
For Ubuntu:

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
For CentOS:

sudo rpm --import https://download.docker.com/linux/centos/gpg
Step 5: Set Up the Stable Repository
For Ubuntu:

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
For CentOS:

sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
Step 6: Install Docker
For Ubuntu:

sudo apt update
sudo apt install docker-ce
For CentOS:

sudo yum install docker-ce
Step 7: Start Docker
Enable and start the Docker service:

sudo systemctl start docker
sudo systemctl enable docker
Step 8: Verify the Installation
Check if Docker is running:

sudo systemctl status docker
You can also run a test container:

sudo docker run hello-world
Step 9: (Optional) Manage Docker as a Non-Root User
If you want to run Docker commands without sudo, add your user to the Docker group:

sudo usermod -aG docker $USER
After running this command, log out and back in for the changes to take effect


