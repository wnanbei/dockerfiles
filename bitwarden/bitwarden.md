# Bitwarden

## 生成 Admin Token

创建一个临时容器，使用容器中自带的工具生成 Admin Token：

```bash
docker run --rm -it vaultwarden/server /vaultwarden hash
```