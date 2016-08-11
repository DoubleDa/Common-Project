Android学习笔记


## Android优化

### Android写出高效清晰Layout布局文件的一些技巧

> 使用测试工具：
> [原文来自](http://www.open-open.com/lib/view/open1470474317994.html)

- 用TextView本身的属性同时显示图片和文字

```java
drawableLeft- 指定drawable放在文本的左边
drawableStart- 作用和drawableLeft相同但是它基于新的API(android 4.2)支持RTL
drawablePadding- 指定文本和drawable之间padding
```

- 同时使用ImageView的src和background属性实现点击效果

```xml
<ImageView
    android:id="@+id/image"
    android:layout_width="@dimen/batman_logo_width"
    android:layout_height="@dimen/batman_logo_height"
    android:background="?attr/selectableItemBackground"//点击效果
    android:src="@drawable/batman_logo_transparent"//图片
    style="@style/logo_image_style"/>
```

- 用LinearLayout自带的分割线

创建shape：divider_horizontal.xml


```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android">
    <size android:width="@dimen/divider_width"/>
    <solid android:color="@color/colorPrimaryDark"/>
</shape>
```

添加属性：

```xml
<LinearLayout android:layout_width="match_parent"
              android:layout_height="wrap_content"
              android:orientation="horizontal"
              android:background="@android:color/white"
              android:divider="@drawable/divider_horizontal"  //添加分割线
              android:dividerPadding="5dp" //设置padding
              android:showDividers="middle">//居中显示


    <TextView android:layout_width="0dp"
              android:layout_weight="0.5"
              android:layout_height="wrap_content"
              android:gravity="center"
              style="@style/Text.Title"
              android:text="@string/batman_name"/>

    <TextView android:layout_width="0dp"
              android:layout_height="wrap_content"
              android:layout_weight="0.5"
              android:gravity="center"
              style="@style/Text.Title"
              android:text="@string/superman_name"/>

</LinearLayout>
```

使用到的属性

```xml
divider -用来定义一个drawable或者color作为分割线
showDividers -指定分割线在哪里显示，它们可以显示在开始位置，中间，末尾或者选择不显示
dividerPadding -给divider添加padding
```
- 使用Space控件

```xml
<TextView 
		  android:layout_width="match_parent"
          android:layout_height="wrap_content"
          style="@style/Text.Title"
<Space 
          android:layout_width="match_parent"
          android:layout_height="10dp"/>//添加间距
<TextView 
          android:layout_width="match_parent"
          android:layout_height="wrap_content"
          android:text="@string/gotham_city_description"
          style="@style/Text.Details"/>
```

- 使用include和merge标签


