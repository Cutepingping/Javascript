# function-stage-1
   使用了我们定义的第一个参数msgText，对于第二个参数msgType，这个就涉及了稍微多一点的东西— 我们要设置一些依赖于这个 msgType 参数的东西, 我们的函数将会显示不同的图标和不同的背景颜色。
   来解释下, 如果第二个参数 msgType 的值为 'warning', 我们的消息框将显示一个警告图标和一个红色的背景. 如果这个参数的值是 'chat', 将显示聊天图标和水蓝色的背景. 如果 msgType 没有指定任何值 (或者不是'warning'和'chat'), 然后这个 else { ... } 代码块将会被执行, 代码的意思是给消息段落设置了一个简单的左内边距并且没有图标, 也没有背景颜色。这么做是为了当没有提供 msgType 参数的时候给函数一个默认行为, 意思是这是一个可选参数（你没发现？其实我们已经用过了！就在这里btn.onclick = function() { displayMessage('Woo, this is a different message!'); };只是当时我们没有写这个else段，也就是啥操作也没做）！
