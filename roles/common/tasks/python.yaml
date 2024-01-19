- name: Install python packages
  ansible.builtin.dnf:
    name: "{{item}}" 
    state: present
  loop:
  - python36
  - gcc
  - python3-devel

- name: Install dependencies
  ansible.builtin.command: pip3.6 install -r requirements.txt
  args:
    chdir: /app