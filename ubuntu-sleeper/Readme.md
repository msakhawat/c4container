build docker image

`$ docker build -t ubuntu-sleeper:1.0 .`

build docker container from this image with default value of sleep(5)
`$ docker run ubuntu-sleeper`

build docker container from this image with custom value of sleep(10)
`$ docker run ubuntu-sleeper 10`

build docker container from this image, changing entrypoint from 'sleep' to 'sleep2' and provide a custom value to the command(10)
`$ docker run --entrypoint sleep2  ubuntu-sleeper 10`