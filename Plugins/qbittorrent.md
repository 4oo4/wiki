# qBittorrent
Downloads content from entry URL and loads it into the ​qBittorrent bittorrent client.

Requirements: Supports qBittorrent 3.1.3 and above. qBittorrent WebUI must be enabled in the options menu.

**Example:**

```
qbittorrent:
  path: /media/disk/downloads/
  label: tv
  host: localhost
  port: 8080
```

## Options
All options are optional and will default to whatever you have set in qBittorrent. If you wish not to set any of the parameters the format is:
```
qbittorrent: yes
```

**Options**

|  Name  |  Description  |
| --- | --- |
|  host  |  qBittorrent host (default *localhost*)  |
|  port  |  qBittorrent port (default *8080*)  |
|  username  |  qBittorrent username that was set in the WebUI options. Can be omitted if *Bypass authentication for localhost* is checked  |
|  password  |  qBittorrent password that was set in the WebUI options. Can be omitted if *Bypass authentication for localhost* is checked  |
|  path  |  The download location  |
|| label || qBittorrent label ||