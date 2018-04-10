#dopass

Dopass的安全性高吗？

1. 非常高，如果自定义内置key，则无法破解。



2. 查看dopass源码可以发现内置了一个key(crypt.js:16)，如果破解者知道是使用dopass算法进行加密的，那破解难度和用户的key成正比关系。



3. 但是如果破解者不知道是使用dopass加密或者 **用户自行修改了内置key**，那么将无法破解，即使把全球所有的计算资源加起来，也不可破解。



**警告，如果你自行修改了内置key，请一定要保存好，否则只能期待外星人帮你解密了**

演示：

![dopass](https://github.com/BuNuo/dopass/blob/master/dopass.png)

