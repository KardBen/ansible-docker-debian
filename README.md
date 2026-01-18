# Ansible Role: Docker for Debian

A streamlined Ansible role to install the **Official Docker Engine** and **Docker Compose** on Debian-based systems using the `keyrings` method. According to official Documentation: https://docs.docker.com/engine/install/debian/

## 📋 Requirements

* **Target OS:** Debian (Bullseye, Bookworm, or later).
* **Ansible Version:** 2.10 or higher.
* **Privileges:** The role requires root privileges (`become: true`).

## 📦 Installation

To use this role in your project, add it to your `requirements.yml`:

```yaml
roles:
  - name: docker_debian
    src: https://github.com/KardBen/ansible-docker-debian.git
    scm: git
    version: main
```

## 🚀 Example Playbook

Minimal configuration:

```yaml
- name: Setup Debian
  hosts: localhost
  become: true
  gather_facts: true

  roles:
    - docker_debian
```

## 📄 License
MIT

## 👤 Author
Benjamin Kardumovic