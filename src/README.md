Building need to tools of Centos

# Run all mdule
command:
		ansible-playbook -i hosts deploy.yml

# Run common module, This module contain all base tools, It need to be runing first
command:
		ansible-playbook -i hosts deploy.yml --tags "common"

# Run work module contain, This module contain all work tools, let it work, need to ran common module first 
command:
		ansible-playbook -i hosts deploy.yml --tags "work"

