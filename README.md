# ansible-roles-automation
A collection of Ansible playbooks for server setup and automation with roles

# roboshop-ansible-project

This is an Ansible automation project to provision and configure the RoboShop application stack. RoboShop is a real-world e-commerce app used for DevOps learning.

## Project Overview

The application consists of several microservices, each implemented in a different language or framework. This repository provides Ansible playbooks and roles to deploy these services efficiently.

## What’s Included

- Ansible playbooks to install and configure:
  - Frontend (Nginx)
  - Backend microservices (catalogue, user, cart, payment, shipping)
  - Databases and tools (MongoDB, MySQL, Redis, RabbitMQ)
- Ansible roles for reusable logic
- Inventory file to define your target servers
- Pre-defined structure that follows Ansible best practices

## Folder Structure

- `ansible.cfg` – Ansible configuration file
- `inventory/roboshop.ini` – List of all target servers
- `playbooks/` – Contains one playbook per service
- `roles/` – Each service has its own Ansible role


