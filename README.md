# ansible

## About: 

This is a reusable ansible simple module which used to deploy and destroy in one command full env to aws on ec2 with docker.


## How to deploy: 
1. Install ansible
2. Create vars.yml file and fill those parameters: 
```
---
region: 
vpc_cidr_block: 
vpc_name: 
subnet_cidr_block: 
subnet_names:


security_group_name: 
ami_id: 
instance_type: 
key_name: 
volume_size: 
server_name: 
env: prod

private_key_path:
git_repo_url: 
git_repo_dest: 
```
3. Run this command: ```ansible-playbook deploy.yml```

## How to destroy: 
Run ``ansible-playbook destroy.yml``


<u>Author:</u> Shahar Kozenyuk
