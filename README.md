# MiraiSteward

## Introduce

**If you want to know what can It help you?**

> Execute system command and screen gestrue and control music(Netease Cloud | QQMusic)
>
> > **Of course,If you want to realize public network,this is can do becuase I already have tested.**
> >
> >  One step:
> >
> > > You only need to change receving end configuration file and must set host parameter values that your "Public netework Internet protocol" and port parameter values that your "Intranet Internet protocol".
> >
> >  Two step:
> >
> > > You only need to change sending end configuration file and must set port parameter values that your "Public netework Internet protocol".

### Sending end

> By Mirai realizes as a sender who's messages send. 
>
> In plugin folder contains the configuration file and you can Into that change parameter.(config.yml)
>
> ![](http://offsnow.top:40146/TestPhoto/3.png)



### Receiving end

> By some encapsulation class realizes that establishing serversocket recives. 
>
> When you ready start "SystemControl-1.0-jar-with-dependencies.jar",It can down in operation folder creates a configuration file.
>
> ![](http://offsnow.top:40146/TestPhoto/4.png)

### List  of  Funcation 

> [指令] 系统指令
>
> > if you don't know some command of system,then you can click the link "https://www.jianshu.com/p/2761c8c51fab".
>
> [屏幕手势]
>
> > ↑ -> The expression will can let mouse up the moving
> >
> > ↓  -> The expression will can let mouse down the moving
> >
> > ← -> The expression will can let mouse left the moving
> >
> > →  -> The expression will can let mouse right the moving
> >
> > √  -> The expression will can let mouse double the clicking
>
> [网易云] [QQ音乐] [音乐]
>
> > 播放，暂停、音量增大、音量减小、喜欢歌曲、歌词显示、上一首歌、下一首歌

### What Is HearBeat Detection?

> HeartBeat detection:
>
> 作用:
>
> Firstly,heartbeat detection usually is used for that network detection connects circumstance.	
>
> 首先,心跳检测经常用于网络检测连接情况。
>
> Secondly,becuase of Network transmitting maybe can happen interrupted so for user guarantees that It very well experiences,heartBeat detection is used for that Information channe connects detection -- If some object interrupted, immediately ready anew conneact.
>
> 其次,由于网络传输可能会出现中断的情况，所以为了保证用户体验良好，心跳检测用于通道连接检测 -- 一旦某一方挂掉了，就马上准备进行重连。 
>
> 原理:
>
> Sending end can give receiving end every ten seconds that send a empty data packet that will has finished heartbeat detection. If while sending throws the socketexception so illustrate receiving end interrupted and Immediately anew create an Instantiation socket object that establish connection.
>
> 发送端会给接收端每10s为一个周期发送一个空包完成心跳检测。如果发送中抛出了异常说明接收端断开，然后立即重新创建一个实例化套接字对象来建立连接。
>
> Receiving end as It can give sending end every ten seconds that send a empty data packet that will has finished heartbeat detection. If while sending also throws the socketexception so illustrate sending end interrupted and anew ready wait that sending end connects.
>
> 接收端同样会给发送端每10s为一个周期发送一个空包完成心跳检测，如果发送中也抛出了异常说明发收端断开，然后重新准备等待发送端连接。

## Results of  Test 

![](http://offsnow.top:40146/TestPhoto/1.png)

![](http://offsnow.top:40146/TestPhoto/2.png)

> When you send "[指令]SystemCommand",minraibot can help you automatic transfer to receiving end and it execute command of system.
>
> -- 当你发送 [指令]系统指令 给机器人,它可以帮你自动传给接收端来执行系统指令。

## How can I install it?

> HopeSteward-1.0-jar will install to minrai plugin in folder
>
> > You only double click "start.bat" this scirpt.
>
> Choice one you like folder,"SystemControl-1.0-jar" drops to folder.
>
> > execute system command -> Java -jar SystemControl-1.0-jar

## Original Intention

> I can't want to closing my computer because too lazy can't get up. -- Maybe reason is so~~

## Contact way

> My email: hjqy.xy@foxmail.com
>
> My QQ: 2622099140
>
> My Wechat: Null ~
