EMC Report Database V5.0 RC5 - iPhone PWA 使用版

本程序包已经增加：
- iPhone/iPad 主屏幕图标
- Web App Manifest
- Service Worker 离线缓存
- iOS独立全屏模式元数据
- iPhone安全区域适配
- 手机按钮和筛选框尺寸优化
- iOS“添加到主屏幕”操作提示

重要：PWA不能直接从ZIP或iPhone“文件”App安装。必须将本目录全部文件部署到HTTPS网站，并保持目录结构不变。

部署目录：
index.html
manifest.webmanifest
service-worker.js
offline.html
icons/

iPhone安装：
1. 用Safari打开部署后的HTTPS网址。
2. 点击Safari的“分享”按钮。
3. 选择“添加到主屏幕”。
4. 点击主屏幕上的“EMC DB”图标运行。

说明：
- 应用数据仍保存在当前iPhone的浏览器本地存储中。
- 清除Safari网站数据可能删除本地数据库，请定期导出Excel或JSON备份。
- Excel组件仍通过在线CDN加载，首次使用Excel导入/导出需要网络。
- Windows网络共享路径（UNC）不能由iPhone直接打开；可复制路径供Windows电脑使用。
