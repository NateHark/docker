MAKEFILE_PATH := $(abspath $(lastword $(MAKEFILE_LIST)))
CWD := $(dir $(MAKEFILE_PATH))

all:
	docker build --tag aws $(CWD)
