# Problem

平时遇到的问题


## Vue

1. provide / inject 响应式

`provide` 值使用 `computed` 包一层

```javascript
setup(props) {
  provide(
    'data',
     computed(() => props.data)
  );
}
```

### 小程序

- input、textarea 无法通过 js 设置值

https://github.com/NervJS/taro/issues/2642

## Flutter

### 升级 Android 12 后无法使用真机调试
 
:bug: **ADB exited with exit code 1 Performing Streamed Install**

:bird: https://stackoverflow.com/questions/71763912/app-installation-error-install-parse-failed-manifest-malformed

### 无法使用 sentry_flutter 

:bug: 因 `minSdkVersion` 为 19 导致无法引入 sentry_flutter 后无法正常启动

:bird: minSdkVersion 改为 21,https://developer.android.com/studio/build/multidex
