# quick and dirty minikube

### To use this Role:

Edit the `site.yml` file, mentioned this role:

```yaml
---
 - hosts: yourbox
   become: yes
   gather_facts: yes
   roles:
     - common
``` 


Then run this command:

```
ansible-playbook -i hosts -u <youruser> site.yml
```
