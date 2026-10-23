.PHONY: build xhostallow up down start stop restart

build:
	docker compose build

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