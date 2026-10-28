# sing-box-rules

sing-box 远程自定义直连规则集（JSON 源码格式，免编译在线维护）。

## 规则链接

* **GitHub Raw（首选，配置通过 Reality 代理下载）**：
  `https://raw.githubusercontent.com/Crucialmer/sing-box-rules/main/custom-direct.json`
* **jsDelivr CDN（国内加速备用）**：
  `https://cdn.jsdelivr.net/gh/Crucialmer/sing-box-rules@main/custom-direct.json`

## 文件说明

* `custom-direct.json`：国内小众/补漏网站直连规则集，基于 sing-box Headless Rule 标准规范编写。已预收录国检集团、CBMA 建材数据库、快看漫画、韵达、小米 IoT 等不在 geosite-cn 官方规则中的国内常用服务。

## 维护指南

遇到国内因未收录在 geosite-cn 而误走代理的小众网站时：
1. 访问 [custom-direct.json](https://github.com/Crucialmer/sing-box-rules/blob/main/custom-direct.json)；
2. 点击右上角的铅笔图标编辑；
3. 在 `domain_suffix` 列表中追加你要直连的域名（如 `"example.com"`）；
4. 点击 **Commit changes** 提交；
5. sing-box 客户端会在达到设定周期（12小时）后自动拉取，或手动在客户端点击「更新规则集」立即生效。
