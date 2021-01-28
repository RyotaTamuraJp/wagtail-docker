tail = 500

setup:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml build --no-cache
build:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml build
up:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml up -d

exec-app:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml exec wagtail /bin/bash || true
exec-db:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml exec db /bin/ash || true

start:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml start
stop:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml stop
down:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml down

logs-app:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml logs wagtail --tail=${tail}
logs-db:
	docker-compose -f ./docker-compose.yml -f ./docker-compose.dev.yml logs db --tail=${tail}