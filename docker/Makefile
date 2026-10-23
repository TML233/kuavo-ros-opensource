.PHONY: build buildx xhostallow up down start stop restart

build:
	docker compose build

buildx:
	docker buildx bake -f docker-compose.yml --allow=network.host --load

xhostallow:
	export DISPLAY="$${DISPLAY:-:0}" && xhost +

up: xhostallow
	docker compose up -d

down:
	docker compose down

start:
	docker compose start

stop:
	docker compose stop

restart:
	docker compose restart