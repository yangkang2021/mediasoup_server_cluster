## Protoo

1. Protoo协议：https://protoo.versatica.com/
    - 实现了基于json的传输协议。
    - 但没有实现网络传输transport，需要用户按照接口实现网络传输，可以用websocket或tcp，甚至dup实现。
    - 消息分三类：
        - Request(request，id，method，data)
            - <span style="background-color: #red"><font size=4 color=#DC143C> 请求消息，回调给用户处理并需要回复：accept或reject。</font></span>
        - Response(response，id，ok，data/errorCode/errorReason)
            - 回复消息，发包结果需要回调给用户：resolve或reject。
        - Notification(notification，method，data)
            - 通知消息，需要回调给用户。
    - 初始化传入transport和监控listener。request函数发包和收到Response都回调给用户。
2. 官方js版本protoo-client的用法
