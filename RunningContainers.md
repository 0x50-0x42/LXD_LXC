# Running containers

To view the containers that we have currently running, use the following command:

```bash
$ lxc list
```

If you have no containers running, you can create one via the `lxc launch` command to create a container from an image (provided as an argument to the launch command) as follows:

```bash
$ lxc launch images:mint/21.3 linuxMint
```

Here `images` is the repository of our choice and `mint/21.3` is one of its images. `linuxMint` is the name that we gave to the container. This command basically "pulls" (in Docker terms) the image `mint/21.3` from the `images` repository and creates the `linuxMint` container and starts it. So, if we use the `lxc list` command, then this we will see the container running.

To execute a command in the container like so:

```bash
$ lxc exec linuxMint -- bash
```

Here, we are basically executing the `bash` command on the `linuxMint` container which means that it will open up the bash prompt in the container. The two dashes `--` basically acts as a separator between the `lxc` command and the command that we want to execute against the container.


---