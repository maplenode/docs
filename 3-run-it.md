# 3. Run it

This step will show you how to run your node with tmux session

[**tmux**](https://en.wikipedia.org/wiki/Tmux)** **allowing a user to access multiple separate terminal sessions inside a single terminal window or remote terminal session.

Open tmux session

```
tmux
```

> maplenode@maplenode-website:~/docs$
>
> \[0\] 0:bash\*                                                           "maplenode-website" 01:54 09-Oct-18

Make sure to be in your node directory /opt/turtle

```
cd /opt/turtle
```

Start your node

```
java -jar TN-all-0.13.6.jar TN-mainnet.conf
```

> 2018-10-08 20:55:21,340 INFO  \[main\] c.w.Application$ - Starting...
>
> 2018-10-08 20:55:22,182 INFO  \[main\] kamon.Kamon$Instance - Initializing Kamon...
>
> 2018-10-08 20:55:22,592 INFO  \[main\] kamon.Kamon$Instance - Kamon-autoweave has been successfully loaded.
>
> 2018-10-08 20:55:22,593 INFO  \[main\] kamon.Kamon$Instance - The AspectJ load time weaving agent is now attached to the JVM \(you don't need to use -javaagent\).
>
> 2018-10-08 20:55:22,595 INFO  \[main\] kamon.Kamon$Instance - This offers extra flexibility but obviously any classes loaded before attachment will not be woven.
>
> 2018-10-08 20:55:26,757 INFO  \[ctor.default-dispatcher-5\] a.event.slf4j.Slf4jLogger - Slf4jLogger started
>
> 2018-10-08 20:55:27,342 INFO  \[main\] c.w.Application$ - TN v0.13.6 Blockchain Id: L
>
> 2018-10-08 20:55:34,511 INFO  \[main\] c.w.n.PeerDatabaseImpl - Loaded 30 known peer\(s\) from peers.dat
>
> ....
>
> 2018-10-08 20:55:37,294 INFO  \[nio-worker-group-3-3\] c.w.n.HandshakeHandler$Server - \[06628c86 206.189.187.215:47184\] Accepted handshake Handshake\(TNL,\(0,13,6\),MapleNode \#2 3JtJ5Kf3XuAUiMhtDQasSPdpaG6X5WLa8cE,501045,Some\(/206.189.187.215:6860\)\)
>
> 2018-10-08 20:55:37,352 INFO  \[appender-46\] c.w.s.BlockchainUpdaterImpl - New height: 239158

Now your node will stay online when you will close your ssh session.

To to go back into your tmux session, simply do this command

```
tmux attach -t 0
```

0 = session \# 

