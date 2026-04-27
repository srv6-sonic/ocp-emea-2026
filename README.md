# SONiC Labs

## Supported Use Cases

- SRv6 AI Backend
- SRv6 L3VPN
- SRv6 GRT

Each use case contains its own configuration files and deploy script.

## Common Workflow

All use-case scripts support the same actions:

- deploy
- destroy
- shell <node_name>

Run from the repository root.

### SRv6 AI Backend

```sh
cd use-cases/SRv6-AI-Backend
sudo ./srv6_ai_backend.sh deploy
sudo ./srv6_ai_backend.sh shell <node_name>
sudo ./srv6_ai_backend.sh destroy
```

### SRv6 L3VPN

```sh
cd use-cases/SRv6-L3VPN
sudo ./srv6_l3vpn.sh deploy
sudo ./srv6_l3vpn.sh shell <node_name>
sudo ./srv6_l3vpn.sh destroy
```

### SRv6 GRT

```sh
cd use-cases/SRv6-GRT
sudo ./srv6_grt.sh deploy
sudo ./srv6_grt.sh shell 01T0
sudo ./srv6_grt.sh shell 01T1
sudo ./srv6_grt.sh shell NIC-A
sudo ./srv6_grt.sh destroy
```

Valid SRv6 GRT node names:

- Spines: 01T1, 02T1
- Leafs: 01T0, 02T0
- Hosts: NIC-A, NIC-B
