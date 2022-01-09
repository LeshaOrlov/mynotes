# Dockerfile
Created вторник 16 Февраль

Комментарии
```docker
# Comment
```

Базовый образ
```docker
FROM ImageName
FROM python:3.6
```

ENV Инструкция устанавливает переменную окружения <key>к значению <value>
```docker
ENV <key>=<value>
ENV MY_NAME="John Doe"
```

Выполнить команду
```docker
RUN mkdir -p /usr/src/app/
```

Перейти в деррикторию
WORKDIR Инструкция устанавливает рабочий каталог для любых RUN, CMD, ENTRYPOINT, COPYи ADD инструкции , которые следуют за ним в Dockerfile. Если WORKDIR не существует, он будет создан, даже если он не будет использоваться в последующих Dockerfile инструкциях.
```docker
WORKDIR /usr/src/app/
```

Копируем файлы из гостевой ос в контейнер
```docker
COPY . /usr/src/app/
```



```docker
WORKDIR /usr/src/app/
```

```docker
EXPOSE <port> [<port>/<protocol>...]
```
В EXPOSE инструкции сообщает Docker , что контейнер прослушивает на указанных сетевых портов во время выполнения. Вы можете указать, будет ли порт прослушивать TCP или UDP, и по умолчанию используется TCP, если протокол не указан.
EXPOSE 80/tcp

```docker
CMD
ENTRYPOINT
ADD
VOLUME
EXPOSE


LABEL
STOPSIGNAL
USER
```

       

