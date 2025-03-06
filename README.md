用于嵌入试应用和开发的信息发布
Fix typo test
\n这是对 README.md 文件的一个改进。
\n这是对 README.md 文件的一个改进。
\n这是对 README.md 文件的一个改进。
\n这是对 README.md 文件的一个改进。

## Git 别名配置

为了方便查看提交历史，可以添加以下 Git 别名到 `~/.gitconfig` 文件：

```ini
[alias]
    graph = log --all --graph --decorate --oneline
```

运行 `git graph` 即可查看图形化提交历史。

## 全局 Git 忽略文件配置

为了避免将操作系统或编辑器生成的临时文件提交到仓库，可以设置全局 Git 忽略文件：

1. 运行以下命令设置全局忽略文件路径：

   ```bash
   git config --global core.excludesfile ~/.gitignore_global
   ```

2. 创建 `~/.gitignore_global` 文件并添加以下内容：

   ```gitignore
   # 忽略 macOS 的 .DS_Store 文件
   .DS_Store
   *.swp
   *.swo
   *.swn
   *.bak
   *.tmp
   *.log
   *.cache
   .idea/
   .vscode/
   ```
