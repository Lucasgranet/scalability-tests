# Scalability tests

This repo collects code, instructions and results for scalability tests on the Rancher product family.

## Troubleshooting

### Kubernetes cluster unreachable

If you get this error:
```
│ Error: Kubernetes cluster unreachable: Get "https://upstream.local.gd:6443/version": dial tcp 127.0.0.1:6443: connect: connection refused
```

SSH tunnels might be broken. Reopen them via:
```shell
./config/open-tunnels-to-upstream-*.sh
```
