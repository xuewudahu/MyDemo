## android与H5界面的交互

1.存在android调用H5和H5调用android两种。

2.在android调用H5的交互中

```bash
WebView.loadUrl("javascript:method(" + "'" + param+ "'" + ")");
```

需要初始化WebView，进入H5界面后进行相关逻辑。

3.在H5页面调用android的交互

需要使用@JavaScriptInterface标记

```cpp
    WebView.addJavascriptInterface(new JsInterface(), tag);
```

不熟悉。需要继续查看

