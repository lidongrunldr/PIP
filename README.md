# :racehorse: PIP :racehorse:
常用的pip操作
## :book: 常用的下载源
https://pypi.tuna.tsinghua.edu.cn/simple

http://mirrors.aliyun.com/pypi/simple/

https://pypi.mirrors.ustc.edu.cn/simple/

http://pypi.hustunique.com/simple/

https://mirror.sjtu.edu.cn/pypi/web/simple/
## :construction_worker: 使用
* 下载库<br>
  1.直接下载
  ```
  pip install <库名> -i https://pypi.tuna.tsinghua.edu.cn/simple
  ```
  2.依据指定文件下载
  ```
  pip install -r requirements.txt
  ```
  3.从GitHub仓库安装包
  ```
  pip install git+https://github.com/numpy/numpy.git
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
* 查看当前环境中的所有库
  ```
  pip list
  ```
* 查看某个已安装库的依赖包信息
  ```
  pip show -f <库名>
  ```
* pip导出python依赖包<br>
  1.导出所有已安装的依赖至文件requirements.txt中
  ```
  pip freeze > requirements.txt
  ```
  2.以pip list查询出来的形式输出到文件requirements.txt中
  ```
  pip list --format=freeze > requirements.txt
  ```
