Скачиваем страничку mhtml. Смотрим описание

в docker-compose правим VIRTUAL_HOST ставим там наш домен

подымаем jira
```
docker-compose up -d
```


после установки, на моменте ввода ключа заходим в наш контейнер

```
docker exec -it jira bash
```

и выполняем команду:
```
java -jar /crack/atlassian-agent.jar -p jira -m admin@test.com -n MD -o http://test.com/ -s BLJN-UAPY-0SJL-STX6
```

получаем ключ и продолжаем установку


