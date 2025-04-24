# Ping pong of a Docker container between two nodes

## Description

The Vagrantfile automatically generates two Ubuntu 24.04 virtual machines with Docker preinstalled. On each machine, a script named docker_start_stop.sh is created, which starts a container called echo-server, keeps it running for 60 seconds, and then stops it. The script is executed automatically via cron: on even minutes on node1, and on odd minutes on node2. This allows the container to run alternately between the two virtual machines. In this way, the container is started alternately on each machine. The resulting environment is useful for simulations, basic orchestration tests, or failover scenarios.







