# mydog
监控文件改动，随时自动备份，彻底防止误删

效果：指定目录下的指定文件类型一旦发生改动（创建、改动、删除），立刻备份到指定路径。可以指定备份周期，在备份周期内的改动将汇总到同一个目录，不同备份周期则备份到不同目录，保存备份的目录结构跟原目录结构一致。

## 使用
`python mydog.py /home/you/you`即可，`/home/you/you`是被监控的目录。

如果出现`too many open files`错误，可以尝试执行
```
sudo sysctl -w fs.inotify.max_user_watches="99999999"
```
再运行脚本。

## 链接
https://kexue.fm/

## 交流
QQ交流群：67729435，微信群请加机器人微信号spaces_ac_cn
