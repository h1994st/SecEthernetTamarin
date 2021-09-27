# Secure Ethernet Tamarin

A formal model of a broadcast protection approach in Tamarin for automated security analysis

## Install Tamarin

### macOS

```bash
brew install tamarin-prover/tap/tamarin-prover
```

### Linux

To avoid using Homebrew on Linux, please follow the instructions below:

```bash
# get the source codes of Tamarin 1.6.1
git clone https://github.com/tamarin-prover/tamarin-prover.git
cd tamarin-prover
git checkout 1.6.1

# install dependencies
# - Haskell Stack
# https://github.com/commercialhaskell/stack/blob/master/doc/install_and_upgrade.md
curl -sSL https://get.haskellstack.org/ | sh

# - Graphviz
sudo apt install graphviz

# - Maude 2.7.1
# NOTE: please double check the version, but it seems 2.7.2 can work well
sudo apt install maude

# compile
make default
```

## Get Started

```bash
tamarin-prover --prove broadcast_protection.spthy
```
