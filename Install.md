## 安装教程

### Docker部署
```bash
# 安装命令
docker run --name kmfaka -itd -p 8000:8000 baiyuetribe/kamifaka:latest
```
```bash
# 卸载命令
docker rm -f kmfaka && docker rmi -f baiyuetribe/kamifaka:latest
```

#### 支付宝对接教程
http://119.29.25.39:3200/byfaka/#%E6%94%AF%E4%BB%98%E5%AE%9D%E5%BD%93%E9%9D%A2%E4%BB%98%E5%AF%B9%E6%8E%A5%E6%95%99%E7%A8%8B