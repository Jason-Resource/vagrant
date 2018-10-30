- **[网络设置](https://pan.baidu.com/s/1uJj8j6SGBq0B5iM094TJow)**

```
// 新建一个文件夹
mkdir test

cd test/

// 加载box
vagrant.exe box add test E:/360极速浏览器下载/centos-7-clean.box

// 初始化
vagrant.exe init
vagrant.exe init test   // 指定box, test是已经加载的box, 可以使用vagrant.exe box list  查看
 
// 启动
vagrant.exe up

// 查看状态
vagrant.exe status

// 查看所有box
vagrant.exe box list

// 移除box
vagrant.exe box remove test

// 导出box
vagrant package
```
