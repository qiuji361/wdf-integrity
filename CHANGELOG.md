# 更新日志

## 7.1

- 清理 `wdf_mark`、`wdf_spoof`、`wdf_susfs` 源码中的大段解释性注释。
- 重建受保护二进制、远程 hashes 和待压缩发布目录。

## 7.0

- 增加 `wdf_mark` 守护进程启动即检和每 300 秒完整性复查。
- WebUI 执行前增加 `module.prop` 作者字段复核，拦截改名二改。
- 真机完成 `wdf_loader`、`wdf_verify`、`wdf_mark` 和 WebUI 发布包联调验证。
