# Troubleshooting

## Proxmox connection
- Confirm the Proxmox host is reachable from the Android device.
- Verify hostname, port, TLS configuration, and network route.
- Check API token or account permissions in Proxmox.
- Never paste credentials, API tokens, cookies, or private keys into an Issue.

## VM or LXC information does not load
- Refresh the relevant screen.
- Check that the Proxmox account can view the resource.
- Check whether Proxmox itself reports an error.
- Record the DeepMox version and non-sensitive error text.

## Terminal or console problems
- Confirm the VM/container is accessible through the Proxmox web interface.
- Record exact reproduction steps, device model, Android version, and DeepMox version.
- Do not publish terminal output containing credentials or private infrastructure data.

## Backup and restore
- Confirm the selected storage has sufficient free space.
- Verify target storage and backup configuration in Proxmox.
- Do not upload backup archives or configuration exports to a public Issue.

If the problem persists, open a Bug Report.
