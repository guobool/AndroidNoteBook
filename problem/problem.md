# getLayoutParam

只有使用 xml 实例的View getLayoutParam 才能得到 LayoutParam。使用 new 的对象但是没有设置 LayoutParam 的对象，get的结果为 null。

不建议使用 new 来设置 layoutParam, 不同版本的 LayoutParam 会有些问题，4.4 版本 GridView 使用 TextView 设置了LayoutParam 之后就会爆出

android.widget.ViewGroup$LayoutParams cannot be cast to android.widget.AbsListView$LayoutParams

使用带父布局参数的函数才能成功传入 LayoutParams。
```
convertView = mInflater.inflate(R.layout.item_phonetic, parent,false);
```

使用两个参数的 inflate 获的的 LayoutParams 仍然为 null

```
convertView = mInflater.inflate(R.layout.item_phonetic, null);
```

1. 为什么 5.0 之后的版本不会出现这种问题？
2. 为什么使用 inflate 实例的 View 能够正常传入 LayoutParam 的类型 ？


## 升级版本一定遵循官方指南，将所有的都改了

百度 TTS 的bug 太沉重了，每次升级版本，牵涉到的不只是表面看到的编译错误，还有许多运行时错误，会牵涉到其中。新的安卓版本可能对软件有不同要求，这些都需要跟着改

```
<uses-library
      android:name="org.apache.http.legacy"
      android:required="false" />
```

https://developers.google.com/maps/documentation/android-sdk/config#specify_requirement_for_apache_http_legacy_library


## 印象大的问题，一定要定位准确，推理要有理有据，不能根据猜测。
