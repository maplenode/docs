# 2.5 Start your node for first time

This step will show you how to run your node for first time and download blockchain.

Make sure you are in your node directory \( /opt/turtle \)

```
cd /opt/turtle
```

Start your node with this command;

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

Just wait the blockchain to download !

Browse to [explorer](https://explorer.blackturtle.eu/peers) and confirm your node is listed.

If you see your node, than you're good







