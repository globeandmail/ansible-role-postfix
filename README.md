ansible-role-postfix
======

This role will install postfix and configure it for either 'Local only' or 'Satellite system' type.  The others aren't supported by this role, at this time.

Variables
------

```
ansible_role_postfix_type:      one of 'Satellite system' or 'Local only'
ansible_role_postfix_mailname:  defaults to ansible_fqdn
```

If ansible_role_postfix_type is 'Satellite system', the following variable is required:
```
ansible_role_postfix_relayhost: <fqdn or IP of your mail relay host>
```
