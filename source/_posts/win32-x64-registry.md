---
title: 64位Windows下32位应用程序访问64位注册表键值，或者反过来
date: 2016-04-26 14:32:42
tags:
  - Visual Studio
  - C
---
本来以为64位Windows下，32位app只能访问32位注册表键值，64位app只能访问64位，原来可以很简单地通过以下两个flag来实现互通：
```
KEY_WOW64_64KEY
KEY_WOW64_32KEY
```
可以应用的函数包括：
[RegCreateKeyEx][2]
[RegDeleteKeyEx][3]
[RegOpenKeyEx][4]

MSDN：[Accessing an Alternate Registry View][1]

[1]:http://msdn.microsoft.com/en-us/library/windows/desktop/aa384129(v=vs.85).aspx
[2]:https://msdn.microsoft.com/en-us/library/windows/desktop/ms724844(v=vs.85).aspx
[3]:https://msdn.microsoft.com/en-us/library/windows/desktop/ms724847(v=vs.85).aspx
[4]:https://msdn.microsoft.com/en-us/library/windows/desktop/ms724897(v=vs.85).aspx
