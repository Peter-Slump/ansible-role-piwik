# Ansible role Piwik

Version: 0.0.2

Supported OS: Ubuntu

Ansible role Piwik

## Role variables
```
piwik_user: piwik
piwik_group: "{{ piwik_user }}"
piwik_home: "/home/{{ piwik_user }}"

piwik_hostname: piwik.example.com

piwik_database_name: piwik
piwik_database_user: piwik
piwik_database_password: ChAnGeMe

piwik_download_url: https://builds.piwik.org/piwik.zip

piwik_web_root: "{{ piwik_home }}"

piwik_use_self_signed_ssl: False
piwik_use_letsencrypt: False

piwik_php_port: 9005
```

## Example
```
- hosts: all
  roles:
   - role: piwik
     piwik_hostname: piwik.example.com
```
