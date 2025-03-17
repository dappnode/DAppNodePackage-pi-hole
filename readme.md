# Pi-hole DAppNode Package

Pi-hole is a network-wide ad blocker that works at the DNS level. This package allows you to run Pi-hole directly on your DAppNode.

![Pi-hole Logo](https://pi-hole.net/wp-content/uploads/2016/12/Vortex-R.png)

## Description

Pi-hole acts as a DNS sinkhole that protects your devices from unwanted content, without installing any client-side software. It blocks ads and trackers at the network level, improving your internet browsing experience and potentially reducing bandwidth usage.

Key features:
- Network-wide ad blocking
- Web interface to view statistics and control filtering
- API for interaction with other systems
- Custom whitelist and blacklist management
- DHCP server capability (optional)

## Getting Started

### Prerequisites
- A running DAppNode installation

### Installation
1. Go to the DAppNode admin UI
2. Navigate to "Installer" or "Install" section
3. Search for "Pi-hole"
4. Click "Install"

### Configuration
During the installation process, you will be asked to set:
- Admin password
- (Optional) Upstream DNS providers

## Usage

Access the Pi-hole web interface by clicking on the link in your DAppNode dashboard or navigate to:
http://pihole.dappnode/admin

## Default Settings

- The default admin password is shown in the package info
- Default DNS settings use Cloudflare DNS (1.1.1.1)
- The package uses its own internal volume for data persistence

## Advanced Configuration

You can customize Pi-hole by modifying:
- Blocklists
- Whitelist domains
- Blacklist domains
- DNS settings

All changes made through the web interface are persisted across package restarts and updates.

## Support

If you have any issues or questions, please reach out to the DAppNode community:
- [DAppNode Discord](https://discord.gg/dappnode)
- [GitHub Issues](https://github.com/dappnode/DAppNodePackage-pi-hole/issues)

## License

This DAppNode package is licensed under the GNU General Public License v3.0.
Pi-hole is free software licensed under the EUPL v1.2.