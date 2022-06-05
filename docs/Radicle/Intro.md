---
sidebar_position: 1
---

# Installing Radicle

## What is Radicle?
Radicle is an open-source peer-to-peer software collaboration tool. It's similar to github, but P2P.

More details can be found here [https://radicle.xyz/](https://radicle.xyz/).


:::note
FragStack Website is pushed to `maple.radicle.garden`:

   * (web) https://app.radicle.network/seeds/maple.radicle.garden/rad:git:hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o
   * (git) https://maple.radicle.garden/hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o.git
:::


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
To create a repo or a project on radicle, you need to run `rad init`.

Enter the following info:
* Project Name 
* Description 
* default branch

You can run `rad .` to get the project id.

:::note
The project id for FragStack Website is:
    `rad:git:hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o`
:::

Run `rad push` to push your project to one of the networks (ex.`maple.radicle.garden`).

:::note
FragStack Website is pushed to `maple.radicle.garden`:

   * (web) https://app.radicle.network/seeds/maple.radicle.garden/rad:git:hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o
   * (git) https://maple.radicle.garden/hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o.git
:::

## How to Clone a Project
You can clone a project by using the `rad clone rad://<seed-id>/<project URN>` command. 

For FragStack Team members, clone the project by running `rad clone rad://maple.radicle.garden/hnrkqgxwcc6131omr5cmwbanshdy796cn6o3o`

## How to Create Patch/Submit your changes
Full instructions can be found []here(https://docs.radicle.xyz/using-radicle/create-submit-patch). 

First create a new branch for the changes you want to make to the main project. You can do this by running the command:

```
git checkout --branch my-proposed-changes 
git add *
git commit -m'my proposed changes'
```
If you're maintaining your report on github as well, you'd want to do a `git push` here.

Now create a radicle patch by using `upstream`:

```
upstream patch create

```

Use `upstream patch update` to update the patch after creating it.

:::note
You'll need to share your Peer ID with the delegate so that they can track your patch in Upstream.
:::


## How to Apply a Patch

If you go to the Radicle client, you can click the patch tab and click on `Merge Patch`. It will give you the commands you need to do a merge.

Here are an example commands:

```
upstream patch fetch hybjocw8c9k7f7dh38ybsx6d33bz5p54q9nba3i5gt5qt6di887hwk/docsUpdate
git merge radicle-patch/hybjocw8c9k7f7dh38ybsx6d33bz5p54q9nba3i5gt5qt6di887hwk/docsUpdate
rad push
```
