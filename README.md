# Roblox Telemetry Blocklist

A simple list of Roblox telemetry and analytics domains that can be blocked using your system's `hosts` file.

## How to use

### Windows

1. Copy the lines from the [`hosts`](./hosts) file.
2. Open **Notepad as Administrator**.
3. Open:
   `C:\Windows\System32\drivers\etc\hosts`
4. Paste the copied lines at the bottom of the file.
5. Save the file.

### macOS

1. Copy the lines from the [`hosts`](./hosts) file.
2. Open **Terminal**.
3. Run:

```bash
sudo nano /etc/hosts
```

4. Enter your macOS password when asked.
5. Paste the copied lines at the bottom of the file.
6. Press `Ctrl + O` and then `Enter` to save.
7. Press `Ctrl + X` to exit.

## What does this do?

The entries in this blocklist redirect selected Roblox domains to `127.0.0.1` instead of allowing your computer to connect to them normally.

This is intended to block selected telemetry and analytics endpoints.

## Disclaimer

This can break Roblox or some of its features.

The Roblox client may stop working correctly if it needs one of the blocked domains. Updates can also change which domains Roblox uses.

Use this at your own risk.

If Roblox stops working properly, remove the entries you added to your `hosts` file.

## Contributing

Found a domain that should be added or removed?

Feel free to open a **pull request** with your changes. Please include a short explanation of why the domain should be added or removed.
