## Cookie 操作工具类

## 调用方式

### 普通引入方式

`<script type="text/javascript" src="/cookie-util/index.js">`


### AMD
```
require(['cookie-util'], function(CookieUtil){

  //cookie方法操作

})
```

### CMD

```
import CookieUtil from 'cookie-util';
```

### Node （暂未发布到公共npm平台）

`npm install 'cookie-util';`


## 设置方法
```
/**
 * @param name {String} cookie名
 * @param value {String} cookie值
 * @param expires {Date} 过期时间 若不设置 默认为30天
 * @param domain {String} 域
 * @param path {String} 路径
 * @param secure {boolean} 是否启动安全模式
 */
CookieUtil.set(name, value, expires, domain, path, secure);
```

## 获取方法

```
/**
 * @param name {String} cookie名称
 * @param decode {boolean} 是否解码
 */
CookieUtil.get(name, decode);
```

## 删除方法

```
/**
 * @param name {String} cookie名
 * @param domain {String} 域
 * @param path {String} 路径
 * @param secure {boolean} 是否启动安全模式
 */
CookieUtil.deleteCookie(name, domain, path, secure);
```

## 解码方法

```
/**
 * @param str {String} 需要解码的字符串
 * @return newStr {String}
 */
CookieUtil.decodeStr(str);
```
