# docker-ds
Personal docker environment for data science

## Installation

Currently the images are not available on Docker Hub but soon they will be.

## Usage

There are two images available:

### CPU

#### Build CPU image

```sh
$ docker-compose --file docker-compose.cpu.yml build
```

#### Run CPU container

```sh
$ docker-compose --file docker-compose.cpu.yml run datascience
```

### GPU

#### To build GPU image

```sh
$ docker-compose --file docker-compose.gpu.yml build
```

### To run container with GPU image

Currently `docker-compose` does not support [runtime in file version `3`](https://github.com/docker/compose/pull/5405). Hence docker-compose file version used is `2.3`.

```sh
$ docker-compose --file docker-compose.gpu.yml run datascience
```

## License
[MIT](https://github.com/ManrajGrover/docker-ds/blob/master/LICENSE) © Manraj Singh
