# Cloud Infrastructure Laboratory

## Mission Overview

This laboratory activity focuses on understanding basic cloud infrastructure by examining a Linux environment and identifying its compute, storage, networking, and operating system resources. It also compares the core infrastructure services of AWS, Microsoft Azure, and Google Cloud Platform.

## Objectives

- Identify the main cloud infrastructure components in a Linux environment.
- Document the compute, storage, networking, and operating system resources of the KillerCoda environment.
- Compare equivalent infrastructure services offered by AWS, Microsoft Azure, and Google Cloud Platform.
- Design a simple cloud infrastructure diagram containing compute, storage, networking, user, and internet connection components.
- Practice basic Linux commands for inspecting system resources and configuration.

## Cloud Infrastructure Components

### Compute Resources

The KillerCoda environment has an Intel Xeon E312xx processor with 1 CPU core. The compute resource provides the processing power needed to execute Linux commands and laboratory tasks.

### Storage Resources

The environment has a 19G disk capacity. Mounted file systems include `/`, `/boot`, and `/boot/efi`, which provide storage for the operating system and system files.

### Networking Resources

The KillerCoda environment has the IP addresses `172.30.2.1` and `172.17.0.1`. These provide network addresses used for communication within the Linux environment.

### Operating System

The laboratory environment uses Ubuntu 24.04.4 LTS with kernel version `6.8.0-136-generic`. The operating system provides the environment needed to run Linux commands and perform the laboratory activities.

## Tools Used

- KillerCoda
- Ubuntu Linux
- GitHub
- Canva
- Microsoft Word
- Web browser

## Linux Commands Executed

The following Linux commands were used to inspect the system:

- `cat /etc/os-release` – displayed the operating system information.
- `uname -r` – displayed the kernel version.
- `lscpu` – displayed CPU and processor information.
- `free -h` – displayed memory and swap information.
- `df -h` – displayed disk usage and mounted file systems.
- `hostname` – displayed the system hostname.
- `hostname -I` – displayed the IP addresses of the environment.

## Skills Learned

Through this laboratory activity, I learned how to inspect and document basic Linux system resources using command-line tools. I also learned how cloud providers offer equivalent infrastructure services under different names and how compute, storage, networking, and identity services work together in a cloud environment.

## Challenges Encountered

One challenge was understanding the information shown by the Linux commands because some of the output contains technical terms and system details. I also needed to make sure that the information collected from the environment was correctly documented in Markdown files and that the cloud infrastructure diagram was saved in the required folder and filename.
