---
sidebar_position: 1
---

# Installing Radicle

## What is Radicle?
Radicle is an open-source peer-to-peer software collaboration tool. It's similar to github, but P2P.

More details can be found here [https://radicle.xyz/](https://radicle.xyz/).

## How to Install Radicle?

:::note
Requirements: 
You will need these installed to use Radicle.
* Linux or MacOS (not available on Windows at this time)
* Cmake
* Cargo
* pkg-config
* libssl-dev
* Git 2.34.0 or later
:::

Full instructions for the installation can be found [here](https://docs.radicle.xyz/getting-started). 

Here is an overview of the instructions:

* Install the above requirements.
* Run `cargo install --force --locked --git https://seed.alt-clients.radicle.xyz/radicle-cli.git radicle-cli`
* Run `rad auth` to Initialize your profile (create your identity). You will need to re-run this command each time you reboot to login into your profile.
* Install the Upstream client, download it [here](https://radicle.xyz/tryit).
* Run `chmod +x ./radicle-upstream-0.3.1.AppImage`
* Run `./radicle-upstream-0.3.1.AppImage` to start the upstream client
* Update your path, by adding `export PATH="$HOME/.radicle/bin:$PATH"` to `~/.profile`, `~/.zshrc`, `~/.bashrc`, etc. Restart your terminal.
* Verify that you can access upstream, by running `which upstream` and `which git-remote-rad` (you're looking for something like:
`/Users/rudolfs/.radicle/bin/upstream` or `which git-remote-rad
`/Users/rudolfs/.radicle/bin/git-remote-rad`)

 
## How to Create a Project on Radicle


## How to Add Team Members to Project

## How to Create Patch


:::note
Radicle repo for this project:
:::
 