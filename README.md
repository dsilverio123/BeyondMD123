<h1>BeyondMD Projects</h1>

<h2>Platform and Technologies</h2>
<ul>
    <li>Cloud Platform: AWS</li>
    <li>Service: EC2 Instance</li>
    <li>Containerization: Docker</li>
    <li>OS: Ubuntu</li>
</ul>

<hr>

<h3>1. Dockerized "Hello BeyondMD!" Page</h3>
<a href="#">View the Project in the Home Directory</a>

<h4>Description</h4>
<p>A simple page built with HTML, CSS, and/or JavaScript that displays "Hello BeyondMD!". This web page is dockerized to ensure easy deployment and consistent runtime environment.</p>

<h4>Dependencies</h4>
<pre><code>
Docker: sudo apt install docker.io
Docker Compose: sudo apt install docker-compose
</code></pre>

<hr>

<h3>2. System Health Reporting Script for Debian</h3>
<a href="#">View the System Health Project</a>

<h4>Description</h4>
<p>A script tailored for Debian systems to gather and report various system health metrics, including CPU usage, memory consumption, disk utilization, active users, and running processes.</p>

<h4>Dependencies</h4>
<pre><code>
sysstat: sudo apt install sysstat
net-tools: sudo apt install net-tools
</code></pre>

<hr>

<h3>3. Ansible Playbook for Docker on Debian Bookworm</h3>
<a href="#">View the Ansible Playbook Project</a>

<h4>Description</h4>
<p>An idempotent Ansible playbook designed for Debian Bookworm systems. This playbook automates the installation and configuration of Docker, ensuring it's executed without unnecessary changes to the system state.</p>

<h4>Dependencies</h4>
<pre><code>
Ansible: sudo apt install ansible
</code></pre>

<hr>

<h3>Docker Permissions and Setup</h3>
<p><strong>Add the User to the Docker Group:</strong> Docker has a group named docker. Any user added to this group will have the required permissions to run Docker commands without using sudo.</p>
<pre><code>
sudo usermod -aG docker ubuntu
</code></pre>
<p>After running this command, you'll need to log out and log back in for the group changes to take effect.</p>
<p><strong>Start the Docker Service:</strong> Ensure that the Docker service is running. If not, start it with:</p>
<pre><code>
sudo systemctl start docker
</code></pre>
<p><strong>Using sudo:</strong> As a quick workaround, you can use sudo to run Docker commands:</p>
<pre><code>
sudo docker-compose up
</code></pre>
<p><em>Note: This is not a recommended long-term solution. It's safer to run Docker commands without sudo by adding your user to the docker group as mentioned in the first step.</em></p>
<p><strong>Additional Information:</strong> The hostname in <code>/BeyondMD123/systemhealth123$</code> docker-compose.yml has to be changed to the appropriate host.</p>

<hr>

<h3>Firewall Settings</h3>
<p>Remember to always ensure your security groups are correctly configured, especially when deploying web-based applications. For the first project, allowing traffic on port 80 is vital:</p>

<h4>Inbound Rules:</h4>
<ul>
    <li>HTTP (Port 80)</li>
    <li>Custom TCP (Port 19999)</li>
    <li>SSH (Port 22)</li>
</ul>
<p><em>Note: Always ensure that your firewall or security groups are configured according to the needs of your application and the best security practices.</em></p>
