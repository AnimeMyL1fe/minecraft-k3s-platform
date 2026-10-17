netbird добавляет хосты в изолированную сеть, чтобы была связность между локальной сетью и entrypoint (vps)
 
в k3s rancher закинуть в конфиг /etc/rancher/k3s/config.yaml:
tls-san:
  - "100.81.233.21"
  - "k3s-controlplane"

и после просто рестартнуть k3s:
systemctl restart k3s