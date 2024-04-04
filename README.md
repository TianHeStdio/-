# 天和文档

### English Vison

[README-en](README-en.md)

## 软件介绍

这个软件我们的界面思路仿照了Office，不过我们把字体文档等组件放在了最上面，把特殊组件放在了左边（可以自行调整），如果你懒得移动鼠标，还可以按下 / 按键，使用方向键来选择  

这个软件的所有快捷键放在了项目的 KEYWORDS.md 文件里，这款软件可以使用Office快捷键布局或天和文档快捷键布局，让每个不同习惯的人用上熟悉的按键布局  

我们这款软件可能比不上市面上的软件好，不过我们保证这款软件永久免费、开源，假如后来我们让某个功能收费了，你也可以修改源代码来让你白嫖


### 目前支持格式

#### 读取

.docx 
.doc 
.pdf 
.png 
.md 
.txt 

#### 写入

.docx 
.doc 
.md 
.txt 

## 介绍

这是一个文档类软件，虽然不如市场上其他软件，但我们保证它永远开源（目前免费）

## 为什么有它

这款软件我们对macOS和Windows版本使用了不同的开发框架，Windows使用QT编写，而macOS使用swiftUI编写
为什么这样，我是使用macOS的人，这里的生态很糟糕（在中国大陆），就算有macOS版软件的，也大部分是个凑数的，而我正是一个swiftUI的前端，所以机缘巧合下开启了这个项目  

你可能觉得这个项目是C语言做的，实际上它是C++实现的，从这段代码就能看出  

```
#include "mainwindow.h"

#include <QApplication>

int main(int argc, char *argv[])
{
    QApplication a(argc, argv);
    MainWindow window;
    window.show();
    return a.exec();
}
```

为什么是这样呢，因为CMake会生成一堆 .h 的文件，这能让人产生错觉

##### 2024/4/4
