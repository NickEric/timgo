timgo是tim即时聊天的golang客户端 <br/>
连接服务器与发送信息等操作都比较简单 <br/> 
1. 新建Conf对象，并主要几个属性赋值，包括用户名(Name)，密码(Pwd)，域名(Domain),资源(Resource) <br/>
   同时服务器掉用客户端方法是，需要实现几个回调的方法 <br/>
   AckListener   <br/>
   MessageListener  		实现客户端处理服务器推送的信息   <br/>
   PresenceListener 		实现客户端处理服务器推送的好友状态信息   <br/>
   MessageListListener		实现客户端处理服务器推送的信息，对象为信息集合   <br/>
   PresenceListListener		实现客户端处理服务器推送的好友状态信息，对象为信息集合  <br/>
2. 连接服务器client.NewConn，需要提供ip与端口  <br/> <br/>
 
具体操作请参考 timgo.go  ，有任何问题请随时email到donnie4w@gmail.com 谢谢！
   