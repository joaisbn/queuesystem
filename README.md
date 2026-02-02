# docker-lamp
https://github.com/jcavat/docker-lamp

# Mailhog
https://gist.github.com/dipenparmar12/4e6cd50d8d1303d5e914742f62659116

# docker-compose.yml
# at www: add php.ini volume line
# - ./php.ini:/usr/local/etc/php/php.ini

# docker cp queuesystem-www-1:/usr/local/etc/php/php.ini-development ./php.ini

# If we see something like following means everyting is working fine and ready to go. 
# Visit http://0.0.0.0:8025/ where we receive all mails.

# ############################
# docker-lamp

Docker example with Apache, MySql 8.0, PhpMyAdmin and Php

- You can use MariaDB 10.1 if you checkout to the tag `mariadb-10.1` - contribution made by [luca-vercelli](https://github.com/luca-vercelli)
- You can use MySql 5.7 if you checkout to the tag `mysql5.7`

I use docker-compose as an orchestrator. To run these containers:

```
docker-compose up -d
```

Open phpmyadmin at [http://localhost:8000](http://localhost:8000)
Open web browser to look at a simple php example at [http://localhost:8001](http://localhost:8001)

Run mysql client:

- `docker-compose exec db mysql -u root -p` 

Enjoy !
