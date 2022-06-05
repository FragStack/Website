---
sidebar_position: 3
---

# Installing IPFS Cluster Ctl
## What is IPFS Cluster Ctl?
The `ipfs-cluster-ctl` is a command line application. It is a user-friendly REST API client for IPFS Cluster. It allows to perform all the operations supported by a Cluster peer. Here is a list of these actions:

* Pinning
* Unpinning
* Adding
* Listing items in the pinset
* Checking the status of pins
* Listing cluster peers
* Removing peers


## How to Install IPFS Cluster Ctl?
You can download this package [here](https://dist.ipfs.io/#ipfs-cluster-ctl). The Docs for installing `ipfs-cluster-ctl` can be found next to the download link or [here](https://github.com/ipfs/ipfs-cluster/blob/v1.0.1/README.md).

:::note
You will need IPFS and IPFS Cluster Services running to use IPFS Cluster Ctl.
:::
 

### Linux Installation
* After you downloaded the above package. Run `ipfs-cluster-ctl_v1.0.1_linux-amd64.tar.gz`
* Run `cd ipfs-cluster-ctl`
* Copy the `ipfs-cluster-ctl` to the bin folder, ex. `cp ipfs-cluster-ctl /usr/local/bin/`
* You can verify installation by running `ipfs-cluster-ctl --version`
