# Network Sniffer
Capture, store and filter network traffic.

## Dependencies
### Linux
```bash
apt install cargo protobuf-compiler libprotobuf-dev libssl-dev libpcap-dev
```

## Run
```bash
cargo build && \
    sudo setcap cap_net_raw,cap_net_admin=eip ./target/debug/sniffer && \
    ./target/debug/sniffer
```