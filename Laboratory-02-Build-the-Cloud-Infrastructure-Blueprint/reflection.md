# Reflection

## 1. Which cloud infrastructure component do you think is the most important? Why?
I think compute is the most important component. It's the resource that
actually does the work running applications, processing requests, and
executing code. Storage and networking are essential too, but they only
support compute: storage holds the data compute needs, and networking lets
compute be reached. Without compute, none of the other components have
anything to "power."

## 2. How does Linux support cloud computing?
Linux manages the hardware resources (CPU, memory, disk, network) of a
server efficiently and predictably, which is critical when a cloud provider
is running thousands of virtual machines at once. Because Linux is
open-source, stable, and lightweight, it has become the standard operating
system for cloud servers. Its strong command-line tools also make it easy
for engineers to configure, monitor, and automate infrastructure at scale.

## 3. Why is technical documentation important before deploying infrastructure?
Documentation prevents costly mistakes and miscommunication. Before spending
time or money provisioning real servers, a written infrastructure report
lets engineers, teammates, or clients confirm that what's being built
actually matches what's needed. It also creates accountability if
something breaks later, the documentation shows what was planned and why
certain decisions were made.

## 4. What new skills did you learn during this laboratory activity?
I learned how to investigate a Linux server's compute, storage, and
networking details directly from the command line using tools like
`lscpu`, `free -h`, `df -h`, and `hostname`. I also learned how to compare
cloud providers using their actual product names (like EC2 vs. Compute
Engine vs. Azure VMs), and how to design a simple cloud architecture diagram
showing how a user's request flows through a network to compute and
storage.

## 5. How has your GitHub portfolio improved after completing this mission?
My portfolio now goes beyond the basic Linux and Git skills from Lab 1 — it
shows I can investigate real infrastructure, compare cloud providers, and
produce professional technical documentation like an actual junior cloud
engineer would. Having a second, well-structured lab folder also makes the
whole repository look more like a real, growing portfolio rather than a
single one-off assignment.
