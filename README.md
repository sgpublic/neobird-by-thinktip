# luci-theme-neobird

原 repo：[thinktip/luci-theme-neobird: 一个专门针对移动端优化的OpenWRT主题，基于luci-theme-material，全新的登录界面，沉浸式Webapp体验。 (github.com)](https://github.com/thinktip/luci-theme-neobird)

## 使用 （云编译）

1. 在 `diy-part1.sh` 中添加：

   ```
   echo 'src-git neobird https://github.com/SGPublic/neobird-by-thinktip' >>feeds.conf.default
   ```

2. 在 `diy-part1.sh` 中设置默认主题修改：

   ```
   sed -i ' s/luci-theme-bootstrap/luci-theme-neobird/g ' feeds/luci/collections/luci/Makefile
   ```

3. 在你的 `.config` 文件中添加：

   ```
   CONFIG_PACKAGE_luci-theme-neobird=y
   ```

   
