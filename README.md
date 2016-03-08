# svn-note
svn-note

## SVN 官网

http://subversion.apache.org/source-code.html#source-release

hust镜像 

http://mirrors.hust.edu.cn/apache/subversion/

以上方法需要编译，需要apache port runtime

## ubuntu直接采用 apt-get install

```
sudo apt-get install subversion
```
## 检查是否安装好
svn help
```
用法: svn <subcommand> [options] [args]
Subversion 命令行客户端，版本 1.8.8。
使用“svn help <subcommand>” 显示子命令的帮助信息。
使用“svn --version”查看程序的版本号和版本库访问模块，或者
使用“svn --version --quiet”只查看程序的版本号。

大多数的子命令可接受文件或目录参数，对目录进行递归处理。
如果没有指定参数，默认对当前目录(包含当前目录)递归处理。

可用的子命令:
   add
   blame (praise, annotate, ann)
   cat
   changelist (cl)
   checkout (co)
   cleanup
   commit (ci)
   copy (cp)
   delete (del, remove, rm)
   diff (di)
   export
   help (?, h)
   import
   info
   list (ls)
   lock
   log
   merge
   mergeinfo
   mkdir
   move (mv, rename, ren)
   patch
   propdel (pdel, pd)
   propedit (pedit, pe)
   propget (pget, pg)
   proplist (plist, pl)
   propset (pset, ps)
   relocate
   resolve
   resolved
   revert
   status (stat, st)
   switch (sw)
   unlock
   update (up)
   upgrade

Subversion 是版本控制工具。
欲取得详细资料，请参阅 http://subversion.apache.org/

```
## Probloms;

   1.svn: E200009: Could not add all targets because some targets are already versioned
   
   2.解决命令：
   
或者

terminal，cd到你要提交的目录，输入命令：
```
find ./ -name .svn        (显示该目录下所有的.svn)文件
find ./ -name .svn | xargs rm -rf       (删除该目录下所有的.svn)文件
```
