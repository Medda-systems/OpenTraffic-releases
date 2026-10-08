# OpenTraffic

OpenTraffic is a macOS menu bar app for sharing the web servers you run while developing, through
Cloudflare Quick Tunnels or your own domain, Tailscale, ngrok, or OpenTunnel. Shares can turn on
live collaboration: everyone who opens the link sees each other's cursors and can pin comments to
the page, and coding agents can pick that feedback up over MCP.

This repository holds OpenTraffic's releases and its update feed.

## Install

```sh
brew install --cask medda-systems/tap/opentraffic
```

Or download the disk image from the [latest release](https://github.com/Medda-systems/OpenTraffic-releases/releases/latest),
open it, and drag OpenTraffic into Applications. Installed copies update themselves.

Releases aren't notarized yet, so macOS blocks the first launch. On macOS 15 or later, open
**System Settings → Privacy & Security** and click **Open Anyway**; on macOS 14, Control-click the app
and choose **Open**.

Requires macOS 14 or later (Apple silicon or Intel). Cloudflare shares need `cloudflared`
(`brew install cloudflared`); Tailscale, ngrok, and OpenTunnel are optional.

## Updates

Each release carries `appcast.xml`, the feed installed copies check once a day. The feed and every
disk image are signed with Medda Systems' update key and verified before anything is installed.

OpenTraffic is made by [Medda Systems](https://medda.se) and released under the MIT License.
