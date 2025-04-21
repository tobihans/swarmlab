# Trying Docker Swarm mode

## Snippets

- Creating a VM

```sh
incus launch images:debian/13 debian-test-vm --vm
```

- Assign a set of environment to the VM

```sh
incus config set debian-test-vm limits.cpu=2
incus config set debian-test-vm limits.memory=1024MiB
```

- Setup docker for running OCI containers

```sh
incus remote add docker https://docker.io --protocol=oci
```

- 
