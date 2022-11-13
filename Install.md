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

### 手动部署

```python
# 服务器或本地电脑安装好python3.8或最新版的环境。
# 克隆源码到本地
git clone https://github.com/Baiyuetribe/kamiFaka.git
cd kamiFaka
# 安装项目依赖
pip install -r requirements.txt

# 初始化数据库
python db_init.py

# 启动程序
gunicorn -k gevent --bind 0.0.0.0:8000 --workers 8 app:app
```
