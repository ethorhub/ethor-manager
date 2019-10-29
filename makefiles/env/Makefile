ROOT_DIR:=$(shell dirname $(realpath $(lastword $(MAKEFILE_LIST))))

private_ENV := $(ROOT_DIR)/.private.env
include $(private_ENV)
export $(shell sed 's/=.*//' $(private_ENV))

public_ENV := $(ROOT_DIR)/.public.env
include $(public_ENV)
export $(shell sed 's/=.*//' $(public_ENV))

export _ENV_DIR=$(ROOT_DIR)
export _public_ENV=$(public_ENV)
export _private_ENV=$(private_ENV)