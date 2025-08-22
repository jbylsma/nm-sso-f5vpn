# NetworkManager F5 VPN with SSO
Invokes a pre-configured NetworkManager connection for a F5 VPN from a `f5-vpn://`
link. Currently limited to a single NetworkManager F5 VPN connection, which must
be set in `${HOME}/.config/nm-f5vpn-sso.conf`.

The provided desktop entry must be installed to register `f5-vpn://` schemes.
Use the following to install the entry locally.
```sh
desktop-file-install \
  --dir="${HOME}/.local/share/applications" \
  ./nm-f5vpn-sso.desktop
update-desktop-database "${HOME}/.local/share/applications"
```

Adjust the executable path as needed.
