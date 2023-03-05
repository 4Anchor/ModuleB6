# Ansible repository

## Роли

### Install PostgreSQL

Используется если надо установить DB PostgreSQL 

```
ansible-playbook --vault-password-file=/opt/vault-pass -i inventory/sf_hwork_pg.yml --tags=deploy_pg playbooks/playbook_pg.yml -v
```


### Install  Docker

Используется если надо установить Docker+Docker-compose на группе хостов

```
ansible-playbook -i inventory/sf_docker.yml --tags=deploy_docker playbooks/playbook_pg.yml -v
```

