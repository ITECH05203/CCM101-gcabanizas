# Infrastructure Report

## Operating System
[paste output of: cat /etc/os-release  OR  lsb_release -a]

## Kernel Version
[paste output of: uname -r]

## CPU Model
[paste output of: lscpu | grep "Model name"]

## Number of CPU Cores
[paste output of: nproc  OR  lscpu | grep "^CPU(s):"]

## Total RAM
[paste output of: free -h]

## Disk Capacity
[paste output of: df -h]

## Mounted File Systems
[paste output of: mount | grep "^/dev"  OR  df -hT]

## Hostname
[paste output of: hostname]

## IP Address
[paste output of: ip a  OR  hostname -I]
