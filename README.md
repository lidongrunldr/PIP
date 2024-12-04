# :racehorse: PIP :racehorse:
常用的pip操作
## :book: 常用的下载源
https://pypi.tuna.tsinghua.edu.cn/simple

http://mirrors.aliyun.com/pypi/simple/

https://pypi.mirrors.ustc.edu.cn/simple/

http://pypi.hustunique.com/simple/

https://mirror.sjtu.edu.cn/pypi/web/simple/
## :construction_worker: 使用
* 下载库
  ```
  pip install <库名> -i https://pypi.tuna.tsinghua.edu.cn/simple
  ```
* 查看当前环境中的所有库
  ```
  pip list
  ```
* 经常会遇到一种情况，已经用`pip install`下载了相关库且下载成功，但是仍然报错，那么就有两种办法：<br>
  1.没有安装指定版本
  ```
  pip install <库名>=版本号 -i https://pypi.tuna.tsinghua.edu.cn/simple
  ```
  2.若没有指定版本，
  ```
  pip install -U <库名>  
  ```
  若只需要下载某一个库中的某一个模块及其依赖项
  ```
  pip install -U <库名>[模块名]
  ```
