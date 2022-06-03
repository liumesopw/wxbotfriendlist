# wxbotfriendlist
PC微信机器人之实战分析微信获取群好友列表
今天讲一下微信获取群成员列表的功能，首先先找一个群，知道这个群的id，然后附加微信到CE，原理就是点击某个微信群的时候，他会取出该群的所有成员列表信息，当切换点击的时候，CE上面会显示不同的群id，先切换个人的微信，然后搜索wxid_，过滤一些数据。
![image](https://user-images.githubusercontent.com/96330669/171816633-ceffba5b-dc1c-4198-968a-09f9ca4ccbb5.png)
然后切换到某个群，就直接显示某个群的id了，然后记录下来这个群的id，然后再切换到其他群，继续过滤，剩下7条数据了。
![image](https://user-images.githubusercontent.com/96330669/171816671-d518bc5b-4fdc-448d-a63c-f76613ec7c41.png)
![image](https://user-images.githubusercontent.com/96330669/171816687-70542b67-05b1-455d-8179-605ca5377a28.png)
然后把过滤到的，移到下面，然后选择几个修改后面的Value值为另外一个群的id，如果切换后跟着变化，说明就是这个地址，然后复制到OD里面，下断点
![image](https://user-images.githubusercontent.com/96330669/171816715-43346f93-0986-4428-bf74-75ab880d96e9.png)
给找到的地址下一个内存访问断点，然后点击一下微信群，他就断下来了，
然后一直走断点找到wxid，
![image](https://user-images.githubusercontent.com/96330669/171816740-12be7f55-463c-4eb1-b9c5-3e9a1016add8.png)
![image](https://user-images.githubusercontent.com/96330669/171816757-78e5d69d-3ecb-48fd-bd98-ed1cb0344d58.png)
个微：
目前已经实现了大部分功能，运行稳定，比如：发各种消息，
接收各种消息，群管，下载文件，加好友，检测僵尸粉，获取朋友圈，发送朋友圈，点赞发评论等等功能，
可提供接口，方便各种语言二次开发，欢迎技术交流。

Q：2645542961

企微：
目前已经实现了大部分功能，运行稳定，比如：发各种消息，
接收各种消息，外部群内部群管理，下载文件，加好友等等功能，
可提供接口，方便各种语言二次开发，欢迎技术交流。

![image](https://user-images.githubusercontent.com/96330669/171817003-135608da-0cd1-4bd4-ab1d-6eac007868d1.png)
