# ansible-role-certbot #

An ansible role to install and configure certbot.

## Variables ##

The role uses the following variables (all are required):

| Variable                | Type            | Description |
|-------------------------|-----------------|-------------|
| `certbot_email_address` | string          | The recovery email address that will be registered with letsencrypt. |
| `certbot_accept_tos`    | bool            | Indicates that you've read and accepted the [letsencrypt TOS](https://letsencrypt.org/documents/LE-SA-v1.2-November-15-2017.pdf). |
| `certbot_domains`       | list of strings | Domains to get a certificate for. The first entry will be the name of the certificate. |
