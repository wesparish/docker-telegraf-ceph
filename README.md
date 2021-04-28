# docker-telegraf-ceph

Adds a ceph install to the upstream telegraf image

Example:
```
docker run --rm -ti --entrypoint telegraf \
  -v /etc/ceph/:/etc/ceph:ro \
  -v $PWD/telegraf-ceph.config:/telegraf-ceph.config \
  -v /var/run/ceph:/var/run/ceph:ro \
  wesparish/docker-telegraf-ceph:ubuntu-18.04 \
  --config /telegraf-ceph.config --debug
```
