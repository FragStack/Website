---
sidebar_position: 1
---

# Installing IPFS
## What is IPFS?
A peer-to-peer hypermedia protocol designed to preserve and grow humanity's knowledge by making the web upgradeable, resilient, and more open. Read more [here](https://ipfs.io/#how) to understand how IPFS works.

## How to Install IPFS?
The best way to install IPFS is to install `ipfs-update` package.  You can download this package [here](https://dist.ipfs.io/#ipfs-update). The Docs for installing `ipfs-update` can be found next to the download link.

### Linux Installation
* After you downloaded the above package. Run `tar -xvf ipfs-update_v1.8.0_linux-amd64.tar.gz`
* Run `.\ipfs-update\install.sh`. This will copy ipfs-update file that has been extracted to `\bin` folder.
* You can verify installation by running `ipfs-update --version`
* To install the latest version of `ipfs` you need to run `ipfs-update install latest`
* Run `ipfs daemon` to run ipfs as a daemon.
  