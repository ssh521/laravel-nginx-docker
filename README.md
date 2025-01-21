# Laravel Docker Compose

라라벨 프로젝트를 위한 Docker Compose 환경 설정

```
.
├── Dockerfile
├── docker-compose.yaml
└── nginx
    └── default.conf
`
```

## Laravel 다운로드

```
composer create-project laravel/laravel laravel-nginx-docker

cd laravel-nginx-docker
```

## Docker Compose 실행

```
docker compose up -d
```

## 컨테이너 접속

```
docker compose exec php bash
```


## 컨테이너 종료

```
exit
```

## 컨테이너 삭제

```
docker compose down
```
