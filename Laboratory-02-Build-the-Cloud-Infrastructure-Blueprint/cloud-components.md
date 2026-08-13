# Cloud Infrastructure Components

This document identifies and explains the major cloud infrastructure components 
observed in the KillerCoda Linux environment, and relates each to their role in 
cloud computing.

---

## 1. Compute Resources

**Observed in environment:** CPU and RAM allocated to the KillerCoda instance

**Purpose:**  
Compute resources are the processing power that executes instructions, runs 
applications, and performs calculations. In a cloud context, this refers to 
virtual machines, containers, or serverless functions that provide the CPU and 
memory needed to run workloads.

**Why it's important in cloud computing:**  
Compute is the core resource cloud providers sell — it determines how fast and 
how many tasks a system can handle. Cloud computing allows compute resources to 
be scaled up or down on demand (elasticity), so businesses only pay for what 
they use instead of maintaining physical servers.

**Relation to KillerCoda environment:**  
The KillerCoda playground itself is a virtual machine instance provisioned in 
the cloud, providing temporary compute power (CPU and RAM) to run Linux commands. 
This mirrors how a cloud provider like AWS EC2 or Azure VMs allocates compute 
instances to users.

---

## 2. Storage Resources

**Observed in environment:** Root filesystem (/dev/vda1) — 19G total, ext4 format

**Purpose:**  
Storage resources hold data — files, applications, logs, and system data — 
either temporarily or persistently. This includes block storage, object 
storage, and file systems.

**Why it's important in cloud computing:**  
Cloud storage allows data to be stored reliably, backed up, and accessed 
from anywhere, without depending on a single physical device. It also enables 
scalability, since storage capacity can be increased without hardware changes.

**Relation to KillerCoda environment:**  
The root filesystem (`/`) observed via `df -h` represents the disk storage 
allocated to the KillerCoda instance. This is analogous to a cloud provider's 
block storage volume (e.g., AWS EBS, Azure Managed Disks) attached to a virtual 
machine.

---

## 3. Networking Resources

**Observed in environment:** Hostname "ubuntu", IP address 172.30.1.2 (enp1s0)

**Purpose:**  
Networking resources allow systems to communicate with each other and with 
external users over the internet or private networks. This includes IP 
addressing, DNS, firewalls, and virtual networks.

**Why it's important in cloud computing:**  
Networking connects cloud services to users and to each other. It enables 
remote access, load balancing, and secure communication between distributed 
systems — all essential for cloud-based applications to be reachable and 
functional.

**Relation to KillerCoda environment:**  
The KillerCoda instance was assigned an internal IP address and hostname, 
allowing the terminal session to communicate over a network. This reflects how 
cloud providers assign private/public IPs to virtual machines within a Virtual 
Private Cloud (VPC) or Virtual Network (VNet).

---

## 4. Operating System

**Observed in environment:** Ubuntu 24.04 (Linux-based OS)

**Purpose:**  
The operating system manages hardware resources and provides the environment 
in which applications run. It handles process management, memory allocation, 
file systems, and user permissions.

**Why it's important in cloud computing:**  
The OS is the foundation that cloud compute instances run on. Cloud providers 
offer various OS images (Linux distributions, Windows Server, etc.) so users 
can choose the environment best suited for their applications.

**Relation to KillerCoda environment:**  
The KillerCoda playground runs Ubuntu
