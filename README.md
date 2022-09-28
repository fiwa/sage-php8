# sage-php8

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
>>>>>>> 69e78a1dc81415339111d40fe294fc679b1b3e4b
