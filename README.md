# nginx

## nginx剧本使用说明

    这个剧本用来以源码方式 安装nginx:1.22.1。安装方式为很直白，请在安装前保持目标系统干净，剧本
    有二处需要配置，在剧本中都有说明 ，请在运行前编辑。另 关于nginx的ssl配置，需要把nginx使用的
    证书放到files文件夹，取名为web.pem 和web.key，并配置hosts文件，改示例为你的域名
    然后运行如下：


    `
        ansible-playbook nginx.yaml
    `

### 再说点废话，如果主机是在云上，请配置安全组，本地主机请先配置防火墙和selinux