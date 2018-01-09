## 项目随笔
1、点击div模拟的假的input，使之展现出真正的input输入框，并且同时获得焦点。
  > 刚开始是设置state展示input与获取焦点this._textArea.focus()同时了，导致还没出现input，就想获取焦点，坑定不会获取到。解决办法
  > this.setState({
        inputFlag: true
       },() => {
        this._textArea.focus()
       })
