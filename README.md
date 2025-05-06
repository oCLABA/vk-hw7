# vk-hw7
vk-education hw7

# Ansible vault example

Создаем vault.yml
```bash
ansible-vault create vault.yml
```
Поместим содержимое vault.yml
```yaml
vault_app_user: "appadmin"
vault_app_password: "Sup3rS3cr3tP@ssw0rd123"
vault_sudoers_rule: '{{ vault_app_user }} ALL=(ALL) NOPASSWD:/usr/bin/systemctl'
```
