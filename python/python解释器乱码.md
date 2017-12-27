# macos python 解释器乱码

强制重启了下机器，结果导致 python3 解释器启动失败，之前环境是python2和python3共同存在的
尝试找到路径直接运行，也没解决

```shell
➜  ~ python3
python3: posix_spawn: /Library/Frameworks/Python.framework/Versions/3.6/bin/python3.62.7: No such file or directory
➜  ~
➜  ~
➜  ~
➜  ~ which -a python3

/Library/Frameworks/Python.framework/Versions/3.6/bin/python3
/usr/local/bin/python3
```

最后全部卸载重新安装了

```shell
➜  ~ sudo rm -rf /Library/Frameworks/Python.framework/Versions/3.6
➜  ~ sudo rm -rf "/Applications/Python\ 3.6/"
➜  ~ brew link python3
➜  ~ brew link python3
```

最后在重新安装下 jupter  ipython 之类的就好了



