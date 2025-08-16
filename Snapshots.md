# Snapshots

A snapshot is a copy of a virtual machine taken at a specific point in time. Snapshots are useful for restoring a VM to a certain point in the event of a system failure or error.

Now, I have my container `linuxMint` running, as seen here:

```bash
$ lxc list
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
|   NAME    |  STATE  |         IPV4          |                     IPV6                      |   TYPE    | SNAPSHOTS |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
| linuxMint | RUNNING | 10.116.202.111 (eth0) | fd42:8b74:9e00:35ab:216:3eff:feac:5cf3 (eth0) | CONTAINER | 0         |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
```

Notice that the `SNAPSHOTS` column has the number $0$ indicating that I currently have no snapshots of this container.

To create a snapshot, type the following command:

```bash
$ lxc snapshot linuxMint mysnap1
```

`mysnap1` is the name of my snapshot. I can use `lxc list` command again to view the status of my container:

```bash
$ lxc list
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
|   NAME    |  STATE  |         IPV4          |                     IPV6                      |   TYPE    | SNAPSHOTS |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
| linuxMint | RUNNING | 10.116.202.111 (eth0) | fd42:8b74:9e00:35ab:216:3eff:feac:5cf3 (eth0) | CONTAINER | 1         |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
```

Here, in the `SNAPSHOTS` column, we can see that there is a number $1$ indicating that we have one snapshot. I will create another snapshot using the same command again:

```bash
$ lxc snapshot linuxMint mysnap2
```

The number of snapshots will be updated to $2$ when we will run the `lxc list` command.


---