MAKEFILE_PATH := $(abspath $(lastword $(MAKEFILE_LIST)))
CWD := $(dir $(MAKEFILE_PATH))

DOCKER_REGISTRY := registry:5000

all:
	docker build --no-cache --tag aws --tag $(DOCKER_REGISTRY)/aws $(CWD)
	docker push $(DOCKER_REGISTRY)/aws