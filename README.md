# Laravel Docker Compose

## Laravel 다운로드

```
git clone https://github.com/ssh521/laravel-nginx-docker.git

cd laravel-nginx-docker
```

## 라라벨 프로젝트를 위한 Docker Compose 구성

```
.
├── Dockerfile
├── docker-compose.yaml
└── nginx
    └── default.conf
```

## 라라벨 프로젝트 세팅하기

```
composer install
npm install
cp .env.example .env
php artisan key:generate
php artisan migrate
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

## 컨테이너 재시작

```
docker compose restart
```

## 컨테이너 로그 확인

```
docker compose logs
```

## 회원 로그인 추가하기 Breeze
```
docker-compose exec php composer require laravel/breeze --dev
docker-compose exec php php artisan breeze:install
docker-compose exec php php artisan migrate
```