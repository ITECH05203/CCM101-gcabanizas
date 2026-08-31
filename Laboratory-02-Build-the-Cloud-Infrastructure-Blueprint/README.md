# Laboratory Activity 2 – Mission 2: Build the Cloud Infrastructure Blueprint

## Mission Overview
This activity simulates the planning phase of a cloud deployment. Using a
Linux server provisioned through KillerCoda, I investigated the underlying
infrastructure, identified the major components of cloud computing, compared
how the three leading cloud providers implement those components, and
produced a simple cloud infrastructure diagram.

## Objectives
- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components
- **Compute** – CPU and memory resources that run applications and processes.
- **Storage** – Persistent disk space for files and data.
- **Networking** – Hostname and IP addressing that let the server communicate.
- **Operating System** – Ubuntu Linux, which manages all of the above resources.

## Tools Used
- KillerCoda Playground (Ubuntu Linux environment)
- GitHub (version-controlled documentation and portfolio)
- Markdown (technical documentation)
- Draw.io (cloud architecture diagram)

## Linux Commands Executed
| Command | Purpose |
|---|---|
| `cat /etc/os-release` | Identify the operating system and version |
| `uname -r` | Check the kernel version |
| `lscpu` | View CPU model and core count |
| `nproc` | Count available CPU cores |
| `free -h` | Check total and available RAM |
| `df -h` | Check disk capacity and usage |
| `df -hT` | List mounted file systems |
| `hostname` | Display the server hostname |
| `hostname -I` | Display the server's IP address |

## Skills Learned
Investigating and documenting a Linux server's compute, storage, and
networking resources; differentiating cloud infrastructure components;
comparing AWS, Azure, and GCP services; designing a basic architecture
diagram; and maintaining a structured GitHub portfolio.

## Challenges Encountered
Mapping the same infrastructure concept to different service names across
AWS, Azure, and GCP required careful research. Translating command-line
output into clear, client-ready documentation also took extra effort.
