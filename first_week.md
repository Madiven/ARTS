# Algorithm

[3. Longest Substring Without Repeating Characters](https://www.jianshu.com/p/bf1ecee43a94)

[5. Longest Palindromic Substring](https://www.jianshu.com/p/2fd36b813198)

# Review

[每个程序员都应该了解的内存知识，Part 1 - 简介](https://www.jianshu.com/p/a5719a4cee68)

该文章适合有点硬件基础的读者阅读，作者试图阐明编程时硬件对软件性能的影响。

# Tip

linux上看日志的方法：

## tail命令

tail 命令可用于查看文件的内容，有一个常用的参数 -f 常用于查阅正在改变的日志文件。
tail -200f filename 会把 filename 文件里的最尾部的200行内容显示在屏幕上，并且不断刷新，只要 filename 更新就可以看到最新的文件内容。
其他参数：

- -q 不显示处理信息
- -v 显示详细的处理信息
- -c<数目> 显示的字节数
- -n<行数> 显示文件的尾部 n 行内容
- --pid=PID 与-f合用,表示在进程ID,PID死掉之后结束
- -q, --quiet, --silent 从不输出给出文件名的首部
- -s, --sleep-interval=S 与-f合用,表示在每次反复的间隔休眠S秒

日志实时监控：tail -200f filename

查询最后200行并且匹配关键字，且关键字标红：tail -n 200 name.log | grep '结果' --color

## less命令

less命令是对文件或其它输出进行分页显示的工具。
less filename

常用：
ctrl + F - 向前移动一屏

ctrl + B - 向后移动一屏

ctrl + D - 向前移动半屏

ctrl + U - 向后移动半屏

j - 向前移动一行

k - 向后移动一行

G - 移动到最后一行

g - 移动到第一行

q / ZZ - 退出 less 命令

v - 使用配置的编辑器编辑当前文件

h - 显示 less 的帮助文档

&pattern - 仅显示匹配模式的行，而不是整个文件

当使用 less 查看大文件时，可以在任何一个位置作标记，可以通过命令导航到标有特定标记的文本位置：

ma - 使用 a 标记文本的当前位置

'a - 导航到标记 a 处

# Share

[JDK1.8 ArrayDeque源码阅读](https://blog.csdn.net/maijia0754/article/details/86583183)
