Simple playbooks with roles for setup NFS exports and mounts.

Provided inventory contains example definitions of host groups and NFS exports/mounts per host.
It is expected that target OS is Ubuntu and user has configured ssh access to hosts (localhost in provided inventory) with paswordless sudo.

Apply on server:
- ansible-playbook -i inventory/nfs_servers.yml nfs_server.yml

Apply on client:
- ansible-playbook -i inventory/nfs_clients.yml nfs_client.yml
