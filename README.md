# Awvs 2019_07 Docker
基于 https://github.com/Leezj9671/SecDevices_docker 项目修改

下载awvs保存到当前目录: https://pan.baidu.com/s/1P8KKBtXqi-_n2egxp9pLCQ 提取码: m9h3

refs: https://xs3c.co/archives/643

```
生成镜像
docker build -t awvs_2019_07 ./

启动docker
docker run -d -p 51443:13443 --name wvs07 awvs_2019_07

进入docker
docker exec -it -u root wvs07 /bin/bash

运行patch
./patch_awvs
```

登录awvs平台: http://vpsip:51443/

账号密码:
admin@test.com
Test123...

awvs api调用: awvs_api.py
