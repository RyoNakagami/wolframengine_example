## Prerequisites

- [docker set-up for wolfram_jupyterserver](https://github.com/RyoNakagami/wolfram_jupyterserver)

## Usage

```zsh
### START
docker run \
  --rm \
  -ti \
  --publish 8888:8888 \
  --user $(id -u $USER):$(id -g $USER) \
  --volume $PWD:/home/docker/work \
  ryonak/wolfram-jupyterserver:latest
```

If you want to stop the service, just `ctrl` + `c`.
