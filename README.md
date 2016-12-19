# Ansible Role: Docker role

Tools:

    - docker-engine
    - docker-compose

## Role Variables

Available variables are listed below, along with default values:

    docker_opts: "--selinux-enabled -H tcp://0.0.0.0:2376 -H unix:///var/run/docker.sock"
    docker_bridge_ip:
    docker_mirror_host:
    docker_mirror_protocol: "https"
    docker_mirror_port: 5000
    docker_compose_version: 1.9.0

## Example Playbook

    - hosts: servers
      roles:
         - { role: bezrukovp.docker }

## License

MIT
