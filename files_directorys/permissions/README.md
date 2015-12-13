# 文件与目录的权限

首先先看一下``ls``的长列表输出，以空格分割出了几个字段:

```
$ ls -l /bin/ls
-rwxr-xr-x 1 root root 110080 Jan 14  2015 /bin/ls
|    |     |  |    |     |          |          |
|    |     |  |    |     |          |          `- 文件名(/bin/ls)
|    |     |  |    |     |          `------------ 文件最后修改时间(2015年1月14日)
|    |     |  |    |     `----------------------- 文件大小(110080 B，-h参数将以易读形式显示)
|    |     |  |    `----------------------------- group name(root)
|    |     |  `---------------------------------- owner name(root)
|    |     `------------------------------------- 硬链接的次数(1)
|    `------------------------------------------- 权限(rwxr-xr-x)
`------------------------------------------------ 文件类型(-)
```