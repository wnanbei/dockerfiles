# PostgreSQL

## 安装向量插件

Postgres 需要安装 `pgvector` 插件以支持向量的存储和检索。

安装向量插件：

```bash
docker exec -it postgres /bin/bash
apt update
apt install -y postgresql-server-dev-all make gcc
git clone https://github.com/pgvector/pgvector.git
cd pgvector
make
make install
```

安装完成后，进入 PostgreSQL 数据库终端：

```bash
psql -U postgres -d mtphotos
```

进入需要启用向量额数据库后，启用向量：

```sql
use mtphotos;
CREATE EXTENSION vector;
```