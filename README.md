# Ansible Playbook Usage Guide

## Overview

This document provides step-by-step instructions on how to effectively use the Ansible playbook

## Prerequisites

1. **Clone Repository:**

2. **Enable AWS EC2 Plugin:**
   - Open the `/etc/ansible/ansible.cfg` file and ensure that the `aws_ec2` plugin is added in the `enabled_plugins` line. If the file is not populated, leave it be.

## Usage

5. **Navigate to Ansible Folder:**

   - Change your working directory to the Ansible folder.

6. **Generate Inventory Graph:**

   - Use the following command to generate an inventory graph from the provided AWS EC2 inventory file (`di.aws_ec2.yml`):
     ```bash
     ansible-inventory -i di.aws_ec2.yml --graph
     ```

7. **Run Ansible Playbook:**
   - Execute the Ansible playbook using the following command:
     ```bash
     ansible-playbook -i di.aws_ec2.yml playbook.yml
     ```


