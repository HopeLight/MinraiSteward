# MiraiSteward

## Introduce

**If you want to know,It can do what?**

> Execute System Command and Screen gestrue and Control Music(Netease Cloud、QQMusic)
>
> > **Of course,If you want to realize public network,This is can do becuase I already have tested.**
> >
> >  One Step:
> >
> > > You only need to change Receving End Configuration File and must set Host Parameter values that your "Public Netework Internet Protocol" and Port Parameter values that your "Intranet Internet Protocol".
> >
> >  Two Setp:
> >
> > > You only need to change Sending End Configuration File and Must set Port t Parameter values that your "Public netework Internet Protocol".

### Sending end

> By Minrai Realizes that establishing socket sends. 
>
> In Plugin folder contains The Configuration File and You can Into that change parameter.(config.yml)
>
> ![](http://offsnow.top:40146/TestPhoto/3.png)



### Receiving end

> By some Encapsulation Class Realizes that establishing ServerSocket recives. 
>
> When you ready start "Receving End.jar",It can down in operation folder creates a Configuration File.
>
> ![](http://offsnow.top:40146/TestPhoto/4.png)

### Funcation List

> [指令] 系统指令
>
> > if you don't know What System Command has,You can click the link "https://www.jianshu.com/p/2761c8c51fab".
>
> [屏幕手势]
>
> > ↑ -> The Expression will can let mouse up the moving
> >
> > ↓  -> The Expression will can let mouse down the moving
> >
> > ← -> The Expression will can let mouse left the moving
> >
> > →  -> The Expression will can let mouse right the moving
> >
> > √  -> The Expression will can let mouse double the clicking
>
> [网易云] [QQ音乐] [音乐]
>
> > 播放，暂停、音量增大、音量减小、喜欢歌曲、歌词显示、上一首歌、下一首歌

### What Is HearBeat detection?

> HeartBeat detection:
>
> 作用:
>
> Firstly,HeartBeat detection usually is used for that network detection connects circumstance.	
>
> 首先,心跳检测经常用于网络检测连接情况。
>
> Secondly,Becuase of Network transmitting maybe can happen interrupted So for user guarantees That It very well experiences,HeartBeat detection is used for that Information channe connects  detection -- If some Object interrupted, immediately ready anew conneact.
>
> 其次,由于网络传输可能会出现中断的情况，所以为了保证用户体验良好，心跳检测用于通道连接检测 -- 一旦某一方挂掉了，就马上准备进行重连。 
>
> 原理:
>
> Sending End Can Give Receiving End Every Ten seconds That send a Empty Data Packet That will has Finished HeartBeat detection. If while sending throws The SocketException So illustrate Receiving end interrupted And Immediately anew create an Instantiation Socket Object That establish connection。
>
> 发送端会给接收端每10s为一个周期发送一个空包完成心跳检测。如果发送中抛出了异常说明接收端断开，然后立即重新创建一个实例化套接字对象来建立连接。
>
> Receiving End As Can Give Sending End Every Ten seconds That send a Empty Data Packet That will has Finished HeartBeat detection. If while sending also throws The SocketException So illustrate Sending End interrupted And anew ready wait that Sending End connects.
>
> 接收端同样会给发送端每10s为一个周期发送一个空包完成心跳检测，如果发送中也抛出了异常说明发收端断开，然后重新准备等待发送端连接。

## TestResults

![](http://offsnow.top:40146/TestPhoto/1.png)

![](http://offsnow.top:40146/TestPhoto/2.png)

> When you send "[指令]SystemCommand",MinraiBot can help you automatic transfer to receiving end and it execute SystemCommand.
>
> -- 当你发送 [指令]系统指令 给机器人,它可以帮你自动传给接收端来执行系统指令。

## How can I install it?

> HopeSteward-1.0-jar will install to Minrai Plugin in Folder
>
> > You only double click "start.bat" this scirpt.
>
> Choice one you like folder,"SystemControl-1.0-jar" drops to folder.
>
> > execute System Command -> Java -jar SystemControl-1.0-jar

## Original intention

> I can't want to closing my computer  because too lazy can't get up. -- Maybe is so~~

## Contact way

> My email: hjqy.xy@foxmail.com
>
> My QQ: 2622099140
>
> My Wechat: Null ~
