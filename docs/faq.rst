Wireshark FAQ
=============
1. 介绍
--------------------
1.1 Wireshark是什么？
  * Wireshark®是基于网络协议的分析工具，通过它您可以捕获和交互式地浏览流动在计算机网络中的流量。它功能强劲，是世界上最流行的网络协议分析工具，兼容于Windows，macOS，Linux和UNIX等绝大多数平台，广泛应用于网络、安全、开发、教育等领域。作为开源软件，Wireshark完全免费，适用GPL2协议授权。
  * Wireshark由全球网络协议专家组成的团队维护，它是一项颠覆性的杰作。
  * Wireshark曾用名Ethereal，详情请参见下一节。如果您仍在使用Ethereal，考虑到它已经停止维护并具有已知的安全缺陷，我们强烈建议您升级至Wireshark。
  * 详情请移步 `关于Wireshark`_ 页面
  .. _关于Wireshark: https://www.wireshark.org/about.html

1.2 为什么Ethereal要改名？Wireshark是它的分支吗？
  * 2006年5月，工作于CACE Technologies（WinPcap的开发公司）的Gerald Combs（Ethereal的作者）出于某些原因不得不停止使用Ethereal的商标。出于该项目的延续，Ethereal以Wireshark的新名字重生。你可以认为Wireshark是Ethereal的一个“分支”——它们来自同一开源项目，但具有不同的名字、不同的主页、不同的开发团队和不同的支持团队，但你也应当注意到所有的Ethereal核心开发团队目前都工作于Wireshark。自改名以来，Ethereal不再进行过任何的维护，Ethereal的部分网站（包括邮件列表、源码仓库和build farm）也已下线。
  * 详情请参见：
  * `Original press release`_
  * `NewsForge article`_
  * Many other articles in `our bibliography`_
  .. _Original press release: http://www.prweb.com/releases/2006/6/prweb396098.htm
  .. _NewsForge article: http://archive09.linux.com/articles/54968
  .. _our bibliography: https://www.wireshark.org/bibliography.html

1.3 去哪里寻求帮助？
  * 你可以到 `Q&A site`_ 以及Wireshark用户邮件列表寻求社区的帮助。
  * 订阅信息和邮件归档可以在这里查询：https://www.wireshark.org/mailman/listinfo。
  * IRC频道可以在这里查询：irc://irc.freenode.net/wireshark。
  * 自学Wireshark可移步 `Wireshark University`_ ，您可通过Wireshark认证网络分析师项目获得认证资质。
  .. _Q&A site: https://ask.wireshark.org/
  .. _Wireshark University: http://www.wiresharktraining.com/

1.4 什么样的shark才是Wireshark？
  * 反正就是那种特别牛X的shark什么的。

1.5 Wireshark的发音、拼写和首字母大写？
  * Wireshark的发音正如你所见，先念wire再念shark。
  * 至于重读音节可以随您的喜好任意取之。
  * 比如在阿肯色州，重音在前，驼峰式的读法是不存在的。

1.6 Wireshark多少钱？
  * Wireshark是免费软件，您可以无限制地、免费地下载和使用全功能的Wireshark。
  * Wireshark适用 `GPL2协议`_ 授权，详情请参见 `GPL FAQ`_ 。
  .. _GPL2协议: https://www.gnu.org/licenses/gpl-2.0.html
  .. _GPL FAQ: https://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html

1.7 我刚刚在淘宝上付费买了一份Wireshark！我难道被骗了？！
  * 视情况而定。他们是否提供了任何形式的具有附加价值的产品或服务？例如协助安装、提供安装媒介、解答您的问题、为您提供课程或者赠送了您一副酷炫狂拽吊炸天的鲨鱼袜子？哦，很可惜，这样幸运的情况极其罕见。
  * Wireshark是完全免费的软件，它允许任何人在任何地点、任何时间不受限制地 `下载`_ 和使用。如果您为此支付了任何酬劳，您理当接受除此以外的其他服务或产品。
  .. _下载: https://www.wireshark.org/download.html

