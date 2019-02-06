DOCKER
====

DOCKER syntax
-----------

common arguments::

    -f file
    -t open a tty session
    -d start in daemon mode
    -v mount a volume
    --name name for the container
    -i interactive session
    -a all regardless of running state
    --no-trunc more information
    -q only display numeric ids

build an image::

    docker build -f Dockerfile .

build and image with tag::

    docker build -f Dockerfile -t registry_url:tag .

run a container::

    docker run image_name command_to_run

run a container with volume::

    docker run -v /path/to/dir/file:/path/to/dir/file image_name command_to_run

run a container as daemon::

    docker run -d image_name command_to_run

exec into a container with an interactive terminal::

    docker exec -it container_name command_to_run

list images::

    docker images

list running containers::

    docker ps

list all containers::

    docker ps -a

show docker logs::

    docker logs container_name

follow docker logs::

    docker logs -f container_name

show docker container stats::

    docker stats container_name

show all docker container stats::

    docker stats

stop running container::

    docker stop container_name

kill running container::

    docker kill container_name

remove stopped container::

    docker rm container_name

remove all untagged images::

    docker rmi $(docker images | grep "^<none>" | awk "{print $3}")

remove all dangling images::

    docker rmi $(docker images -f dangling=true -q)
