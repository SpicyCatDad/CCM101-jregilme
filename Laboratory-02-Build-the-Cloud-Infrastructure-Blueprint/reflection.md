# Cloud Infrastructure Components

## Compute Resources

**Purpose:** Compute resources supply the processing power required to run applications, perform calculations, and operate the operating system. They can be provided through virtual machines, containers, or serverless services.

**Why it matters in cloud computing:** Compute is essential for running any cloud-based workload. Cloud providers allow organizations to increase CPU and RAM or add more virtual machines as needed, eliminating the need to purchase physical servers.

**Relation to KillerCoda:** The KillerCoda playground functions as a virtual machine, providing a complete Linux environment on demand without requiring physical hardware.

## Storage Resources

**Purpose:** Storage resources provide the space needed for the operating system, applications, files, and other data. Cloud storage can be categorized as object, block, or file storage.

**Why it matters in cloud computing:** Cloud storage is designed to be scalable, reliable, and accessible. It can distribute data across multiple systems to improve durability and reduce dependence on physical storage devices.

**Relation to KillerCoda:** The disk space displayed by `df -h` represents storage allocated to the virtual machine. It works similarly to the root storage volume attached to a cloud VM on AWS, Azure, or GCP.

## Networking Resources

**Purpose:** Networking resources enable communication between virtual machines, storage, cloud services, and users. These include virtual networks, routers, firewalls, and load balancers.

**Why it matters in cloud computing:** Networking allows different cloud resources to communicate and makes applications accessible to users. Proper network configuration also helps protect systems from unauthorized access.

**Relation to KillerCoda:** The playground has its own hostname and IP address, which can be viewed using `hostname` and `hostname -I`. These identify the VM within KillerCoda's underlying cloud network and allow me to interact with it remotely through the browser.

## Operating System

**Purpose:** The operating system manages system resources, runs applications, and provides the interface used to interact with the machine, such as the Linux terminal.

**Why it matters in cloud computing:** Linux is widely used for cloud servers because it is lightweight, stable, and well supported. It provides the environment where cloud engineers configure, maintain, and secure their systems.

**Relation to KillerCoda:** The playground uses Ubuntu 24.04.4 LTS, which was verified using `cat /etc/os-release`. This is similar to the Linux distributions commonly installed on cloud virtual machines such as AWS EC2, Azure Virtual Machines, and Google Compute Engine.
