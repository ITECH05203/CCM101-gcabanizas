# Cloud Infrastructure Components

## Compute Resources
**Purpose:** Compute resources provide the processing power (CPU) and memory (RAM)
needed to run applications, execute code, and handle workloads.

**Why it matters in cloud computing:** Compute is the "engine" of any cloud
service without it, no application, website, or service can actually run.
Cloud providers let you scale compute up or down on demand instead of buying
physical servers.

**In this KillerCoda environment:** The virtual machine running Ubuntu is
itself a compute resource its CPU and RAM (checked using `lscpu` and
`free -h`) are what allow me to run commands, install packages, and host
processes.

---

## Storage Resources
**Purpose:** Storage resources hold data persistently, such as files,
databases, logs, and application data.

**Why it matters in cloud computing:** Applications need a reliable place to
save and retrieve data. In the cloud, storage can be scaled independently
from compute, and can be made highly durable through replication.

**In this KillerCoda environment:** The disk space checked with `df -h`
represents the storage resource — the root filesystem (`/`) where files,
directories, and my portfolio structure (Documents, Notes, Reports,
Screenshots) are stored.

---

## Networking Resources
**Purpose:** Networking resources connect systems together and to the
internet, allowing communication between servers, users, and services.

**Why it matters in cloud computing:** Cloud services need networking to be
reachable — whether that's a web server responding to users, or one server
talking to a database on another machine.

**In this KillerCoda environment:** The container has its own hostname and
IP address (checked with `hostname` and `ip a`), which allow it to be
addressed and to communicate over the KillerCoda platform's virtual network.

---

## Operating System
**Purpose:** The operating system (OS) manages hardware resources and
provides the environment where applications and services run.

**Why it matters in cloud computing:** Every cloud instance runs on an OS
(most commonly Linux for servers) that manages compute, storage, and
networking resources, and provides the tools (like the terminal and package
managers) engineers use to configure the system.

**In this KillerCoda environment:** Ubuntu Linux is the OS running the
playground. Checking its version (`lsb_release -a`) and kernel (`uname -r`)
shows exactly which OS and kernel are managing the underlying hardware
resources I've been working with.
