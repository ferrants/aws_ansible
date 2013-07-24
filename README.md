Run
```
ansible-playbook --private-key=path/to/key -i hosts_local -v create_instance.yml
./ec2.py
ansible-playbook --private-key=path/to/key -i hosts_local -v teardown_instance.yml --extra-vars="instance_ids=i-c4e1e2a8"

```

Add to roles/aws/vars/main.yml, filling in details:
```
---
aws_access_key: 
aws_secret_key:
key_name:
```