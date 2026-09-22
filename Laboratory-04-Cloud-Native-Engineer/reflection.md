Deploying a container with Docker is much faster than setting up a Virtual Machine. Installing an operating system on a VM requires booting an ISO, going through the installation process, and allocating more system resources, while Docker containers can be created and started within seconds.

Port mapping (`-p 8080:80`) is necessary because a container's internal network is isolated from the host by default. Nginx runs on port 80 inside the container, so mapping it to port 8080 allows users to access the web server through the host machine.

When you run `docker rm`, any data stored in the container's writable layer is permanently deleted because that layer is removed along with the container. This shows why persistent data should be stored using Docker volumes when it needs to survive container removal.

Containerization changes the relationship between developers and IT operations by reducing the common "it works on my machine" problem. Since applications can run in consistent environments, deployment becomes more reliable and easier to manage across different systems.

Overall, this mission helped me better understand Docker and containerization. It is another step toward building a body of work that demonstrates my growth from a beginner into someone who is becoming comfortable working with cloud-native technologies.
