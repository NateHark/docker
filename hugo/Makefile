MAKEFILE_PATH := $(abspath $(lastword $(MAKEFILE_LIST)))
CWD := $(dir $(MAKEFILE_PATH))

DOCKER_REGISTRY := registry:5000

all:
	docker build --no-cache --tag hugo --tag hugo:$(HUGO_VERSION) --tag $(DOCKER_REGISTRY)/hugo $(CWD)
	docker push $(DOCKER_REGISTRY)/hugo