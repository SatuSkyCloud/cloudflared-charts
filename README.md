# Cloudflare Helm Charts

### About
A convenient location to publish Cloudflare helm charts

### Setup
```bash
helm repo add cloudflare https://cloudflare.github.io/helm-charts
helm repo update
```

### Discovery
```bash
helm search repo cloudflare
```

### Installation

Make sure `cloudflare` namespace and its labels (privileged security) are created and initialized beforehand.

```bash
cd charts/cloudflare-tunnel
helm upgrade --install cloudflare . --namespace cloudflare
```

### Uninstall

```bash
cd charts/cloudflare-tunnel
helm uninstall cloudflare --namespace cloudflare
```

### Contents

- `charts/cloudflare-tunnel`: Helm 3 chart using cloudflared best practices
