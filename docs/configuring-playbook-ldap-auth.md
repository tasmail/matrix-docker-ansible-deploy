# Setting up the LDAP authentication password provider module (optional, advanced)

The playbook can install and configure the [matrix-synapse-ldap3](https://github.com/matrix-org/matrix-synapse-ldap3) LDAP Auth password provider for you.

See the project's [documentation](https://github.com/matrix-org/matrix-synapse-ldap3/blob/main/README.rst) to learn what it does and why it might be useful to you.

If you decide that you'd like to let this playbook install it for you, add the following configuration to your `inventory/host_vars/matrix.example.com/vars.yml` file (adapt to your needs):

```yaml
matrix_synapse_ext_password_provider_ldap_enabled: true
matrix_synapse_ext_password_provider_ldap_uri:
  - "ldap://ldap-01.example.com:389"
  - "ldap://ldap-02.example.com:389"
matrix_synapse_ext_password_provider_ldap_start_tls: true
matrix_synapse_ext_password_provider_ldap_base: "ou=users,dc=example,dc=com"
matrix_synapse_ext_password_provider_ldap_attributes_uid: "uid"
matrix_synapse_ext_password_provider_ldap_attributes_mail: "mail"
matrix_synapse_ext_password_provider_ldap_attributes_name: "cn"
matrix_synapse_ext_password_provider_ldap_bind_dn: ""
matrix_synapse_ext_password_provider_ldap_bind_password: ""
matrix_synapse_ext_password_provider_ldap_filter: ""
```

## Authenticating only using a password provider

If you wish for users to **authenticate only against configured password providers** (like this one), **without consulting Synapse's local database**, feel free to disable it:

```yaml
matrix_synapse_password_config_localdb_enabled: false
```

## Using ma1sd Identity Server for authentication (not recommended)

The playbook can instead configure [ma1sd](https://github.com/ma1uta/ma1sd) Identity Server for LDAP authentication. However, **we recommend not bothering with installing it** as ma1sd has been unmaintained for years.

If you wish to install it anyway, consult the [ma1sd Identity Server configuration](configuring-playbook-ma1sd.md#authentication).

## Handling user registration

If you wish for users to also be able to make new registrations against LDAP, you may **also** wish to [set up the ldap-registration-proxy](configuring-playbook-matrix-ldap-registration-proxy.md).
