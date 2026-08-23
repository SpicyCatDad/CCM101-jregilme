## Cloud Infrastructure Components

### 1. Compute Resources

**Purpose:** Supplies the CPU and RAM needed to run applications and workloads.
**Importance in cloud computing:** Compute is one of the main resources provided by cloud platforms, allowing users to run programs, host applications, and process information (e.g., EC2, Azure VMs, Compute Engine).
**In this environment:** The KillerCoda VM acts as a compute resource, with its CPU cores and RAM shown in Checkpoint 2 providing the processing power for running services.

### 2. Storage Resources

**Purpose:** Stores data such as files, databases, and logs so they remain available beyond the compute instance's lifecycle.
**Importance in cloud computing:** Cloud storage is designed to be durable and scalable, allowing data to remain even when a compute instance is removed.
**In this environment:** The disks and mounted filesystems displayed through `df -h` serve as the storage connected to the KillerCoda instance.

### 3. Networking Resources

**Purpose:** Allows compute and storage resources to communicate with each other and connect to the internet.
**Importance in cloud computing:** Networking enables communication between services, provides security through firewalls and VPCs, and allows applications to be accessed remotely.
**In this environment:** The VM's IP address and hostname identify it within its network, similar to how cloud VMs use private or public IP addresses within a VPC.

### 4. Operating System

**Purpose:** Controls hardware resources and provides the environment needed for software and applications to operate.
**Importance in cloud computing:** Most cloud servers use operating systems, with Linux being widely used because it is lightweight, flexible, and open source.
**In this environment:** The Linux distribution and kernel version found in Checkpoint 2 represent the operating system layer running on the KillerCoda compute instance.
