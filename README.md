Docker services collection
===

Taskd
---

**Containers**:
 - [ogarcia/taskd](https://github.com/ogarcia/docker-taskd)

**Volumes**:
 - `/var/taskd`

**Ports**:
 - 53589

**Run**: `docker stack deploy -c taskd.yml taskd`

Syncthing
---

**Containers**:
 - [zebradil/syncthing](https://github.com/zebradil/syncthing)

**Volumes**:
 - `data` (may change through `SYNCTHING_DATA_DIR`)
 - `config` (may change through `SYNCTHING_CONFIG_DIR`)

**Ports**:
 - 8384
 - 22000
 - 21027/udp

**Run**: `SYNCTHING_DATA_DIR=/var/sync docker stack deploy -c syncthing.yml syncthing`
