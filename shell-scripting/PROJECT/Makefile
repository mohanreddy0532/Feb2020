.ONESHELL:
.SHELL := /usr/bin/bash
.PHONY: all ROBO-Shop

help:
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[35m%-10s\033[0m %s\n", $$1, $$2}'


all: ## Install all Components of Application
	@sh ROBO-Shop.sh all


mongodb: ## Install MongoDB for Application
	@sh ROBO-Shop.sh mongodb

rabbitmq: ## Install RabbitMQ for Application
	@sh ROBO-Shop.sh rabbitmq

mysql: ## Install MySQL for Application
	@sh ROBO-Shop.sh mysql

redis: ## Install Redis for Application
	@sh ROBO-Shop.sh redis

