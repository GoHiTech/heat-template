# hot/README.md

```bash
openstack stack create \
-t "https://raw.githubusercontent.com/GoHiTech/heat-template/main/server.hot.yaml" \
-e tmp/server.env.yaml \
server001

openstack stack create -e tmp/hpc.env.yaml -t hpc.hot.yaml hpc001

openstack stack update -e tmp/hpc.env.yaml -t hpc.hot.yaml hpc001
```
