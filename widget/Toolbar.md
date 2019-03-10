# Toolbar

[TOC]

[Why use toolbar](https://stackoverflow.com/questions/27238433/when-should-one-use-theme-appcompat-vs-themeoverlay-appcompat)
[]

颜色

> When using a base theme of Theme.AppCompat and the AppCompat-provided app bar, you’ll find the app bar’s background automatically uses your colorPrimary. However, if you’re using a Toolbar (along with a Theme.AppCompat.NoActionBar theme, most likely), you’ll need to manually set the background color.

```xml
<android.support.v7.widget.Toolbar
  android:layout_width="match_parent"
  android:layout_height="wrap_content"
  android:background="?attr/colorPrimary" />
```

> the `?attr/` format is how you tell Android that this value should be resolved from your theme rather than directly from a resource.