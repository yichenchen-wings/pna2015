ifndef NOTEBOOK_PORT
  $(error NOTEBOOK_PORT is undefined: 8888 would be a common one)
endif

#------------------------------------------------------------------------------
# Launch the docker container and run the notebook
#
.PHONY: run
run: prebuild up

#------------------------------------------------------------------------------
# Launch the docker container and run the notebook
#
.PHONY: up
up:
	docker-compose up --force-recreate

#------------------------------------------------------------------------------
#pre-build the image
#
.PHONY: prebuild
prebuild:
	docker-compose build

#------------------------------------------------------------------------------
# Shell into the existing image/container
#
.PHONY: shell
shell: 
	docker-compose run --publish=${NOTEBOOK_PORT}:${NOTEBOOK_PORT} --entrypoint bash notebook



