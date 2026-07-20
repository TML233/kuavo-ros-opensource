.PHONY: build xhostallow up down

build:
	docker compose build

xhostallow:
	export DISPLAY="$${DISPLAY:-:0}" && xhost +

up: xhostallow
	docker compose up -d

down:
	docker compose down