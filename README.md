# Упаковка в Docker Compose

Проект для упаковки приложения js-fastify-blog в Docker образ.
Docker Compose используется для настройки окружения для разработки, запуска тестов и CI. После успешного выполнения CI собирается образ приложения и публикуется на hub.docker.com.

## Требования
docker

docker compose V2

make

## Образ
Dockerhub - https://hub.docker.com/repository/docker/plsn/example-app
Обновление образа происходит по workflow на действие push в ветке main.

## Сборка
_Команды для сборки окружения находятся в файле Makefile_
### Продакшен сборка docker
В docker-compose.yml сборка происходит с использованием образа для продакшена. Копирование файлов внутрь образа происходит в Dockerfile.production.

`make up`

### Для запуска тестов docker
`make test`

## Бейдж

### Hexlet tests and linter status:
[![push app](https://github.com/anna-plsn/devops-for-programmers-project-74/actions/workflows/push.yml/badge.svg)](https://github.com/anna-plsn/devops-for-programmers-project-74/actions/workflows/push.yml)
[![Actions Status](https://github.com/anna-plsn/devops-for-programmers-project-74/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/anna-plsn/devops-for-programmers-project-74/actions)
