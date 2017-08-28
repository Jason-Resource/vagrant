# 编辑配置文件
先禁用默认的ssh转发，再添加自定义转发：

```
     config.vm.network "forwarded_port", guest: 22, host: 2222, id: "ssh", disabled: "true"
     config.vm.network "forwarded_port", guest: 22, host: 3333
```
