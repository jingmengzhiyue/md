
# Linux常用操作

> Written with [StackEdit](https://stackedit.io/).

git 远端强制覆盖本地
```git
git fetch --all
git reset --hard origin/master
git pull
```
linux 复制文件夹下所有文件到另一个文件夹 
```shell
cp -r /home/packageA/* /home/cp/packageB/
cp -r /home/packageA/. /home/cp/packageB/
```

当使用tar解压缩时，默认将文件解压缩到当前目录中。可以通过“-C”选项来指定解压缩的目录。例如，将文件解压缩到“/home/user/”目录中，可以使用以下命令：

```shell
tar -zxvf example.tar.gz -C /home/user/
```
在训练深度神经网络中通常需要实时查看显卡的占用，这时可以使用以下命令来查看
```shell
whatch -n 1 nvidia-smi
```
命令中`-n`后面的参数表示每隔多少秒刷新一次。

通过进程的pid 查找占用的用户名：
```shell
lsop -p 进程的pid号
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExMDYzMDE0MTVdfQ==
-->