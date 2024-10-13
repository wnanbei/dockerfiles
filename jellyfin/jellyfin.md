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
