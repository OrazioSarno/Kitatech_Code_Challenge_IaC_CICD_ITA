# Kitatech_Code_Challenge_IaC_CICD_ITA
Introduction

The goal of this project is to:
Create an Ansible playbook that allows you to perform the following activities:

    Provisioning of two CentOS VMs. The VMs can be local or on a Cloud provider of your choice.
    Configure the VMs: a. Make sure that the partition used by Docker has at least 40GB of free space by making an appropriate resize.
    Docker setup on VMs
    Configure Docker: a. Securely expose the Docker Daemon REST APIs b. Make sure the Docker Daemon is configured as a service that starts automatically on system startup
    Set up a Docker Swarm on the VMs, which is securely accessible. Make sure you are able to interact and deploy services on the Swarm from the local machine.

Optionally:

    Test a task chosen from the previous ones using Molecule Represent each activity with appropriate Ansible roles and related tasks. The reuse of Ansible roles and playbooks made available in the open-source community is highly recommended (some of which are already linked in the text as an example and below for useful references). In case of code reuse it is important to motivate the role selection criteria, to know its features and contents, and to be able to describe any customizations made in order to carry out the above activities.

Versioning of the Code:

    Versioning the code on a public repository on Github.com, so that there is a clear description of the work done in the History of the repository;

Continuous Integration:

    Configure a Continuous Integration pipeline on a tool of your choice (advice: Travis, for simple integration with GitHub, Ansible Docker);

    The pipeline must: a. Lint the code and fail in case of errors, which must be corrected accordingly

    Optionally: Execute the test performed at point 6 automatically at each push of code to the repository

Useful references:

• Ansible User Guide: https://docs.ansible.com/ansible/latest/user_guide/index.html • Ansible Galaxy: https://galaxy.ansible.com/ • Best Practices: http://hakunin.com/ six-ansible-practices
• Testing Ansible provisioning locally: https://www.hamvocke.com/blog/local-ansible-testing/
• Testing Ansible roles and playbooks:
https://www.digitalocean.com/community/tutorials/how-to-implement-continuous-testing-of-ansible-roles-using-molecule-and-travis-ci-on-ubuntu-18-04 • Importance of version pinning: in general, tied to Docker and infrastructure • Role-rich and well-documented playbook for Docker Enterprise Edition setup: https://github.com/HewlettPackard/Docker-SimpliVity 

Dependencies

    Ansible
    Python
        jmespath
    Ruby

Setup

Generate RSA ssh key pair:

$ ssh-keygen -t rsa -N '' -f ~/.ssh/id_rsa -q

Usage

# go to project directory
$ cd /.../Kitatech_Code_Challenge_IaC_CICD_ITA
