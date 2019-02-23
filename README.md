# Kevpress - Docker

Faça o clone do repositório:

```shell
git clone git@github.com:kvnol/kevpress-docker.git --recurse-submodules
```

Entre na pasta "Docker" e rode
```docker-compose up -d```

Limpe os dockers abertos com
```docker stop $(docker ps -a -q)```

Dê start no Docker
```docker-compose up -d```

Rode o banco de dados
```while ! docker-compose exec mysql mysqladmin --user=root --password=root --host "127.0.0.1" ping --silent &> /dev/null ; do```