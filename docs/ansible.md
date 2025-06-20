**Wymagania**
- Obraz kontenera dostępny jest [tutaj](https://gitlab.com/pl.rachuna-net/containers/ansible/container_registry/8648376).

#### Ansible playbook `💥 ansible playbook`
Job uruchamia `ansible playbook`, który wykonuje deployment.

```bash
for file in playbooks/*.yml; do
    ansible-playbook -i $ANSIBLE_INVENTORY $file --extra-vars "$ANSIBLE_VARS"
done
```
