# Additional commands

To stop running a particular container, use the following command:

```bash
$ lxc stop <container name>
```

The command will the stop the container that you have specified in the command.
Replace `<container name>` with the name of the container to be stopped, for example:

```bash
$ lxc stop linuxMint
```

To start it back, simply write:

```bash
$ lxc start <container name>
```

Example:

```bash
$ lxc start linuxMint
```

Restarting a container is also possible via the following command:

```bash
$ lxc restart <container name>
```

Example:

```bash
$ lxc restart linuxMint
```


---