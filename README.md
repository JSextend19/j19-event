# j19-event
这是一个关于event的实现

---

*author* : **usernameisregistered**

*email*：**liming_longxi@163.com**

*buildDate*:**2019年10月27日 12:51**

---

## 安装  npm i @jsextend19/j19-event

## 引入

```
import { J19Event , J19ErrorEvent , J19DispatchEvent } from "@jsextend19/j19-event"

```

## 事件相关说明文档

- [Event 基本事件](./doc/event.md)
- [ErrorEvent 错误事件](./doc/errorEvent.md)
- [DispatchEvent 事件分派](./doc/eventDispatch.md)

## 注意
| 函数名称 | 描述 | 参数 |
| - | - | - |
| apply | 方法调用一个具有给定this值的函数 | thisArg, [argsArray] |
| call | 使用一个指定的 this 值和单独给出的一个或多个参数来调用一个函数 | thisArg, arg1, arg2, ... |
| bind | 会创建一个新绑定函数 | thisArg[,arg1[,arg2[, ...]]] |

### 绑定函数[bound function，BF]
[[BoundTargetFunction]] - 包装的函数对象
[[BoundThis]] - 在调用包装函数时始终作为this值传递的值。
[[BoundArguments]] - 列表，在对包装函数做任何调用都会优先用列表元素填充参数列表。
[[Call]] - 执行与此对象关联的代码。通过函数调用表达式调用。内部方法的参数是一个this值和一个包含通过调用表达式传递给函数的参数的列表。

绑定函数也可以使用new运算符构造，它会表现为目标函数已经被构建完毕了似的。提供的this值会被忽略，但前置参数仍会提供给模拟函数。