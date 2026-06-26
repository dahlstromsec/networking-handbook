# Network Troubleshooting

## What You'll Learn
- Basic troubleshooting workflow
- Common networking tools

## Useful Commands

```bash
ip a
ip r
ping 8.8.8.8
ping example.com
traceroute example.com
ss -tulpn
netstat -tulpn
nslookup example.com
dig example.com
```

## Suggested Workflow

1. Verify interface configuration.
2. Check IP address.
3. Verify default gateway.
4. Test connectivity with `ping`.
5. Test DNS resolution.
6. Inspect open ports and listening services.

## Cybersecurity Context

Systematic troubleshooting helps identify misconfigurations, outages, and suspicious network behavior.

## Summary

Following a structured troubleshooting process reduces time spent diagnosing network issues.
