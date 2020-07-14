# ansible-role-phpldapadmin

Role to install and configure phpLDAPadmin

# Role Variables

Below is the full list of variables:

| Variable | Description | Default |
|----------|-------------|---------|
| `phpldapadmin_url`| Download URL  | `https://github.com/leenooks/phpLDAPadmin/archive/master.zip` |
| `phpldapadmin_apache_server_admin`| Email support | `admin@hostname` |
| `phpldapadmin_host`| URL and port to connect LDAP  | `ldap://example.com:389` |
| `phpldapadmin_base`| Specify the base content to display | `dc=base,dc=com` |
| `phpldapadmin_auth.type`| Setting type session | `auth_type` |
| `phpldapadmin_auth.via`| Setting session or cookie | `cookie` |
| `phpldapadmin_login_admin.type`| Setting type login admin (DN,cn,etc) | `bind_id` |
| `phpldapadmin_login_admin.base`| User admin to LDAP | `cn=userldap,ou=group,dc=example,dc=com` |
| `phpldapadmin_login_admin.type_password`| Setting type login admin | `bind_pass` |
| `phpldapadmin_login_admin.password`| Specify the password of the LDAP admin User | `null` |
| `phpldapadmin_certificates.type`| Specify type certificates | `tls` |
| `phpldapadmin_certificates.check`| True/False | `false` |
| `phpldapadmin_login.type`| Select type parameter for login | `attr` |
| `phpldapadmin_login.objectClass`| Select parameter for login | `cn` |
| `phpldapadmin_login.base`| Specify location of users | `ou=group,dc=example,dc=com` |
| `phpldapadmin_hide_template_warning`| Disable or enable warning | `false` |
| `phpldapadmin_reCAPTCHA_enable`| Enable captcha | `false` |
| `phpldapadmin_reCAPTCHA_key_site`| reCAPTCHA Public | `vault` |
| `phpldapadmin_reCAPTCHA_key_server`| reCAPTCHA Secret | `vault` |

# Example Playbook

    - hosts: all
      roles:
        - { role: ansible-role-phpldapadmin }

# License

GPLv2

Author Information
------------------

https://github.com/UdelaRInterior/ansible-role-phpldapadmin
