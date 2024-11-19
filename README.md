To use this playbok you have to make inventory.ini and add your hosts.

**cat ./inventory.ini** 

```[servers]
u26.local ansible_host=192.168.64.3 ansible_user=ubuntu ansible_pass=ubuntu ansible_become_password=ubuntu
f38.local ansible_host=192.168.64.4 ansible_user=fedora ansible_pass=fedora ansible_become_password=fedora
```
Then run

```bash
 ansible-playbook -i inventory.ini playbook.yml -Dv
```
