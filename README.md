# 一道面试题

❓ 当你在浏览器输入 `google.com` 后发生了什么
总原则：以面试知识点为基本纲领。通常经典面试题正好也是涉及每个领域里最基本和重要的知识点。
总的参考原则：参考经典面试题的经典解答，参考著名大学课程的内容。但是引用时一定要引用到最原始的文献，比如各种RFC。
内容深度：以讲清楚基本原理，基本概念，便于快速准确用口语讲述（这毕竟是面试题）。每一个知识点自成体系，可以单独拿出来讲。
涉及基本知识点同时兼顾前沿，例如穿插4G，5G，ipv6等知识。
提炼几根暗线：1、网络日益变快 2、内容日益丰富 3、系统日益安全

- 按下g开始：键盘中断，字符串补全
- 按下回车键：判断是URL不是搜索关键字，www补全，http(s)协议补全
- 杀毒介入：判断是否是危险的域名
- DNS 查询
  - 本机缓存
  - 递归查询
  - 如果没墙?（基本版本，讲基础知识的分支）；如果有墙?（高级版本，另外一个关于网络安全的大分支）
- 浏览器补全协议猜测（顺序是否在前面？）
- 转换非 ASCII 的 Unicode 字符（有吗？）
- HTTP 请求
  - 发出第一个请求
  - HTTP数据包---TCP三次握手什么的---IP(v4,v6)和路由---MAC层(ARP)---物理层（电，光，WiFi，4G），本条参考计算机网络基础，无线通信基础
  - CDN什么的？
  - 服务器端：网卡缓存接收，操作系统协议栈，层层解包到HTTP Server
  - HTTP 302
  - HSTS（我感觉HSTS可能要开一个大分支）
  - 被墙阻断?（分支）
- HTTP 响应（前后端）
- 基本版本也要有防火墙，WAF等网络安全标配。
- 很多服务器的事，计算机处理信息的过程也可以放在这里讲，在客户端那里少讲一点。篇幅够一直可以降到服务器的供电和散热。篇幅少点就讲基本的网卡，CPU，内存，外存。计算机体系结构只提流水线和多级缓存。
- 内容传输和TCP（这个有来回，要不放一起讲，比如HTTP请求那里）
- 数据层层拆包，最后拿到HTML响应
- 浏览器终于收到响应了
  - HTML解析
  - 页面 HTML 渲染
  - JavaScript 引擎
  - GPU加速
- 显示卡将数据光栅化，通过视频线输出（台式机VGA，HDMI，DP，笔记本LVDS，手机用啥的来着，反正就讲2类：1模拟VGA，2各种数字接口）
- 显示器
  - 颜色LUT，驱动显示内容
  - 液晶，OLED屏幕原理（可补充CRT，DLP投影）
  - 字体渲染和修饰，亮度自动调节

### 参考文献
参考同行：https://github.com/alex/what-happens-when/blob/master/README.rst
不要忘记前面的总原则！
