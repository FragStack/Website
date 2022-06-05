---
sidebar_position: 4
---

# Installing IPFS Cluster Follower
## Installing IPFS Cluster Follower?
The `ipfs-cluster-follow` is a command line application which runs an IPFS Cluster follower peer, allowing users to easily join and be part of collaborative clusters.

## How to Install IPFS Cluster Follower?
You can download this package [here](https://dist.ipfs.io/#ipfs-cluster-follow). The Docs for installing `ipfs-cluster-follow` can be found next to the download link or [here](https://cluster.ipfs.io/documentation/reference/follow/).

:::note
You will need IPFS running to use IPFS Cluster Follower. It's recommended to have `ipfs-cluster-ctl` installed as well.
:::
 
### Linux Installation
* After you downloaded the above package. Run `tar -xvf ipfs-cluster-follow_v1.0.1_linux-amd64.tar.gz`
* Run `cd ipfs-cluster-follow`
* Copy the `ipfs-cluster-follow` to the bin folder, ex. `cp ipfs-cluster-follow /usr/local/bin/`
* You can verify installation by running `ipfs-cluster-follow --version`

For FragStack team members, Run `ipfs-cluster-follow ipfs-cluster init /ip4/ip/ipfs/`. This will create a folder `~/.ipfs-cluster-follower/ipfs-cluster/`. A copy of `service.json` file is provided for our cluster. You will need to update the `peername` in this file and copy it to `$HOME/.ipfs-cluster-follower/ipfs-cluster/`

Run `ipfs-cluster-follower ipfs-cluster run` to start the follower.