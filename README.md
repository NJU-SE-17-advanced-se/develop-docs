# develop-docs

用于存放项目**开发**文档。

因为视频文件可能会占用较大的空间，所以使用 git lfs 进行管理。新版本的 git 应该自带 git lfs，如果没有请安装一个。

以下命令仅供参考：

clone本仓库：

```shell
git lfs clone <URL>
```

clone本仓库而不想下载lfs文件：

```shell
git lfs clone <URL> -X "*.*"
```

