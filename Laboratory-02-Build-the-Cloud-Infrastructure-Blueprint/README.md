# Laboratory Activity 2: Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity simulates the planning phase of a cloud deployment 
for a fictional company preparing to migrate its services to the cloud. Using 
a temporary Linux server provisioned through the KillerCoda Playground, this 
project investigates the core components of cloud infrastructure — compute, 
storage, networking, and identity — and documents the findings as a Cloud 
Infrastructure Assessment Report intended to guide senior engineers in 
designing the final cloud architecture.

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

Four core infrastructure components were identified and documented in this 
lab (see `cloud-components.md` for full detail):

- **Compute Resources** — the CPU and RAM allocated to the KillerCoda instance, 
  representing the processing power that runs applications and workloads.
- **Storage Resources** — the root filesystem (`/dev/vda1`, ext4) providing 
  persistent disk space, comparable to block storage volumes in the cloud.
- **Networking Resources** — the hostname and IP address assigned to the 
  instance, enabling communication within a virtual network.
- **Operating System** — Ubuntu 24.04, the Linux distribution managing 
  hardware resources and providing the runtime environment.

A comparison of how AWS, Azure, and GCP each implement these components is 
documented in `cloud-provider-comparison.md`.

## Tools Used

- KillerCoda Playground (Ubuntu 24.04 Linux environment)
- Linux terminal and command-line tools
- GitHub (version control and portfolio hosting)
- Git (commit and push workflow)
- Markdown (technical documentation)
- Diagramming tool (for the cloud architecture diagram)

## Linux Commands Executed

| Command | Purpose |
|---------|---------|
| `cat /etc/os-release` | Identify the operating system and version |
| `uname -r` | Check the kernel version |
| `lscpu` | Retrieve CPU model and core count |
| `free -h` | Check total RAM |
| `df -h` | Check disk capacity and usage |
| `df -hT` | List mounted filesystems and their types |
| `hostname` | Display the system hostname |
| `hostname -I` / `ip a` | Display assigned IP address(es) |

## Skills Learned

- Investigating a Linux environment to extract hardware and system information.
- Distinguishing between the core categories of cloud infrastructure (compute, 
  storage, networking, identity) and relating them to real system components.
- Comparing infrastructure services across AWS, Azure, and GCP despite each 
  provider using different product names for equivalent services.
- Structuring and writing professional technical documentation in Markdown.
- Using Git and GitHub for version control, including staging, committing, 
  and pushing changes, and troubleshooting authentication with personal 
  access tokens.
- Designing a basic cloud architecture diagram showing how compute, storage, 
  networking, and users interact.

## Challenges Encountered

- GitHub no longer accepts account passwords for git push authentication, 
  requiring a Personal Access Token instead — this required extra research 
  to resolve.
- Ensuring the exported architecture diagram was saved as a true `.png` file 
  rather than an `.svg` mislabeled with a `.png` extension.
- Remembering that Git does not track empty folders, which meant the 
  `screenshots` folder needed at least one file inside it before it would 
  appear in the repository.
