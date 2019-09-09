## eventEmit
on: 订阅 <br>
emit: 发布 <br>
emit: 发布 <br>

#### 继承events模块
```js
var events = require('events')
var util = require('util')
function Stream() {
  events.EventEmitter.call(this)
}
util.inherits(Stream, event.EventEmitter)
```

#### 如何理解 new events.EventEmitter().once()
如何解决同步锁问题

#### 用