1.8 我可以将Wireshark用于商业用途吗？
  * 是的，包括但不限于::
   #. 您为商业组织工作；
   #. 您利用Wireshark捕获和分析公司或客户的网络流量。
  * 如您欲将Wireshark作为您商业产品的一部分，请参见 :ref:`下一节<节1.9>` 。

.. _节1.9:

1.9 我可以将Wireshark作为我的商业产品的一部分吗？
  * 正如上文所提到的，Wireshark基于 `GPL2协议`_ 授权，该协议限制了您在借用GPL式代码时的情境。比如您不能发售和强制他人使用Wireshark的衍生产品，您必须公开您对Wireshark源代码的修订，Wireshark的衍生产品必须继承GPL授权等等。详情请参见 `GPL FAQ`_ ，特别地，请着重阅读” `关于修订GPL式代码并转售的相关问题`_ “和” `关于调用GPL式代码并发布专有程序的相关问题`_ “两节的内容。
  * 你可以调用GPL式代码，正如GPL FAQ中 `专有程序中的GPL`_ 一节所说，例如调用Wireshark的代码编写一个商业程序，只要他们彼此间是独立的。
  * 我们建议你保持Wireshark和你的产品之间完全分立，以socket和pipe的形式进行通信。如果你以DLL的形式加载了Wireshark的任何一部分，你可能会因此惹上不必要的麻烦。
  .. _关于修订GPL式代码并转售的相关问题: https://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#GPLCommercially
  .. _关于调用GPL式代码并发布专有程序的相关问题: https://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#LinkingWithGPL
  .. _专有程序中的GPL: https://www.gnu.org/licenses/old-licenses/gpl-2.0-faq.html#GPLInProprietarySystem

1.10 Wireshark目前支持什么网络协议？
  * Wireshark目前支持数百种网络协议和媒介。
  * 详情请参见man手册：`wireshark(1)`_ 。
  .. _wireshark(1): https://www.wireshark.org/docs/man-pages/wireshark.html

1.11 未来是否有明确的计划以支持新的网络协议？
  * 没有，Wireshark何时能够支持新的协议完全取决于社区贡献的多寡。

1.12 Wireshark是否可以加载其他网络分析器截获的数据？
  * 是的，多亏了社区的努力，Wireshark支持加载某些特定的网络分析器截获的数据，但是对于那些尚不支持的和将来新出现的格式，未来没有明确的计划。
  * 如果某个网络分析器将截获的数据以Wireshark支持的格式写入文件，那么Wireshark可以直接加载，除非该网络分析器对文件格式进行了某种扩展。
  * 如果该网络分析器以专有的格式保存文件，那么该文件必须经过转换Wireshark方可加载，这通常需要利用反向工程的方法。应当注意到，没有保证反向工程一定成功。

1.13 哪些设备可用于捕获数据？
  * 详情请参见”the list of supported capture media on various OSes“。请注意，”Unknown“并不意味着该设备不可用于在Wireshark中捕获数据，仅表示我们尚不清晰它的兼容性，如果您发现该设备可用，望您向社区报告以利其他的使用者。
  * Wireshark支持许多文件格式，包括但不限于::
   #. AG Group/WildPackets/Savvius EtherPeek/TokenPeek/AiroPeek/EtherHelp/Packet Grabber captures
   #. AIX's iptrace captures
   #. Accellent's 5Views LAN agent output
   #. Cinco Networks NetXRay captures
   #. Cisco Secure Intrusion Detection System IPLog output
   #. CoSine L2 debug output
   #. DBS Etherwatch VMS text output
   #. Endace Measurement Systems' ERF format captures
   #. EyeSDN USB S0 traces
   #. HP-UX nettl captures
   #. ISDN4BSD project i4btrace captures
   #. Linux Bluez Bluetooth stack hcidump -w traces
   #. Lucent/Ascend router debug output
   #. Microsoft Network Monitor captures
   #. Network Associates Windows-based Sniffer captures
   #. Network General/Network Associates DOS-based Sniffer (compressed or uncompressed) captures
   #. Network Instruments Observer version 9 captures
   #. Novell LANalyzer captures
   #. RADCOM's WAN/LAN analyzer captures
   #. Shomiti/Finisar Surveyor captures
   #. Toshiba's ISDN routers dump output
   #. VMS TCPIPtrace/TCPtrace/UCX$TRACE output
   #. Visual Networks' Visual UpTime traffic capture
   #. libpcap, tcpdump and various other tools using tcpdump's capture format
   #. snoop and atmsnoop output
 * 您大可利用那些不直接被Wireshark支持的设备截获数据并保存为Wireshark支持的文件格式，再间接使用。

