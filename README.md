# What is this

An ansible role to configure my machine

# How to run

```bash
ansible-playbook playbook.yml
```

# Start the containers

```bash
for svc in haproxy claire; do
    docker-compose -f "/srv/compose/${svc}.yaml" -p "${svc}" up -d
done
```
