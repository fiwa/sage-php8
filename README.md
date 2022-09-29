# sage-php8

Based on discussion in https://discourse.roots.io/t/sage-9-php-8-0/22485.

## Local development in VVV

#### 1. Setup VM:
1. Clone repo into [local VVV path]/www

2. Add site to your config/config.yml

```
  sage9-php8:
    nginx_upstream: php80
    hosts:
      - sage9-php8.test
```

3. Reprovision with `vagrant reload --provision`

### 2. Install theme dependencies and build assets

```sh
$ cd web/app/themes/sage
$ nvm use # Makes sure you use the node version specified in .nvmrc (if you use nvm)
$ yarn && yarn build
```

### 3. Access:

Access the website: `https://sage9-php8.test`

Access WordPress admin: `https://sage9-php8.test/wp/wp-admin/`

Default user:

```
username: admin
password: password
```
