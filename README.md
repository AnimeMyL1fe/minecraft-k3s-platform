# minecraft-k3s-platform

Helm-чарт и платформа для запуска серверов Minecraft в Kubernetes.

## Ручная сборка и пуш чарта в Harbor (OCI)

```bash
helm lint charts/minecraft
helm package charts/minecraft
helm push minecraft-0.1.0.tgz oci://192.168.0.211/helm-homelab
