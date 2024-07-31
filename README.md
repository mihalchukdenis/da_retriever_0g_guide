# da_retriever_0g_guide

![1_7gPDdUg77wgro3bYJwtNwQ](https://github.com/user-attachments/assets/f8394f2c-cacb-4da0-916e-cc06cd1a9c90)

## Hardware Requirement
```bash
- RAM: 8GB
- CPU: 2 cores
- NET: 100 MBPS
```

## Installation
### Install dependencies
```bash
sudo apt-get update
sudo apt-get install cmake build-essential protobuf-compiler
```

### Install Rust
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

### Download the source code
```bash
git clone https://github.com/0glabs/0g-da-retriever.git
```

## Configuration
|Field|Description|
|:----|:----------|
|log_level|Set log level|
|grpc_listen_address|Server listening address|
|eth_rpc_endpoint|JSON RPC node endpoint for the blockchain network|

## Run
```bash
cargo build --release
./target/release/retriever --config ./run/config.toml
```
