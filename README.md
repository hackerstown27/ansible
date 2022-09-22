# ansible

This Folder contains the ansible role for Opensearch Search Setup (Multi-Node)

## Prerequisites

- Make sure to edit the hosts file and pass the IPs of host in primary and secondary group:
- primary: host on which opensearch-dashboard will be installed
- secondary: hosts on which opensearch will be installed

- Also provide SSH key for each host

```
[primary]
opensearch-node-1 ansible_host=x.x.x.x ansible_connection=ssh ansible_user=username ansible_ssh_private_key_file=sshKey.pem

[secondary]
opensearch-node-2 ansible_host=x.x.x.x ansible_connection=ssh ansible_user=username ansible_ssh_private_key_file=sshKey.pem

```

- Now use the below command to execute the anisble playbook:

```ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook main.yml -i hosts```




## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.com/dotcomino/dotpe-devops/ansible.git
git branch -M main
git push -uf origin main

```


