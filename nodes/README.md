# Nodes

Drop your nodes definition as `yaml` files with the `.yml` extension in this folder.

Note that the `id` in the node definition must match the filename.

# Documentation

Documentation about the nodes is available in the [docs.devo.ps website](http://docs.devo.ps/manual/nodes/).

Documentation about the services and providers is available in their respective sections.

# Example

    id: my-node
    name: My Node
    type: server

    provider:
      name: digitalocean
      size: 66
      location: 3
      image: ubuntu14.04

    services:
      nodejs: '*'
      redis: '*'

