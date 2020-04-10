# {{cookiecutter.app_name}}

## Running

Enter the container and run:

    python app/main.py

## Local Development

Clone this repo, then build the image and enter a shell in that image:

    make run

### Validation Steps

#### Running tests

Enter the container and run:

    make test

#### Running type validation

Enter the container and run:

    make type-check

#### Running vulnerability checks

Enter the container and run:

    make vulnerability-check
