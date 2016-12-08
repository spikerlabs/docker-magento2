##Build environment
```
docker-compose -f docker-compose.yaml -f docker-compose-dev.yaml up -d
```

##Install magento 2
```
docker-compose exec app sh /root/scripts/install.sh
docker-compose exec app sh /root/scripts/refresh.sh
```

##Stop stack
```
docker-compose stop
```

##Start stack after stop
```
docker-compose start
```

###SSH Into boxes
```
docker-compose exec app /bin/bash
docker-compose exec server /bin/bash
docker-compose exec database /bin/bash
```