# Value: Firewall, proxy and DNS integration

While security vendors often include their own threat feeds within their protection products, having an additional, complementary source of CTI under **your control** is highly valuable. This empowers you to focus on intelligence specific to your organisation's areas or sectors and helps overcome data collection blind spots that vendors might have due to geographical, linguistic, cultural, or other limitations

Integrate with firewalls. Provide updates to firewall/block rules
Integrate with proxies. Provide updates to URL block lists
Integrate with DNS. RPZ zones

# Examples

- Firewalls: Integrating CTI feeds with your firewalls. Update block rules.
  - CSV export of threat events and set them up as your "local" threat feed to your firewall. 
    - [Fortinet](https://docs.fortinet.com/document/fortigate/6.4.9/administration-guide/9463/threat-feeds)
    - [Palo Alto External Dynamic List](https://docs.paloaltonetworks.com/pan-os/10-2/pan-os-admin/policy/use-an-external-dynamic-list-in-policy/configure-the-firewall-to-access-an-external-dynamic-list)
- Proxies: This prevents users from accessing newly identified malicious or phishing websites, reducing the risk of malware infections and credential theft.
  - URL block list PaloAlto
- DNS
  - Response Policy Zones. Sinkhole (redirect) potentially malicious URLs to a warning site, providing awareness / info to your users. [DNS firewalling](https://isc.sans.edu/diary/24556) with MISP.
  - Exports to [Infoblox Custom Named List](https://csp.infoblox.com/apidoc/?url=https%3A%2F%2Fcsp.infoblox.com%2Fapidoc%2Fdocs%2FAtcfw)

# References
