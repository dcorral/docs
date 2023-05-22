# Build DeFiChain Node In MacOS

### Get the source code

```bash
git clone -b feature/evm https://github.com/defich/ain
cd ain
```

### Compile the node
Install Xcode Command Line Tools:

```bash
xcode-select –install
```

Other dependencies for running `./make.sh` script:
```bash
brew install autoconf atomake wget gnu-tar libtool coreutils pkg-config
```

Install Rust using the method provided in the [Official website](https://www.rust-lang.org/tools/install) or run the following command:
```bash
./make.sh pkg_install_rust
```

Build the node:
```bash
./make.sh build
```

This command will compile the node dependencies and the node itself. Beware that this will take some time in the first run as it will download all the source code of the libraries needed.
