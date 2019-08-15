# Descirption

This Ansible role configures the [BitWarden]() service based on the instructions listed in [their documentation](https://help.bitwarden.com/article/install-on-premise/#manual-docker-installations).

# Configuration

```yaml
bitwarden_domain: secrets.example.com
bitwarden_inst_id: 'Acquired from https://bitwarden.com/host/'
bitwarden_inst_key: 'Acquired from https://bitwarden.com/host/'
bitwarden_db_pass: 'mySecretDBPassword'
bitwarden_id_cert_pass: 'mySecretCertPassword'
bitwarden_smtp_user: 'smtp-user'
bitwarden_smtp_pass: 'smtp-pass'
bitwarden_smtp_host: 'smtp.example.com'
bitwarden_smtp_port: 587
bitwarden_smtp_ssl: true
```

# Knwon Issues

__TODO__