1.14 Wireshark支持Windows Vista和Windows Server 2008吗？
  * 支持，但请注意，作为普通用户捕获数据时您必须确保npf.sys已被加载，即便Wireshark安装时已默认加载该项。
  * 作为管理员用户运行Wireshark时不存在以上问题。
  * 详情请参见 `CapturePrivileges`_ 。
  .. _CapturePrivileges: https://wiki.wireshark.org/CaptureSetup/CapturePrivileges#windows


2. 安装 Wireshark
-----------------------
2.1 我安装了Wireshark RPM（或其它包），为什么我只得到TShark而不是Wireshark？
  * 一些Linux发行版默认只安装了Wireshark的一部分，并不是所有发行版都默认安装GUI界面，事实上有的仅安装非GUI部分，例如TShark、editcap、dumpcap等等。如果你的系统是这样的情况，请尝试查找安装包 ``wireshark-gnome`` ``wireshark-gtk+``

3. 构建 Wireshark
---------------------
3.1 我已经安装libpcap，为什么配置脚本提示我找不到pcap.h或bpf.h？
  * libpcap官方发行版仅当您执行 ``make install`` 命令时才安装库文件libpcap.a。欲安装pcap.h和bpf.h请执行命令 ``make install-incl`` 
  * 如果您使用Debian或Redhat系统，请确保您已安装包 ``libpcap-dev`` 和 ``libpcap-devel``
  * 或者，pcap.h和bpf.h被安装在不当的位置，此时您应当“tweak aclocal.m4”（此处待译）

3.2 当我尝试从SVN仓库或SVN快照当中构建一份Wireshark时发生了错误，提示“dftest_DEPENDENCIES was already defined in condition TRUE”，我该怎么办？
  * 你可能正在使用automake1.5（使用命令 ``automake --version以检视版本信息`` ），该版本存在的已知BUG导致了该问题，请升级至automake1.6或以上版本。

3.3 当我构建Wireshark失败时，链接器消息的末尾发出了一连串“Output line too long”的提示，我该怎么办？
  * 这是您的 ``sed`` 程序不能处理超长行导致的错误。例如，在Solaris系统中， ``/usr/bin/sed`` 具有的行长限制过短导致了 ``libtool`` 运行失常； ``/usr/xpg4/bin/sed`` 则可以作为代替，正如你在GNU中的体验一样。
  * 以上，在Solaris中将 ``/usr/xpg4/bin`` 目录的命令搜索优先级提高至 ``/usr/bin`` 之前可以解决这个问题；类似地，您可以用同样的方法解决在其它平台遇到的该问题（您可能需要额外安装GNU程序 ``sed`` ）。

3.4 当我构建Wireshark失败时，链接器提示“plugin_list is undefined”，我该怎么办？
  * （此处待译）

3.5 当我在Windows构建Wireshark失败时， ``winsock.h`` 与 ``winsock2.h`` 发生冲突，我该怎么办？
  * （此处待译）

4. Starting Wireshark
---------------------
5. Crashes and other fatal errors
---------------------------------
6. Capturing packets
--------------------
7. Capturing packets on Windows
-------------------------------
8. Capturing packets on UN*Xes
------------------------------
9. Capturing packets on wireless LANs
-------------------------------------
10. Viewing traffic
-------------------
11. Filtering traffic
---------------------
