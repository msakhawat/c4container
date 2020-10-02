# Public Registry
repository where images are stored

`$ docker run nginx`

it means you are running

`$ docker run nginx/nginx`

or

`$ docker run docker.io/nginx/nginx`

to fetch an image stored on your account on docker.io

`$ docker run msakhawat/mysql`

google registry gcr.io

# Private Registory

before pulling image one must login to the private registry using below command

`$ docker login myprivateregistry.io`

this will will ask for credentials

run from private registry

`$ docker run myprivateregistry.io/apps/internal-app`




