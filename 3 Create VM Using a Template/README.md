# Create VM Using a Template

This document provides a guide to creating a Virtual Machine (VM) instance using a predefined template in Google Cloud Platform (GCP), allowing for the quick deployment of multiple VMs with identical configurations.

## Introduction

Creating VMs using a template streamlines the process of deploying multiple instances with the same setup, saving time and ensuring consistency across your environment. This is particularly useful for scaling applications or services rapidly.

## Prerequisites

- Access to Google Cloud Platform (GCP) with a valid account.
- Completion of the steps outlined in the "Create VM Instance from Cloud Console" README.

## Steps

1. **Create an Image**: Shut down the VM instance (`vm1`) and create an image (`vm-image`) based on its disk. This image will be used as the basis for the template.

2. **Create Instance Template**:
    - Navigate to Navigation menu > Compute Engine > Instance templates.
    - Click on "Create instance template" and use the previously created image as the boot disk.
    - Specify the template details according to the assignment requirements, including Name, Series, Machine Type, and Firewall settings.

3. **Deploy VMs Using Template**:
    - Use the `gcloud` command-line interface to create new VM instances using your template.
    - Verify the deployment by checking the external links for specific VMs (e.g., `vm2` and `vm8`) to ensure they are properly set up.

    ```
    gcloud compute instances create --zone "Zone" --source-instance-template vm1-template vm2 vm3 vm4 vm5 vm6 vm7 vm8
    ```

## Conclusion

This README guides the process of using a template for deploying multiple VM instances in GCP. This method ensures a quick and consistent setup across multiple VMs, facilitating the management and scalability of cloud-based services or applications.
