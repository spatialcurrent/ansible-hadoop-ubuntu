# ansible-hadoop-ubuntu

# Description

**ansible-hadoop-ubuntu** is a simple [Ansible](https://www.ansible.com/) role for installing [Hadoop](https://hadoop.apache.org/) on an Ubuntu machine.

# Usage

If installing a unified [Hadoop](https://hadoop.apache.org/) instance for [Accumulo](https://accumulo.apache.org/) or other big data applications, be sure to provision Zookeeper first.  Many big data applications don't package their own Zookeeper JARs and require zookeeper to be installed on every node, even if zookeeper is disabled.  For example, something like this:

```
...
roles:
  - ansible-java-ubuntu
  - ansible-zookeeper-ubuntu
  - ansible-hadoop-ubuntu
...
```

# Contributing

[Spatial Current, Inc.](https://spatialcurrent.io) is currently accepting pull requests for this repository.  We'd love to have your contributions!  Please see [Contributing.md](https://github.com/spatialcurrent/ansible-hadoop-ubuntu/blob/master/CONTRIBUTING.md) for how to get started.

# License

This work is distributed under the **MIT License**.  See **LICENSE** file.
