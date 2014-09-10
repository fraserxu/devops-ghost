# Tasks

Drop your tasks definition as `yaml` files with the `.yml` extension in this folder.

Note that the `id` in the node definition must match the filename.

# Documentation

Documentation about the tasks is available in the [docs.devo.ps website](http://docs.devo.ps/manual/tasks/).

# Example

    id: my-task
    name: My Task
    type: task
    
    triggers:
      webhooks:
        - path: some/custom/path

    vars:
      workspace: /opt/folder

    targets:
      - my-node

    steps:
      - run: mkdir {{ workspace }}
      - run: devops package task_name
      - run: devops scripts/some-script.sh
