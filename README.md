ECV PHP Project - Symfony3 (Docker)

### Includes
    
- Mysql 5.7.15
- Nginx 1.9.1
- PHP 7.0.7

### Installation
    
    1 - git clone https://github.com/Bramvanosta/ECV_PHP.git
    2 - Add '127.0.0.1 symfony.dev' to /etc/hosts
    3 - docker-compose up
    4 - docker exec -it symfony_php composer install
    5 - Enter these parameters when asked to configure the database
        - host : db
        - database name : symfony
        - user : root
        - password : root
    6 - Lauch brower on symfony.dev/app_dev.php

### Add remote PHP interpreter in PHPStorm

    In PHPStorm go to Settings ->  Languages & Frameworks -> PHP
    
    Add a new remote interpreter using the following SSH credentials
        - host: localhost
        - port: 2222
        - user: root
        - password: lbmonkey
