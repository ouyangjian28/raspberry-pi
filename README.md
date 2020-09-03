# raspberry-pi

## troubles
need to set up raspberry pi4's resolution otherwise it will be black screen accessed remotely without plugging in a monitor

[headless raspberry-pi ssh](https://www.raspberrypi.org/documentation/remote-access/ssh/passwordless.md)

网上还有分析为ssh主机被人黑了，并在消除入侵记录时对known_hosts文件做了改动。当然也不排除这种可能，但我估计我是没那个福气了：）

解决方案：

删除~/.ssh/known_hosts文件，或者如果你可以判断出known_hosts中原ssh服务器的公钥，删去那部分，

然后后再次建立新的连接，即可获得新的公钥。
