# vpn-rules-dist

This public repository is generated automatically from the private `vpn-rules` source repository.

Do not edit files here manually. Manual changes will be overwritten by the publishing workflow.

GitHub stores only safe public routing rules here: domains and destination IP/CIDR ranges. It does not store full working VPN client configurations.

Real Hysteria2/VPS outbounds, server addresses, ports, passwords, UUIDs, private keys, access tokens, TLS/SNI values, and any other VPN secrets must live only in local private configuration on your devices.

Devices should download only remote rule sets from this repository and combine them with their own local private VPN outbounds.

A full working VPN configuration cannot be published safely in a public repository, because it must contain connection secrets.

Available artifacts:

- `rulesets/eu-only.json`
- `rulesets/tr-only.json`
- `rulesets/auto-vps.json`
- `txt/eu-only.txt`
- `txt/tr-only.txt`
- `txt/auto-vps.txt`
- `metadata/build-info.json`
- `metadata/domains-index.json`
- `examples/sing-box-remote-ruleset-snippet.json`

Use `examples/sing-box-remote-ruleset-snippet.json` as a safe fragment for the `route.rule_set` section of your private local sing-box configuration.
