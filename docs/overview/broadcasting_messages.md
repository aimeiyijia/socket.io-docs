## 广播消息
- 广播时不支持回调

要进行广播，只需添加广播标志即可发出和发送方法调用。 广播意味着向除了启动它的socket之外的所有人发送消息。


### Server
```js
const io = require('socket.io')(80)
io.on('connection',(socket)=>{
    socket.broadcast.emit('user connected')
    socket.broadcast.to('socketId').emit('hi',"hi") //给指定人发送
})
 ```
