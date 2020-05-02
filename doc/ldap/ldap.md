# install ldap on ubuntu 14.04.6
```sh
sudo apt install slapd ldap-utils

sudo dpkg-reconfigure slapd

sudo apt-get install phpldapadmin
```
---
check running status
```sh
ps auxw | grep slapd

netstat  -an | grep 389

ldapsearch -h 127.0.0.1  -p 389 -x  -b dc=he,dc=org
```


http://127.0.0.1/phpldapadmin

---
phpldapadmin show some error:
> Error trying to get a non-existant value (appearance,password_hash)

how to fix it:

> sudo vi  /usr/share/phpldapadmin/lib/TemplateRender.php

> change from: $default = $this->getServer()->getValue('appearance','password_hash');

> to: $default = $this->getServer()->getValue('appearance','password_hash_custom');
