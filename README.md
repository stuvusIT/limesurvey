# Limesurvey

A role to set up and configure a limesurvey instance. This role depends on an apt system.


## Role Variables

| Name                                               |    Default/Required     | Description                                                    |
|:---------------------------------------------------|:-----------------------:|:---------------------------------------------------------------|
| `limesurvey_release_link`                          |   :heavy_check_mark:    | Link to the tar.gz file of the survey instance to be installed |
| `limesurvey_mysql_database_name`                   |      `limesurvey`       | The database name                                              |
| `limesurvey_mysql_user`                            |      `limesurvey`       | Mysql user                                                     |
| `limesurvey_mysql_host`                            |      `localhost`       | Mysql host                                                 |
| `limesurvey_mysql_port`                            |      `3306`       | Mysql port                                                     |
| `limesurvey_smtp_server`                           |   :heavy_check_mark:    | SMTP server url                                                |
| `limesurvey_smtp_port`                             |   `587`   | SMTP Port                                                      |
| `limesurvey_smtp_user`                             |   :heavy_check_mark:    | SMTP User                                                      |
| `limesurvey_smtp_password`                         |            ` `            | SMTP password                                                  |
| `limesurvey_smtp_ssl`                              |   `tls`    | SMTP encryption either `ssl`, `tls` or ` `                     |
| `limesurvey_smtp_debug`                            |           `false`           | SMTP debug option                                 |
| `limesurvey_admin_user`                            |         `admin`         | Admin nickname default                                         |
| `limesurvey_admin_password`                        |   :heavy_check_mark:    | Admin password                                                 |
| `limesurvey_admin_full_name`                       |       `Your Name`       | Full name of the administrator                                 |
| `limesurvey_admin_email`                           | `your.name@example.com` | Admin email address                                             |
| `limesurvey_mail_admin_name`                       |       `Your Name`       | Sender name for outgoing emails                                |
| `limesurvey_mail_admin_address`                     | `your.name@example.com` | Sender address of outgoing emails                               |
| `limesurvey_mail_bounce_address`                    | `your.name@example.com` | Email address for bounces                                       |
| `limesurvey_ldap_plugin_server_url`                |   :heavy_check_mark:    | Url to your ldap server                                                 |
| `limesurvey_ldap_plugin_server_port`               |          `389`          | Ldap port                                                 |
| `limesurvey_ldap_plugin_ldap_version`              |   :heavy_check_mark:    | Ldap version either `2` or `3`'                                                 |
| `limesurvey_ldap_plugin_opt_referrals`             |           `false`           | Select true if referrals must be followed (use false for ActiveDirectory)                                                |
| `limesurvey_ldap_plugin_tls`                       |           `false`           | Use tls either                                                |
| `limesurvey_ldap_plugin_ldap_mode`                 |   :heavy_check_mark:    | How limesurvey should connect to ldap either `simplebind` or `searchandbind`                                                 |
| `limesurvey_ldap_plugin_search_user_attribute`     |   :heavy_check_mark:    | Attribute to compare to the given login can be uid, cn, mail, ...                                                |
| `limesurvey_ldap_plugin_user_search_base`          |   :heavy_check_mark:    | List of Base DN for the user search operation.                                                 |
| `limesurvey_ldap_plugin_binddn`                    |   ` `   |Optional DN of the LDAP account used to search for the end-user's DN. An anonymous bind is performed if empty.                                                 |
| `limesurvey_ldap_plugin_bindpwd`                   |   ``    | Password of the LDAP account used to search for the end-user's DN if previoulsy set                                                 |
| `limesurvey_ldap_plugin_mail_attribute`            |   :heavy_check_mark:    | LDAP attribute of email address                                                |
| `limesurvey_ldap_plugin_full_name_attribute`       |   :heavy_check_mark:    | LDAP attribute of full name                                              |
| `limesurvey_ldap_plugin_is_default`                |           `false`           | Set to `1` to make ldap the default authentication method                                              |
| `limesurvey_ldap_plugin_auto_create`               |           `false`           | Automatically create user if it exists in LDAP server                                                 |
| `limesurvey_ldap_plugin_automatic_survey_creation` |           `false`           | Grant survey creation permission to automatically created users                                                 |
| `limesurvey_ldap_plugin_allow_initial_user`        |           `false`           | Allow initial user to login via LDAP                                              |
| `limesurvey_use_ldap`                              |         `false`         | Admin password                                                 |

## Example Playbook

```yml
```

## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).


## Author Information

- [Fritz Otlinghaus (Scriptkiddi)](https://github.com/scriptkiddi) _fritz.otlinghaus@stuvus.uni-stuttgart.de_
