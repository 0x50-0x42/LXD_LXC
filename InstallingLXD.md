# Installing `LXD`

Before installing `lxd` on your machine, make sure that you have `snapd` installed in your system as it will be used to install the `lxd` command (refer to the video provided in [README.md](https://github.com/0x50-0x42/LXD_LXC/blob/LearnLXD/README.md)).

Once, you have installed `snapd`, you can install `lxd` using the following command:

```bash
$ sudo snap install lxd
```

To view a list of installed packages using `snap`, you can run the following command:

```bash
$ snap list
```

Once you have installed `lxd`,  it's recommended that you add yourself to the `lxd` group via the following command:

```bash
$ sudo usermod -aG lxd <your username>
```

This command will enable you to  interact with `lxd` without having to use `sudo`. Don't forget to logout and log back in once you have added yourself to the group because group memberships are read as soon as you log in. TL;DR logout and log back in for the changes to take effect.

After you have logged back in, just run the `groups` commands to view the groups that you are a member of:

```bash
$ groups
sepoy adm dialout sudo lpadmin lxd
```



---