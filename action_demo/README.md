# action_demo

action_demo软件包，包括C++与Python两个版本的Action通信的示例。

## 功能介绍

本例需要自定义action文件，见[action/DoDishes.action](./action/DoDishes.action)。

C++版本代码见`src/`下的[dishes_Server.cpp](./src/dishes_Server.cpp)和[dishes_Client.cpp](./src/dishes_Client.cpp)。

Python版本代码见`scripts/`下的[dishes_Server.py](./src/dishes_Server.py)和[dishes_Client.py](./src/dishes_Client.py)。


## 运行方法

启动服务端

```sh
$ rosrun action_demo dishes_Server.py   #Python
$ rosrun action_demo dishes_Server        #C++
``` 

启动客户端

```sh
$ rosrun action_demo dishes_Client.py   #Python
$ rosrun action_demo dishes_Client        #C++
``` 

action是与编程语言无关的通信协议，因此收发双方无论用哪个语言来实现，都可以实现相互的action通信。
