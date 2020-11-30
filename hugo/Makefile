MAKEFILE_PATH := $(abspath $(lastword $(MAKEFILE_LIST)))
CWD := $(dir $(MAKEFILE_PATH))

all:
	docker build --no-cache --build-arg hugoVersion=$(HUGO_VERSION) --tag hugo --tag hugo:$(HUGO_VERSION) $(CWD)
