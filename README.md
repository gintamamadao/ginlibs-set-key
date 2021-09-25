[![NPM version](https://badgen.net/npm/v/ginlibs-set-key)](https://www.npmjs.com/package/ginlibs-set-key)
[![NPM Weekly Downloads](https://badgen.net/npm/dw/ginlibs-set-key)](https://www.npmjs.com/package/ginlibs-set-key)
[![License](https://badgen.net/npm/license/ginlibs-set-key)](https://www.npmjs.com/package/ginlibs-set-key)

# ginlibs-set-key

ginlibs-set-key

可以通过路径字符串读取或修改 object 的内层的值

## 使用例子

```js
import { setKey, getKey } from 'ginlibs-set-key'

const obj = {}
setKey('a.b[0]', 1, obj)
// obj 的值变成
// {
//   a: {
//     b: [1],
//   },
// }

getKey('a.b[0]', obj)
// 得到值 1
```

## API

### `setKey(key, val, obj)`

- `key` 是赋值的路径
- `val` 是要赋予的值
- `obj` 是要处理的对象

```js
setKey('a.b[0]', 1, obj)
```

### `getKey(key, obj)`

- `key` 是赋值的路径
- `obj` 是要处理的对象

```js
getKey('a.b[0]', obj)
```
