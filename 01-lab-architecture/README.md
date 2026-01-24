# Lab Architecture

## Environment Overview

| Machine | OS | Role |
|---------|----|-----|
| Warden  | Ubuntu Server | Splunk Enterprise (Indexer & Search Head) |
| Victor  | Ubuntu VM | Linux endpoint (Splunk Universal Forwarder) |

## Data Sources

- System logs (`/var/log`)
- Custom application logs (Minecraft server)

Logs from Victor are forwarded to Warden for indexing, dashboards, and analysis.
