# Nginx 配置
一些Nignx配置集合
## 安装
推荐使用Nginx官方提供的[Pre-Built Packages for Stable version](https://nginx.org/en/linux_packages.html#stable)

如访问性能不良可以使用[apt-mirror](https://apt-mirror.github.io/)。
## 配置
通过certbot获取Let’s Encrypt证书，需要另外配置
- `nginx.conf` Nginx主配置文件
- `base.conf` http下面的安全&性能优化
- `server_example.conf` server配置示例
- `www.conf` 在server中引用发关于日最、错误页、expires的配置
- `h2.conf` HTTP2(HTTPS) Server需要引用相关配置
- `proxy.conf` 反代需要引用的配置
- `hsts.conf` !!三思!!启用HSTS
- `to_h2.conf` 对支持的浏览器跳转HTTPS,用于port 80