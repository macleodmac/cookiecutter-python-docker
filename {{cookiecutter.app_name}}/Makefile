lint:
	black . --line-length=120

clean:
	find . -name '*.pyc' -delete

build:
	docker-compose build {{cookiecutter.app_name}}

run:
	docker-compose run --service-ports {{cookiecutter.app_name}}

shell:
	docker-compose run --service-ports {{cookiecutter.app_name}} bash

build-test:
	docker-compose build test

test:
	docker-compose run test pytest
