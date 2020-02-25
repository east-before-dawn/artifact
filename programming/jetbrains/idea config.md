# idea config

## 目录

[TOC]

## 参考

- [Changing IDE default directories used for config, plugins, and caches storage](https://intellij-support.jetbrains.com/hc/en-us/articles/207240985-Changing-IDE-default-directories-used-for-config-plugins-and-caches-storage)

# 默认插件安装目录

```
C:\Users\Administrator\.IntelliJIdea2019.2\config\plugins
```

# idea.properties 核心配置文件

IDEA_HOME\bin\idea.properties

## 配置路径

- **idea.config.path**

  这个目录是`File\settings`标签下做的一些配置，例如CodeStyle、KeyMaps等

- **idea.system.path**

  这个目录下的配置很关键，编译工具、本地历史、工作空间配置等都在这里

- **idea.plugins.path**

  自定义插件安装目录。除了在IDEA的操作界面添加，把插件移动到这个目录然后重启也可以安装成功，这就是离线安装。

- idea.log.path

  IDEA产生的log

## 自定义修改配置

```
idea.config.path=Z:/Data/JetBrains/.PyCharm/config
idea.system.path=Z:/Data/JetBrains/.PyCharm/system
idea.plugins.path=${idea.config.path}/plugins
idea.log.path=${idea.system.path}/log
```





