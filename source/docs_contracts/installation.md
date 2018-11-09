title: Installation
---

## Prerequisites

In order to make Embark work in your computer, we need to have some tools installed first. Make sure you have the following ready and in the correct version:

- [Node](#Node)
- [Ethereum Client](#Ethereum-Client-Optional)

Once done, go ahead and [install Embark](#Installing-Embark).

### Node

Please install [Node.js](http://nodejs.org/) in version 8.11.3 LTS or higher.

{% note info Quick tip: %}
**We recommend installing Node using the [Node Version Manager](https://github.com/creationix/nvm/blob/master/README.md).**  This is because it makes it very easy to install different versions of Node in isolated environments that don't require users to [change their permissions](https://docs.npmjs.com/getting-started/fixing-npm-permissions) when installing packages. Find instructions on how to install NVM [here](https://github.com/creationix/nvm/blob/master/README.md#install-script).

Once that is done, you can install and select a specific Node version or use the `--lts` option to get the latest version with long term support like this:

<pre><code class="shell">$ nvm install --lts
$ nvm use --lts
</code></pre>

{% endnote %}

### Ethereum Client (Optional)

Embark can spin up an Ethereum node for you. To make this happen, an Ethereum client has to be installed on your machine as well. Embark already comes with [Ganache CLI](https://truffleframework.com/ganache), a blockchain node emulator, which is accessible via [Embark's simulator](embark_commands.html#simulator) command.

In case you want to run a real node, [geth](https://geth.ethereum.org/) is a pretty good one. Check out the [installation guide](https://ethereum.github.io/go-ethereum/install/) for your platform and verify your installation with:

<pre><code class="shell">$ geth version</code></pre>

Which should result in an output that looks like this (note that the exact version numbers may be different):
<pre><code class="shell">Geth
Version: 1.8.15-stable
Git Commit: 89451f7c382ad2185987ee369f16416f89c28a7d
Architecture: amd64
Protocol Versions: [63 62]
Network Id: 1
Go Version: go1.10.4
Operating System: darwin
GOPATH=
GOROOT=/Users/travis/.gimme/versions/go1.10.4.darwin.amd64
</code></pre>

## Installing Embark

Alright, let's install Embark so we can build our first application. As mentioned earlier, if anything is unclear or you run into problems, make sure to reach out to us on our dedicated channels, [submit an issue on  GitHub](https://github.com/embark-framework/embark/issues), or take a look at our [troubleshooting guide](troubleshooting.html).

We can install Embark using the Node Package Manager (no worries, that one comes with Node), like this:

<pre><code class="shell">$ npm -g install embark</code></pre>

If you want to have access to Embark 4 alpha, do this instead:

<pre><code class="shell">$ npm -g install embark@next</code></pre>

After that, `embark` should be available as a global command in your terminal of choice. Let's verify this by running the following command:

<pre><code class="shell">$ embark --version</code></pre>

At the time of writing this guide, the output looked like this:

<pre><code class="shell">3.2.1</code></pre>

Awesome! We're all set up. Let's build our first decentralized application!

