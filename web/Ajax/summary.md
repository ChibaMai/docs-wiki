# Ajax 总结

## 如果接口使用`http`的`get`方法

这个接口，可以使用浏览器的地址栏直接验证        

> [!NOTE|style:flat]
> 注意: `restful`的无参数`get`方法，和`http`的无参数`get`方法相同

`restful`的`pos`t方法，和`http`的`post`相同

## 功能模块编写思路

| 前端 | 后端 |
| --- | --- |
| 1. 收集整理数据---`get`，`delete`非空验证 <br>2. `ajax`的`xhr4`步 <br>3. 在`if(xhr.readyState==4&........)` <br> 4. 中写`dom`操作，把得到响应数据呈现在`html`上 | 1. 接收前端传过来的数据<br> 2. 写`sql`语句<br> 3. 连接池进行数据操作 <br> 4. 返回的响应越短越好 |

## 课后任务

%accordion%提高题%accordion%
- 对注册的用户名，进行验证
  ```
  逻辑：
    1.失去焦点时调用  onblur

    2.如果查到有这个用户名，说明当前用户名不可用
      如果没有查到这个用户名，说明当前用户名可以注册

    3.要创建要给bool的变量，当次变量为true的时候
      可以注册，为false的时候不可以注册

    4.用户名不可用，为false,两次输入密码不一致为false
      某一个字段为空，为false
  ```
%/accordion%
