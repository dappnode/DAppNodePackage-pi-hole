# Getting Started with Pi-hole on DAppNode

## Introduction
Pi-hole is a network-wide ad blocking solution that acts as a DNS sinkhole, protecting your devices from unwanted content without requiring any client-side software.
Pi-hole includes a web-based admin interface where you can view statistics, manage blocklists, and configure settings. When running on DAppNode, you can access this interface at:

[http://pi-hole.dappnode/admin](http://pi-hole.dappnode/admin)

The admin dashboard provides real-time insights into your network's DNS queries, blocked content, and allows you to customize your Pi-hole configuration.
## Using Pi-hole as Your DNS Server

There are three main ways to use Pi-hole as your DNS server:

### 1. Configure Your Router

The most effective approach is to set Pi-hole as the DNS server for your entire network:

1. Access your router's admin panel (typically at `192.168.1.1` or `192.168.0.1`)
2. Locate DNS settings (often under WAN, Internet, or Network settings)
3. Replace the existing DNS servers with your DAppNode's IP address
4. Save changes and restart your router if required

All devices on your network will now automatically use Pi-hole for DNS resolution.

### 2. Configure Individual Devices

If you can't modify router settings, configure DNS on each device:

- **Windows**: Network Properties > IPv4 Properties > Use the following DNS server
- **macOS**: System Preferences > Network > Advanced > DNS
- **iOS**: Settings > Wi-Fi > (your network) > Configure DNS
- **Android**: Settings > Network & Internet > WiFi > (your network) > Edit > Advanced options

### 3. Use Pi-hole's DHCP Server (advanced)

If your router doesn't allow DNS changes:

1. Disable DHCP on your router
2. In Pi-hole admin panel, go to Settings > DHCP
3. Enable DHCP server
4. Configure IP range and other settings
5. Save changes

New devices connecting to your network will automatically use Pi-hole for both DHCP and DNS.

## Support

For more information:
- Visit [Pi-hole documentation](https://docs.pi-hole.net/)
- Join the [DAppNode Discord](https://discord.gg/dappnode) for community support