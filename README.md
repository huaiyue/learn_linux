# learn_linux

ftp：put get bye  

cat -n 显示行号输出

cat a.txt b.txt > c.txt 将a b内容合并送到c，若c不存在，则创建

ls命令的PATH：bin
[jenkins@ft-api ~]$ echo $PATH
/usr/local/bin:/bin:/usr/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/home/jenkins/.nvm:/home/jenkins/bin
[root@ft-api jenkins]# echo $PATH
/root/.nvm/versions/node/v7.10.0/bin:/sbin:/bin:/usr/sbin:/usr/bin

alias p='pwd'  指令起别名
[jenkins@ft-api sbin]$ alias
alias c='clear'
alias l.='ls -d .* --color=auto'
alias ll='ls -l --color=auto'
alias ls='ls --color=auto'
alias lt='ls -lrht'
alias q='exit'

cat text.txt
tac text.txt 最后一行开始显示
nl text.txt 显示行号
more text.txt 一页一页地显示文件内容

less text.txt 同上，但是可往前翻页
  空格／pagedown：向下翻动一页
  pageup：向上翻动一页
  ／字符串：向下查询
  ？字符串：向上查询
  q：离开less这个程序
  
head text.txt 只看头几行
tail text.txt 只看尾几行（默认10行） 
tail -n 20 text.txt
tail -f text.txt 持续监测文件后面内容 等到ctrl+c才会离开tail这个程序
