# Jellyfin

## 基础配置

### 字体

```bash
apt install fonts-noto-cjk-extra
```

### Intel 核显

确认显卡直通：

```bash
ls /dev/dri
```

驱动安装：

```bash
apt install intel-media-va-driver
```

解码支持确认：

```bash
/usr/lib/jellyfin-ffmpeg/vainfo
```

## 刮削

可以使用 dnscheck 服务来查询正常解析的域名，然后修改 host。

[DnsChecker](https://dnschecker.org/)

需要检查以下域名：

- `api.themoviedb.org`
- `api.thetvdb.org`
- `image.tmdb.org`
