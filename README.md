# RPKI Testing Environment

```bash
% docker compose up -d
% docker compose exec gobgp1 bash
$ gobgp neighbor    # すべてのピアの情報を表示
$ gobgp neighbor 10.0.255.1    # 特定のピアの情報を詳細表示
```

```bash
% docker system prune -a    # コンテナ・イメージ・ボリューム・ネットワークを全削除
```
