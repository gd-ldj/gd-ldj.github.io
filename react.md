## 第二遍学习react官方文档收获
+ 1、使用箭头函数传参 onClick = { (id) = {this.handleClick(id)}}
+ 2、条件渲染的 && 方法  { true && <div>hello word</div> }
+ 3、state 只在交互的时候出现 静态数据是从父级传到子级
+ 4、条件渲染
> 值得注意的是，JavaScript 中的一些 “falsy” 值(比如数字0)，它们依然会被渲染。例如，下面的代码不会像你预期的那样运行，因为当 props.message 为空数组时，它会打印0:
  <div>
    {props.messages.length &&
      <MessageList messages={props.messages} />
    }
  </div>
 改为 请确保 && 前面的表达式始终为布尔值
 <div>
    {props.messages.length > 0 &&
      <MessageList messages={props.messages} />
    }
  </div>
