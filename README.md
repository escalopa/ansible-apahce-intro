# ansible-apahce-intro
Auto deploy site with ansible

## Deploy your site

### Install ansible (Ubuntu)

If you have a different distribution than `ubuntu` then refer to the ansible installation documentation [here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

```shell
curl "https://raw.githubusercontent.com/escalopa/script-installer/main/scripts/ansible.sh"  | bash
```

### Git clone repo & cd in 

```
git clone https://github.com/escalopa/ansible-apahce-site-deployer.git && cd ansible-apahce-site-deployer
```

### Copy your server private key

Replace `KEY_NAME` with the name of your private key or change the whole path if your key is in different location
```
cp ~/.ssh/KEY_NAME ./credentials/ansible
```

### Set hostname in yaml files

- Change hostname in `hosts.yaml` to the ip address of your host (Or the name bined to the ip address)
- Change hostname in `deployer.yaml` exactly under the line `hosts` to the ip address of your host (Or the name bined to the ip address)


