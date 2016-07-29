MarkDown语法整理



# 目录


[TOC]



# 当前日期时间

July 29, 2016 11:21 AM

# 当前文件名

未命名.md

# 标题
## 标题2
### 标题3
#### 标题4
##### 标题5
###### 标题6

# 加粗

曾经，在各大缓存图片的框架没流行的时候。有一种很常用的内存缓存技术：SoftReference 和 **WeakReference**（软引用和弱引用）。但是走到了 Android 2.3（Level 9）时代，垃圾回收机制更倾向于回收 **SoftReference** 或 **WeakReference** 的对象。后来，又来到了 Android3.0，图片缓存在内容中，因为不知道要在是什么时候释放内存，没有策略，没用一种可以预见的场合去将其释放。这就造成了内存溢出。

# 强调

曾经，在各大*缓存图片的框架*没流行的时候。有一种很常用的内存缓存技术：SoftReference 和 WeakReference（软引用和弱引用）。但是走到了 Android 2.3（Level 9）时代，垃圾回收机制更倾向于回收 SoftReference 或 WeakReference 的对象。后来，又来到了 Android3.0，图片缓存在内容中，因为不知道要在是什么时候释放内存，没有策略，没用一种可以预见的场合去将其释放。这就造成了内存溢出。

# 行内代码

`setContentView(R.layout.activity_main);`

# 图片

![](https://raw.githubusercontent.com/android-cn/android-open-project-analysis/master/tool-lib/network/volley/image/volley.png)

# 超链接

[Github](http://www.github.com)

# 引用

> 曾经，在各大*缓存图片的框架*没流行的时候。有一种很常用的内存缓存技术：SoftReference 和 WeakReference（软引用和弱引用）。但是走到了 Android 2.3（Level 9）时代，垃圾回收机制更倾向于回收 SoftReference 或 WeakReference 的对象。后来，又来到了 Android3.0，图片缓存在内容中，因为不知道要在是什么时候释放内存，没有策略，没用一种可以预见的场合去将其释放。这就造成了内存溢出。

# 有序列表

1. First
2. Second
3. Thrid

# 无需列表

- First
- Second
- Thrid

# 分页符


* * *

# 分节符


- - -


# 分段符


_ _ _


# 代码块

```
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
}
```

# X语言代码块

```java
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
}
```

# 删除线

~~即可收到回复给你们农民负担呢~~

# TaskList

- [ ] A
- [ ] B
- [ ] C

# 下划线

++上的复活节啊，方便您科技示范点++

# 脚注

上的黄金股份，[^海口翻江倒海空间]

# 脚注引用

手机电话费各方都好看

[^]: http://www.github.com

# 表格

| 项目 | 类别 |
|--------|--------|
|    Java    |   C++     |

# 高亮

==圣诞节==狂欢官方回复都会感慨聚精会神的房间哭就哭了


# 嵌入对象

@[](Github)

# 数学代码（行间）

$$

$$

# 数学代码（行内）

$$$y=x+8$$$

# 注释

```java
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        <!--setContentView(R.layout.activity_main);-->
    }
}
```