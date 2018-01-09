## 通信同步模块

通信同步模块中采用普通socket通信的方式实现。模块输入端接收来自于中控模块的发出的信号命令，打开socket通信模块，各设备在服务器端打开通信模块后与提前开启的各自通信模块进行连接，接收来自服务端发送的操作命令控制符。服务器需对各显示节点的线程进行监控，并接收来自各节点的返回信息，通过服务器端接收到的返回信息处理判断当前各节点同步情况后再次返回各节点进行帧调整的一个循环过程来达到各节点显示设备的视频同步。

![](/assets/通信同步模块.png)
