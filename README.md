**Palo Alto Firewall Configuration Automation**

This project automates the configuration of a Palo Alto Networks firewall using Ansible. It includes tasks for setting up security policies, creating custom services, and configuring network interfaces. The project is designed to simplify the process of managing firewall configurations, especially in environments where multiple rules and services need to be deployed consistently.

**Features**

Security Policy Configuration: Automates the creation of security policies on the Palo Alto firewall.

Custom Service Creation: Creates custom services (e.g., TCP ports 80 and 8080) for use in security policies.

Interface Configuration: Configures network interfaces, including IP addresses, zones, and modes.

Variable Management: Uses a vars.yml file to manage configuration variables, making it easy to customize and reuse.

**Prerequisites**

Before using this project, ensure you have the following:

Ansible: Install Ansible on your system. You can install it using pip:
pip install ansible

Palo Alto Networks Ansible Collection: Install the paloaltonetworks.panos collection:
ansible-galaxy collection install paloaltonetworks.panos
Palo Alto Firewall: Ensure you have access to a Palo Alto firewall with the necessary credentials.

Python: Ensure Python 3 is installed on your system.

**File Structure**
The project consists of the following files:

security_policy.yml: Ansible playbook for configuring security policies and creating custom services.

vars.yml: Contains variables for firewall configuration, including provider details, interfaces, address objects, and security policies.

hosts.ini: Inventory file specifying the target firewall device.

test.yml: Ansible playbook for configuring network interfaces on the firewall.
