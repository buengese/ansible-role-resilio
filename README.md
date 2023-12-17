# Ansible Role: Resilio Sync

This Ansible role facilitates the deployment of the Home/Pro version of Resilio Sync, a powerful file synchronization and sharing tool.

## Role Variables

### Required Variables
While no variables are strictly required for this role, it is recommended to set the `webui_listen` variable to configure the address for the web UI.

- `webui_listen`: The IP address and port where the Resilio Sync web UI will listen. Default: `'127.0.0.1:8888'`.

### Optional Variables
Additional optional variables provide further customization and control over the Resilio Sync setup:

- `device_name`: The name to identify the device in Resilio Sync. Default: `'{{ inventory_hostname_short }}'`.
- `storage_path`: The path where Resilio Sync stores its data. Default: `'/var/lib/rslsync'`.
- `use_upnp`: Determines whether to use UPnP for port forwarding. Default: `false`.

For a comprehensive list of optional variables, see [defaults/main.yml](defaults/main.yml).

## Supported Operating Systems

This role is tested and supported on the following operating systems:

- Debian 10 (Buster), 11 (Bullseye), 12 (Bookworm)
- Ubuntu 20.04 (Focal Fossa), 22.04 (Jammy Jellyfish)
- Fedora 39
- ArchLinux
- Rocky Linux 9

## License

This Ansible role is distributed under the MIT license.