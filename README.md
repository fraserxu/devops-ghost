# Ghost

Setting up **two** [ghost](ghost.org) blogs with [devo.ps](devo.ps) on **one** digitalocean box.

## Install

Simply use the link below:

[![Fork on devo.ps](https://app.devo.ps/assets/images/fork.png)](https://app.devo.ps/#/fork?git_url=https://github.com/fraserxu/devops-ghost)

Once you've forked the repository, open it in devo.ps and you will be prompted for a few settings, including the Git URL for the code of your application.

To deploy your app, you will need to navigate to the tasks page of the repo and run the task manually (click on "play" icon, right of the "Install ghost app" task).

## What's in the box?

This setup contains one server (`nodes/new-node.yml.sample`) with **Nginx**, **Nodejs**.

We have included as well a task (`tasks/install_ghost.yml`) that:

1. Download and install ghost.
2. start server with forever.

The current repo provides a very simple setup. Hack at will!

# Reference

- [Nodes in devo.ps](http://docs.devo.ps/manual/nodes)
- [Tasks in devo.ps](http://docs.devo.ps/manual/tasks)