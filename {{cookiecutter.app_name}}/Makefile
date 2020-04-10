# Housekeeping

lint:
	black . --line-length=120

clean:
	find . -name '*.pyc' -delete

# Local Development

build:
	docker-compose build {{cookiecutter.app_name}}

run:
	docker-compose run --service-ports {{cookiecutter.app_name}}

shell:
	docker-compose run --service-ports {{cookiecutter.app_name}} bash

# Local Validation

build-validate:
	docker-compose build validate

test:
	docker-compose run validate pytest

flake:
	docker-compose run validate flake8

type-check:
	docker-compose run validate mypy ./app

vulnerability-check:
	docker-compose run validate safety check