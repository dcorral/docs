# Build DeFiChain Node In MacOS

### 1. Install Xcode Command Line Tools:

```bash
xcode-select –install
```
### 2. Get the source code

```bash
git clone -b feature/evm https://github.com/defich/ain
cd ain
```

### 3. Install build dependencies

Other dependencies for running `./make.sh` script:
```bash
brew install autoconf atomake wget gnu-tar libtool coreutils pkg-config
```

### 4. Install Rust

Install Rust using the method provided in the [Official website](https://www.rust-lang.org/tools/install) or run the following command:
```bash
./make.sh pkg_install_rust
```

### 5. Build

Build the node:
```bash
./make.sh build
```

