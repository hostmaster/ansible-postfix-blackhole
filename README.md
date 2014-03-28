ansible-postfix-blackhole
=========================

This is a role for ansible  playbook. It configures postfix smtp server as a email blackhole with configurable list of forwarded emails.

### Example

```yaml
    - role: blackhole
      mail_domain: 'domain.tld'
      admin_user: '{{ my_user }}'
      aliases:
        - { key: 'sub56',  value: 'myrealemail@gvail.tld' }
        - { key: 'fwd38',  value: 'myrealemail@yahoo.something' }
```
