# 能研智助 早期开发 Git 历史

本仓库提供项目早期 Git 历史包，包含 60 条原始提交。公开作品源码及后续提交位于 https://github.com/Viyao691/XJTU-energy-learning-platform 。

下载本仓库所有文件并解压后，在该目录执行以下命令，按顺序还原历史包：

```text
python -c "from pathlib import Path; p=Path('.'); (p/'early-history.bundle').write_bytes(b''.join(x.read_bytes() for x in sorted(p.glob('early-history.bundle.part*'))))"
git bundle verify early-history.bundle
git clone early-history.bundle early-history
git -C early-history log --oneline
```

还原后的 bundle SHA-256：`c8744abd5d864be86fd3914fac0c6116f550e8e1fa51628948d486a3fe21a031`。末次提交：`10e5f27c8d444d4b78580cd5e86f165e7470363d`。

本仓库为私有评审材料，账号授权由项目负责人管理。
