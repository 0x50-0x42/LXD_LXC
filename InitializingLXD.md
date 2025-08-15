# Initializing `LXD`

Now that we are done with installing `lxd`, we have to initialize it via the following command:

```bash
$ sudo lxd init
```

Once, you press ENTER, it will ask you a series of questions, as a response to which you can simply press ENTER. There will be one particular question that will be asked to you which will be this:

```
Name of the storage backend to use (zfs, ceph, btrfs, dir, lvm) [default=zfs]:
```

For this one, it's highly recommended that you choose `zfs`, but you would need a dedicated drive in order to effectively manage `zfs`, so in this case, you should type `dir` if you don't have a dedicated device to manage `zfs` (in my case, I typed `dir` because I didn't have any dedicated device for `zfs`).


---