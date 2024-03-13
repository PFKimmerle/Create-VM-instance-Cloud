# Create VM Instance from Cloud Console

This document outlines the steps to create a Virtual Machine (VM) instance using the Google Cloud Platform (GCP) web UI, including VM instance configurations, cloning a Git repository, performing file operations, and restarting the VM.

## Introduction

The process involves creating a new VM instance in GCP, configuring it according to the project's requirements, and setting up an auto-enabled service. This serves as a foundational step towards deploying web servers or applications on the cloud.

## Prerequisites

- Access to Google Cloud Platform (GCP) with a valid account.
- Basic knowledge of cloud computing and VMs.

## Steps

1. **Navigate to VM Instances**: In GCP Console, go to Navigation menu > Compute Engine > VM instances.

2. **Create New Instance**:
    - Click on "Create instance".
    - Fill in the necessary details as specified in the assignment instructions, such as Name, Region, Zone, Series, Machine Type, Boot Disk, and Firewall configurations.

3. **SSH into VM1**: Use the SSH button provided in the console to securely connect to your newly created VM instance.

4. **Clone Repository**: Use the Git command provided to clone the repository to your VM. This repository contains the necessary scripts and configuration files.

    ```
    git clone https://www.github.com/google/it-cert-automation-practice.git
    ```

5. **Navigate and Operate**: Change directory to the specified folder and perform file operations as required by the assignment.

6. **Restart VM**: Follow the steps to stop and then start your VM instance to ensure all configurations and services are running correctly.

## Conclusion

This README outlines the steps to create and configure a VM instance in GCP, aimed at setting up a consistent and reproducible environment for web services or applications.
