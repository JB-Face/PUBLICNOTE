<!--
 * @Descripttion: 
 * @version: 
 * @Author: JBFace
 * @Date: 2022-01-21 11:55:58
 * @LastEditors: JBFace
 * @LastEditTime: 2022-01-21 11:55:58
-->
# 自动注释

  

===

**VsCode 自动生成文件头部注释和函数注释**
==========================

[http://spidercode.cn/show-34.html](http://spidercode.cn/show-34.html)

### 1、安装插件KoroFileHeader

  

### 2、设置

  

在vscode左下角点击设置按钮，选择“设置”，然后输入“fileheader”,

  

*   文件头部注释：Fileheader:custom Made
*   函数注释：Fileheader:cursor Mode

随便点击哪个"在setting.json"中编辑，输入以下设置后保存，然后重启vscode更新设置：

  

```
    // 文件头部注释
    "fileheader.customMade": {
        "Descripttion":"",
        "version":"",
        "Author":"sueRimn",
        "Date":"Do not edit",
        "LastEditors":"sueRimn",
        "LastEditTime":"Do not Edit"
    },
    //函数注释
    "fileheader.cursorMode": {
        "name":"",
        "test":"test font",
        "msg":"",
        "param":"",
        "return":""
    }
```

### 3、使用

（1）文件头部注释

1.  快捷键：crtl+alt+i（window）,ctrl+cmd+t (mac)
2.  生成样式如下：

  

（2）函数注释

1.  快捷键：ctrl+alt+t (window), ctrl+alt+t(mac)
2.  函数注释不一定生成在头部，自己把控
3.  生成样式如下：

  

配置文件
====

```
     // 文件头部注释
     "fileheader.customMade": {
         
        "Descripttion":"",
        "version":"",
        "Author":"JBFace",
        "Date":"Do not edit",
        "LastEditors":"JBFace",
        "LastEditTime":"Do not Edit"
    },
    //函数注释
    "fileheader.cursorMode": {
        "msg":"",
        "param":"",
        "return":"",
        "LastEditTime":"Do not Edit",
        "LastEditors":"JBFace",
    }
```

# 代码片段存储研究

[https://juejin.cn/post/6933075278512160776](https://juejin.cn/post/6933075278512160776)

  

===
