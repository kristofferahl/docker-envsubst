# Envsubst in docker

## Usage

    declare input="Image: kristofferahl/envsubst. Version: \${VERSION}."
    docker run --rm -e "VERSION=1.0.1" kristofferahl/envsubst "$input"

NOTE: Use quotes for input to preserve newline characters

## Build

    ./koshu.sh docker:build

## Test

    ./koshu.sh docker:test
