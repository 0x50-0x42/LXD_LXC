# Snapshots

A snapshot is a copy of a virtual machine taken at a specific point in time. Snapshots are useful for restoring a VM to a certain point in the event of a system failure or error.

Now, I have my container running, as seen here:

```bash
$ lxc list
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
|   NAME    |  STATE  |         IPV4          |                     IPV6                      |   TYPE    | SNAPSHOTS |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
| linuxMint | RUNNING | 10.116.202.111 (eth0) | fd42:8b74:9e00:35ab:216:3eff:feac:5cf3 (eth0) | CONTAINER | 0         |
+-----------+---------+-----------------------+-----------------------------------------------+-----------+-----------+
```


---