# homelab
Production-quality personal homelab powered by k3s with ZFS storage. Self-hosted services including n8n, Vaultwarden, Joplin and game servers among others.

## Repository layout

```
clusters/homelab/   # GitOps entry point for the cluster
infrastructure/     # cluster-wide components applied before apps
  storage/          # OpenEBS ZFS LocalPV and StorageClasses
  ingress/          # Traefik config and certificates
apps/               # self-hosted services, grouped by area
  automation/       # n8n and other workflow tools
  bd/               # databases
  media/            # media services
  monitoring/       # metrics, logs and alerting
charts/             # Helm charts maintained in this repo
```
