# Axel

## Build
Via GitHub repository
```bash
$ docker build --tag alireaza/axel:$(date -u +%Y%m%d) --tag alireaza/axel:latest https://github.com/alireaza/axel.git
```

## Run
```bash
$ docker run \
--interactive \
--tty \
--rm \
--mount="type=bind,source=$(pwd)/udocker,target=/home/udocker" \
--name="axel" \
alireaza/axel \
"<File/Link>"
```

