# Cloud Infrastructure Components

## Compute Resources
**Purpose:** Compute resources provide the processing power (CPU) and memory
(RAM) needed to run applications, execute code, and handle workloads.

**Why it matters in cloud computing:** Compute is the "engine" of any cloud
service — without it, no application, website, or service can actually run.

**In this KillerCoda environment:** The virtual machine running Ubuntu is
itself a compute resource — its CPU and RAM (checked using `lscpu` and
`free -h`) are what allow me to run commands and processes.

---

## Storage Resources
**Purpose:** Storage resources hold data persistently, such as files,
databases, logs, and application data.

**Why it matters in cloud computing:** Applications need a reliable place to
save and retrieve data, and storage can be scaled independently from compute.

**In this KillerCoda environment:** The disk space checked with `df -h`
represents the storage resource — the root filesystem (`/`) where all my
files and folders live.

---

## Networking Resources
**Purpose:** Networking resources connect systems together and to the
internet, allowing communication between servers, users, and services.

**Why it matters in cloud computing:** Cloud services need networking to be
reachable by users or by other systems.

**In this KillerCoda environment:** The container has its own hostname and
IP address (checked with `hostname` and `hostname -I`), letting it be
addressed on the KillerCoda platform's virtual network.

---

## Operating System
**Purpose:** The operating system manages hardware resources and provides
the environment where applications and services run.

**Why it matters in cloud computing:** Every cloud instance runs on an OS
(usually Linux for servers) that manages compute, storage, and networking.

**In this KillerCoda environment:** Ubuntu Linux is the OS running the
playground, confirmed via `cat /etc/os-release` and `uname -r`.
