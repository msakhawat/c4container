# create a volume for container

`$ docker volume create data_volume`

# attach volume with container(aka volume mounting)

old way

`$ docker run -v data_volume:/var/lib/mysql mysql`

# attach folder to container(aka bind mounting)

old way

`$ docker run -v /data/mysql:/var/lib/mysql mysql`

new way

`$ docker run --mount type=bind source=/data/mysql, target=/var/lib/mysql mysql`

