# Resolvable - Systemd integration

Integrates [Resolvable](https://github.com/mgood/resolvable) with Systemd DNS
configuration.

    docker run -d \
        --hostname resolvable \
        -v /var/run/docker.sock:/tmp/docker.sock \
        -v /var/run/dbus/system_bus_socket:/var/run/dbus/system_bus_socket \
        -v /run/systemd:/tmp/systemd \
        mgood/resolvable-systemd
