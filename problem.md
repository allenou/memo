# Problem

平时遇到的问题

## Javascript

1. js-xlsx 导入 excel 后日期和百分比值被改变

```javascript
const target = e.target.result;
const wb = XLSX.read(target,{ raw: false, dateNF: 'yyyy-mm-dd' });
const data = XLSX.utils.sheet_to_json(wb.Sheets[wb.SheetNames[0]], { raw:false, dateNF:'yyyy-mm-dd' });
```

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

1. input、textarea 无法通过 js 设置值

<https://github.com/NervJS/taro/issues/2642>

1. 自定义 Tabbar 第二次点击后无法高亮

原因 Tabbar 页面第一次打开后已被缓存
```javascript
onShow(){
  // 在这设置一遍高亮
}
```

## Flutter

### 升级 Android 12 后无法使用真机调试

:bug: **ADB exited with exit code 1 Performing Streamed Install**

:bird: <https://stackoverflow.com/questions/71763912/app-installation-error-install-parse-failed-manifest-malformed>

### 无法使用 sentry_flutter

:bug: 因 `minSdkVersion` 为 19 导致无法引入 sentry_flutter 后无法正常启动

:bird: minSdkVersion 改为 21,<https://developer.android.com/studio/build/multidex>


## 其它

1. [pnpm 使用不同 npm registry 无法安装 package](https://github.com/pnpm/pnpm/issues/3361#issuecomment-821238867)
