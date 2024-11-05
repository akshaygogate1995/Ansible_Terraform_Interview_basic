## Ansible 

1. Playbook to install Apache

---

- name: Install Apache on web servers

  hosts: webservers

  become: yes

  tasks:

    - name: Ensure Apache is installed
  
      apt:

        name: apache2

        state: present
