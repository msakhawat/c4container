Docker creates 3 networks automatically

# list the available network in your docker environment
`$ docker network ls`
# bridge
this is the default network. to use the default you don't have to provide any network info in docker run command

`$ docker run ubuntu`

if you want to specify network for you container use

`$ docker run -network=blah-net`

private internal network.
get internal ip(usually 172.17.0.2)
to access from outside you have to map the port on the container to port of the host
# none
private container, not access to network, runs in an isolated network
`$ docker run -network=none ubuntu`
# host
`$ docker run -network=host ubuntu`

# create you own network
below will create a network using default bride driver and use 182.18.0.0.0/16 subnet

`$ docker create network --driver bridge --subnet 182.18.0.0.0/16 dev-net`

# inspect container to check network settings
`$ docker inspect myubuntu`

