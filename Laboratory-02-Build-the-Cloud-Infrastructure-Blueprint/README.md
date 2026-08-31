# Laboratory Activity 2 – Mission 2: Build the Cloud Infrastructure Blueprint

## Mission Overview
This activity simulates the planning phase of a cloud deployment. Using a
Linux server provisioned through KillerCoda, I investigated the underlying
infrastructure, identified the major components of cloud computing, compared
how the three leading cloud providers implement those components, and
produced a simple cloud infrastructure diagram — all documented as if
preparing a Cloud Infrastructure Assessment Report for a client.

## Objectives
- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components
- **Compute** – CPU and memory resources that run applications and processes (investigated via `lscpu`, `nproc`, `free -h`).
- **Storage** – Persistent disk space for files and data (investigated via `df -h`).
- **Networking** – Hostname and IP addressing that let the server communicate (investigated via `hostname`, `ip a`).
- **Operating System** – Ubuntu Linux, which manages all of the above resources (investigated via `lsb_release -a`, `uname -r`).

See `cloud-components.md` for the full breakdown, and `cloud-provider-comparison.md` for how AWS, Azure, and GCP each implement these components.

## Tools Used
- KillerCoda Playground (Ubuntu Linux environment)
- GitHub (version-controlled documentation and portfolio)
- Markdown (technical documentation)
- Draw.io / diagramming tool (cloud architecture diagram)

## Linux Commands Executed
| Command | Purpose |
|---|---|
| `lsb_release -a` | Identify the operating system and version |
| `uname -r` | Check the kernel version |
| `lscpu` | View CPU model and core count |
| `nproc` | Count available CPU cores |
| `free -h` | Check total and available RAM |
| `df -h` | Check disk capacity and usage |
| `mount` / `df -hT` | List mounted file systems |
| `hostname` | Display the server hostname |
| `ip a` / `hostname -I` | Display the server's IP address |

## Skills Learned
- Investigating and documenting a Linux server's compute, storage, and
  networking resources.
- Differentiating cloud infrastructure components and explaining their role
  in a cloud deployment.
- Comparing equivalent services across AWS, Azure, and GCP using official
  documentation.
- Designing a basic cloud architecture diagram.
- Structuring and maintaining professional technical documentation in a
  GitHub portfolio.

## Challenges Encountered
Understanding how the same infrastructure concept (e.g., compute or storage)
maps to different service names across AWS, Azure, and GCP required careful
research into each provider's documentation. Translating raw command-line
output into clear, client-ready documentation also took extra effort to keep
the report professional and easy to understand for a non-technical audience.
