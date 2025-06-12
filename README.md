# My container definitions

## `cpython-fedora`

    podman build cpython-fedora -t cpython-fedora

    podman run -it --rm -v ~/dev/cpython:/workspace:O -w/workspace cpython-fedora

## `buildmaster-fedora`

    podman build buildmaster-fedora -t buildmaster-fedora

    podman run -it --rm -w/buildmaster-config -p 9011:9011 buildmaster-fedora
