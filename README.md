# Descirption

This Ansible role configures the [BitWarden]() service based on the instructions listed in [their documentation](https://help.bitwarden.com/article/install-on-premise/#manual-docker-installations).

# Configuration

```yaml
bitwarden_domain: secrets.example.com
bitwarden_ssl_private_key: 'super-secret-private-key'
bitwarden_ssl_certificate: 'public-certificate'
bitwarden_ssl_cert_authority: 'certificate-authority'
bitwarden_inst_id: 'Acquired from https://bitwarden.com/host/'
bitwarden_inst_key: 'Acquired from https://bitwarden.com/host/'
bitwarden_db_pass: 'mySecretDBPassword'
bitwarden_id_key: 'myInternalIdentityKey'
bitwarden_id_cert_pass: 'mySecretCertPassword'
bitwarden_smtp_user: 'smtp-user'
bitwarden_smtp_pass: 'smtp-pass'
bitwarden_smtp_host: 'smtp.example.com'
bitwarden_smtp_port: 587
bitwarden_smtp_ssl: true
# Optional YubiKey API
bitwarden_yubico_client_id: ~
bitwarden_yubico_secret_key: ~
# Duo A-Key
bitwarden_duo_akey: ~
# HaveIBeenPwned API Key
bitwarden_duo_hibp_api_key: ~
```

# Knwon Issues

* The default Nginx config assumes a lot of things
* Version upgrade will probably involve template updates
* Sometimes MSSQL instance refuses to start for no fucking reason
