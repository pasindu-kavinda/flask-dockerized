#!/usr/bin/make

SHELL = /bin/sh

UID := $(shell id -u)
GID := $(shell id -g)

export UID
export GID

shell:
	docker exec -it python-app sh

up:
	UID=$(UID) GID=$(GID) docker compose -f docker-compose.yml up -d --build --remove-orphans

up-f:
	UID=$(UID) GID=$(GID) docker compose -f docker-compose.yml up --build --remove-orphans

down:
	docker compose -f docker-compose.yml down --remove-orphans
