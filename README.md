# FuckHR
[WIP] Anti huorong anti-virus.绕过火绒免杀专用方法。

唔 我骗你了，其实不是工具包。

思路有3：

1 过静态。

PE切片。一般来说切片注意2类重复。

呃，POC我就不放了，但是你要听好。

以前的切片工具，是[0.1k][1k.2k][2k.3k]

这样有一个问题。特征码可能被切开。

正确方法是[0.2k][1k.3k][2k.4k][3k.5k]

ok，拿到特征码以后直接插nop，位置不够就掐jmp吧，把特征码中间一部分移到代码段末尾，用jmp粘好。

2 过动态。

这个有一个无脑方法。弹窗“你是否不同意软件许可协议”

HR的沙箱永远是“是”。

或者检测鼠标，那个啥都行，比如说什么按钮是不是用鼠标按的。

想想嘛。那么大个按钮，鼠标移进去是不是至少有10个mouseevent？

ok。

3 过手动。

这个其实更简单

直接每次启动改写pe后面的10个byte就行。

就是 exe 发布前先写10个花byte。

启动时 懂得都懂。

结束

再见

不对，放个POC吧

https://x.threatbook.com/v5/article?threatInfoID=34373
