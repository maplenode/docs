# 2.4 Editing the TN-mainnet.conf file

This step will show you how to modify you config file. You will need to change few config to personalize and setup your node.

Open your TN-mainnet.conf file in /opt/turtle

```
sudo nano TN-mainnet.conf
```

#### Change the following defaults;

##### \# TN node settings

> ~~\# ~~node-name = "~~My MAINNET node~~"

Remove the \# then put your node name into " ".

```
node-name = "Your Node Name"
```

> ~~\# ~~declared-address = "~~1.2.3.4:6868~~"

Remove the \# then put your static IP

```
declared-address = "yournodeip:6860"
```

##### \# Wallet settings

> password = "~~ridetheTN!~~"

Change password ridetheTN! with your password. This will secure your wallet.dat in your VPS

```
password = "yourpassword"
```

> ~~\# ~~seed = ""

Remove the \# then put your ENCODED SEED noted before in [section 2.3](/23-create-tn-wallet.md)

##### \# Node's REST API settings

> enable = ~~no~~

Change 'no' to 'yes'

```
enable = yes
```

> bind-address = "127.0.0.1"

Change bind-address with 0.0.0.0 , This will allow you to use REST API \(swagger\) with your web browser. We will put back 127.0.0.1 later

```
bind-address = "0.0.0.0"
```

> ~~features {~~
>
> ~~    supported = \[1, 2, 3, 5, 6\]~~
>
> ~~  }~~

To add new new supported feature to your node, replace this section with

```
features {
auto-shutdown-on-unsupported-feature = yes
supported = [1, 2, 3, 5, 6,8]
}
```

#### 

#### Next step will show you how to start your node and download blockchain.



