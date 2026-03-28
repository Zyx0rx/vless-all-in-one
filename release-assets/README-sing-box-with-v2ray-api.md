# Sing-box with_v2ray_api custom build

This release includes a custom **Sing-box** binary with `with_v2ray_api` enabled.

Current custom version string: **zyx0rx-with-v2ray-api1-a11cd1e**

It is required for **Sing-box user traffic statistics** in `vless-all-in-one` v3.5.3, including:

- Hysteria2 user traffic stats
- TUIC user traffic stats
- AnyTLS user traffic stats
- traffic sync to database
- quota / expiry workflows based on synced traffic

## When you need this

Use this custom binary if you want **Sing-box traffic statistics** in the script.

If you only use basic Sing-box protocols and do not care about per-user traffic sync, the upstream official binary may still work for normal proxy usage.

## Install

On the target server:

```bash
systemctl stop vless-singbox 2>/dev/null || true
cp -f sing-box-zyx0rx-with-v2ray-api-linux-amd64 /usr/local/bin/sing-box
chmod +x /usr/local/bin/sing-box
/usr/local/bin/sing-box version
systemctl restart vless-singbox
```

## Verify

You should see a custom version string and `with_v2ray_api` in version output:

```bash
/usr/local/bin/sing-box version
```

Then re-generate config in the script and verify traffic stats features.

## Notes

- This binary is a **custom build**, not the upstream official release artifact.
- It is intended for `vless-all-in-one` v3.5.3 traffic-stat workflows.
- If you replace it later with the official upstream binary, Sing-box traffic statistics may stop working.
