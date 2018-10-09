# Create new user

Create a local App user with sudo rights.

It will be more secure than using root.

1. [ ] Issue the following command: adduser \*yournodename\*

```
adduser testnode
```

1. [ ] Add the new username into the sudo group with the following command: usermod -aG sudo \*yournodename\*

```
usermod -aG sudo testnode
```

1. [ ] Logout as root

```
Close putty or CRTL+D
```







