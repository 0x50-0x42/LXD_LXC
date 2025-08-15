# Images and remote repositories

`lxd` is able to pull images from remote servers. To find out which remote servers we have available, the following command is used:

```bash
$ lxc remote list
```

This command[^1] basically gives us a list of available remote servers in tabular format.

We can also list the contents (the images available) of a remote server via the following command:

```bash
lxc image list images:
```

With this command we are listing the images in the `images` repository (put the repository name that you got by running `lxc remote list` command). If we were searching for specific image then we will have to mention it explicitly as follows:

```bash
lxc image list images: mint
```

Here we are interested in images that have `mint` in the name (\[**Note**: The images are displayed in table format and there is one column named `TYPE`, make sure that you only select the images which are `CONTAINER`s). You can certainly add more than one keyword when searching for a particular image.


[^1]:The command used here is `lxc` and not `lxd`. `lxc` is the container type and `lxd` is the management layer.



---