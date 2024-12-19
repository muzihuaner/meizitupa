## 项目介绍
node脚本爬虫，爬取[美之图](https://kkmzt.com/)网站的所有图片
node版本: 大于16版本
修复图片不能下载的BUG
本项目仅供技术学习

## 项目启动

### 一、启动代理池
因该网站有反爬虫手段，同一IP频繁访问会导致IP被封，故采用了[ProxyPool]推荐Docker部署(https://github.com/jhao104/proxy_pool/tree/master)作为IP池，该池子抓去的IP部分质量还挺好的，做好异常判断就能用，打开[ProxyPool](https://github.com/jhao104/proxy_pool/tree/master)按照流程部署好服务。


### 二、启动本脚本
1. git clone
```bash
git clone https://github.com/huangyizhou0710/meizhitu.git
```

2. 安装依赖（若安装报错，请使用node v16）
```bash
npm install
```

3. 启动
```bash
node index.js
```