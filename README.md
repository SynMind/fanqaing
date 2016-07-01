
![Chinese Wikipedia Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/Wikipedia-logo-v2-zh-hans.svg/209px-Wikipedia-logo-v2-zh-hans.svg.png)

本文将介绍维基百科在中国大陆的访问状况和在中国访问维基百科的方法。

**本文更新于 2016 年 7 月。当您阅读到这篇文章时可能情况发生了变化。**

**如果您有任何疑问，或者对本教程中的某些内容有质疑，请前往[此处](https://github.com/techyanWP/zh-Wikipedia-Accessing-Guide/issues)递交 issues 。**

# 当前封锁状态
目前，维基百科除中文外所有语言版本在中国大陆均可访问。其他维基百科姊妹项目、维基百科存储图片的网站也可访问。在中国的部分地区，可能会出现能够访问中文维基的情况。但是这通常只是区域性、间歇性的。

因此，当您访问中文维基百科 https://zh.wikipedia.org 时打不开是正常的，其他语言如 https://en.wikipedia.org 是应该能够打开的。如果您打不开 https://en.wikipedia.org ，那么这很有可能是您所使用的宽带出现问题。请参见常见问题解答的第五条。

中文维基百科受到来自中国政府的网站审查机制的干扰而无法访问。也就是常说的“被墙了”、“被屏蔽了”。这套审查机制被称作“防火长城（ Great Firewall ）”，通常简称 GFW 。包括中文维基百科在内的大量外国站点在中国无法访问都因为防火长城的屏蔽。您需要进行一些技术处理以跨过防火长城的干扰，也就是“翻墙”。

# 常见问题解答
### Q：为什么维基百科会被屏蔽？
A：维基百科内包含了一些被中国政府认为不符合有关法律的敏感条目。如六四事件、天安门自焚事件等。维基百科不接受来自政府的审查，因此中国政府将中文维基百科封锁。

### Q：为什么其他语言的维基百科未受干扰？
A：防火长城的审查机制是不透明的。它并不会对外公开自己屏蔽网站的理由。因此只能通过防火长城平时运作的特点来推断。这可能是因为防火长城在面对使用外语的网站时往往会放宽审查。如 BBC 、 CNN 、纽约时报的中文网站均被封锁，但是同样也会包含被中国政府认为是敏感内容的对应的英文网站却能够正常访问。

### Q：为什么我实际遇到的封锁情况与前文所说的不一致？
A：受防火长城屏蔽网站原理的限制，在中国的部分地方出现短时间能够访问中文维基百科的情况是正常的。如果您能够长时间稳定地访问中文维基百科，这也只是您的个案。

### Q：翻墙犯法吗？
A：不犯法。

### Q：我使用的通信运营商会对翻墙造成影响吗？
A：不同网络环境（如固定宽带、移动数据等）都会对翻墙的速度、稳定性甚至是能否连接上翻墙服务器都会或多或少地造成影响。一些翻墙软件在一种网络环境下能使用、换另一种网络环境就不能使用也是很常见的情况。如果您遇到了翻墙服务不能连接的情况，请您换用其他网络多试几次。使用中国联通和中国电信的网络通常可以获得较好的翻墙体验；使用中国移动的固定宽带、长城宽带、畅联宽带、方正宽带、宽带通、广电宽带等较廉价的二级宽带运营商可能会导致翻墙服务缓慢、间歇性中断甚至无法连接。

----
下文将介绍访问维基百科的几种途径。

# 我应该使用哪种方法？
本文介绍了三种访问中文维基百科的方法。您可以根据下面的描述选择最适合您的一种。建议您在做出决定之前完整地阅读本教程的所有内容，以便您均衡考虑各种方法的优缺点。

“反向代理”通常用于设备没有安装翻墙工具、没有对翻墙做出配置的情况下临时使用，或者只偶尔阅读而不想编辑。反向代理通常不够稳定，并且会经常被防火长城屏蔽。您可以参考下面“反向代理”小节中的缺点。

使用“免费翻墙代理”后，您不但可以自由地访问中文维基百科，还能访问 Google 、 YouTube 、 Twitter 、 Facebook 等其他被防火长城屏蔽的网站。但是当您编辑维基百科时可能会遇到一些障碍。

“修改 hosts 文件”适合想长期稳定访问维基百科，对速度要求不高，对除了维基百科外其他被屏蔽网站不感兴趣，需要编辑维基百科的用户。但是修改 hosts 文件需要一定的动手能力，并且有可能会失败。

----
# 反向代理
## 原理
反向代理是一种主动突破网络审查的方法。由于中文维基百科的官方站点被屏蔽，反向代理则通过建立与维基百科内容一样的网站、并向官方站点实时地获取内容的方式来突破审查。使用这种方式不需要对电脑做出任何特殊的配置处理、也不需要安装软件。但是反向代理也有很明显的缺点，因此不建议使用。通常只有在不便于使用后两种方法的情况下再使用。

### 缺点
* 从技术上，反向代理网站的经营者可以看到您试图访问的内容。因此如果您使用了不安全的反向代理网站，如中国政府为控制翻墙流量故意设置的“钓鱼”代理（这种钓鱼代理被称作“蜜罐”），那么您的信息将会被完全泄露。
* 反向代理的服务器通常也位于中国国外。因此，反向代理本身也有被屏蔽的风险。防火长城在发现反向代理后往往会在第一时间屏蔽，通常同一个反向代理无法长期使用。
* 使用反向代理通常不能编辑维基百科，只能阅读。

## 使用方法
非常简单，直接访问下列网站即可：

* [https://w1.bypassgfw.xyz/wiki/Wikipedia:%E9%A6%96%E9%A1%B5]()

----

# 免费翻墙代理
## 原理
使用翻墙代理（如 VPN 、 Shadowsocks 等）时，您的电脑会首先连接到一台位于中国国外、但是没有被屏蔽的服务器，再经由这个服务器中转您与被屏蔽网站之间传输的数据。

通常提到的 VPN 就是利用了上面介绍的原理。翻墙代理有免费的，也有付费的。下面介绍一个免费代理的用法。

## 首先您需要...
如果您准备使用 macOS 、 Andorid （安卓）、 iOS 设备翻墙，那么您可以跳过这一段。但是如果使用 Windows ，您就需要按照这一段提前准备好您的电脑以备继续操作。当然，您就算不进行本段提到的操作也有可能会成功。

### 停止使用中国浏览器和安全软件
您需要在首次翻墙之前关掉电脑上几乎一切中国软件。如 360 安全卫士、 360 杀毒、金山毒霸等。有证据显示，这些安全软件会对翻墙工具造成干扰，并且有可能会将翻墙者的信息发送出去，而 360 可能参与了防火长城这个项目本身。建议您使用 Firefox （火狐）、 Chrome 作为您翻墙时使用的浏览器。360 安全浏览器、猎豹浏览器等也有可能会阻止您翻墙。除此之外，在翻墙软件对操作系统内部的一些设置做出必要的修改时，安全软件也有可能会拦截他们、甚至将他们误报成病毒。

建议您使用外国杀毒软件（如 [avast!](https://avast.com/) 等）替代中国杀毒软件。首次翻墙时应该关掉所有的中国软件，甚至包括腾讯 QQ 等。待翻墙成功后再一一打开，这样可以排除那些对翻墙有干扰的软件。

建议您[在此](https://www.mozilla.org/zh-CN/firefox/new/?utm_source=firefox-com&utm_medium=referral)下载 Firefox 浏览器。

### 翻墙软件会对我的电脑造成伤害吗？
不会。最起码本文介绍的不会。本文介绍的翻墙工具“ Lantern ”是一个开放源代码的软件。它的源代码完全开放、供别人检阅。一旦其中包含了威胁您电脑的代码，也会被其他人很快发现。

## 使用方法
请您按照您需要翻墙的设备选择合适的教程。

### Microsoft Windows
#### 下载
首先从下面的地址下载翻墙工具“ Lantern ”。**请不要使用迅雷等工具下载！尽可能使用 Internet Explorer 及其他非中国浏览器自带的下载功能！**

* [下载地址](https://raw.githubusercontent.com/getlantern/lantern-binaries/master/lantern-installer.exe)

如果上面的地址失效，请到[此处](https://github.com/techyanWP/zh-Wikipedia-Accessing-Guide/issues)递交 issues 。

#### 安装及使用
Lantern 在 Windows 上的安装非常简单。通常直接双击下载下来的安装包， Lantern 就会自动进行安装。

安装过后， Lantern 会自动弹出一个网页，如下图所示。通常如果您看到了这个网页，就说明 Lantern 已经安装成功。这时您可以尝试访问中文维基百科 https://zh.wikipedia.org/ 。而与中文维基百科一同屏蔽的其他网站（如 YouTube 、 Twitter等）此时也可以正常访问。

![](https://ooo.0o0.ooo/2016/07/01/577669b0b139c.png)

通常情况下， Lantern 会自动识别需要代理的网站。换句话说，被屏蔽的网站会自动使用代理；而未屏蔽的网站则直接连接。如果您需要通过代理连接所有需要连接的网站，您可以点击网页右下角的小齿轮，勾选“代理全部流量”。

#### 常见故障
如果您成功安装，并出现如上图所示的网页，但是仍然无法访问中文维基百科，那么您可以尝试访问其他被屏蔽的网站。如果这些网站都无法访问，请稍等一段时间重试。若仍无法访问，请尝试更换其他浏览器、重新启动您的电脑、重新安装 Lantern 。

### Android （安卓）
#### 下载
首先从下面的地址下载翻墙工具“ Lantern ”。您可以选择先下载到计算机上再拷贝到 Android 设备上，或者直接将链接发到手机上通过手机下载。**请使用系统自带的浏览器下载，不要使用 UC 等其他中国浏览器！要求 Android 版本在 4.1 及以上。**

* [下载地址](https://raw.githubusercontent.com/getlantern/lantern-binaries/master/lantern-installer.apk)

如果上面的地址失效，请到[此处](https://github.com/techyanWP/zh-Wikipedia-Accessing-Guide/issues)递交 issues 。

#### 安装及使用
其安装与大部分 Android 软件安装一样。您第一次打开 Lantern 的时候，屏幕上会出现一个大开关。直接将这个开关由 off 拨到 on 的位置，您的设备就可以访问维基百科了。在第一次启用 Lantern 的时候，您的设备可能提示有软件要开启 VPN 服务。请您允许这项请求。当您不需要翻墙时，直接将开关拨到 off 即可。

#### 常见故障
如果将开关拨到 on 后仍无法访问维基百科，那么您可以尝试访问其他被屏蔽的网站。如果这些网站都无法访问，请关掉您手机上所有的安全防护软件重试。您也可以尝试将手机连接到不同的 Wi-Fi 热点或者使用移动数据、使用您朋友的 Android 设备重试。

## 我为何无法编辑维基百科？
您可能会在使用 Lantern 翻墙后发现若要编辑维基百科时出现如上图所示的提示。这是因为维基百科不允许使用开放代理进行编辑。这类翻墙软件就属于开放代理。维基百科作为人人可编辑的百科全书，自然会招来很多破坏者。这些破坏者经常使用开放代理编辑，维基百科为避免这类情况的发生，当遇到开放代理时通常会大规模封禁。

为方便编者，维基百科有一项叫 IP 封禁例外权的权限。拥有这项权限的用户可以绕过维基百科对于某段 IP 的封禁而继续编辑。但是，如果您使用有 IP 封禁例外权的账户做出破坏维基百科的编辑，您的账户可能就会因此被维基百科封禁。

想要申请 IP 封禁例外权非常简单。只需要向 unblock-zh/at/lists.wikimedia.org 发送邮件，注明您使用的账户名即可。如果您收 IP 封禁的影响，无法创建账户，请在邮件中告知您想要创建一个账户，管理员会将创建好的账户信息发送给您。

您可以参考[维基百科上有关 IP 封禁例外权的信息](https://zh.wikipedia.org/wiki/Wikipedia:IP%E5%B0%81%E7%A6%81%E4%BE%8B%E5%A4%96)。通过下文将提到的修改 hosts 文件的方式翻墙通常不会受到上文提到的封禁的影响。

----
# 修改 hosts 文件
## 原理
防火长城使用了一种称作“ DNS 污染”的方式屏蔽中文维基百科。 DNS 污染会干扰维基百科域名的 DNS 查询结果，电脑会试图访问错误的 IP 地址从而达到屏蔽网站的目的。对于这种屏蔽方式，可以通过修改 hosts 文件的方式解决。 hosts 文件存储于电脑本地，用户可以通过修改 hosts 文件来纠正错误的 DNS 解析。

## 首先您需要...
### Q：修改 hosts 文件会对我的电脑造成伤害吗？
A：使用来源可靠的 hosts 文件不会对电脑造成伤害。

### 关闭电脑上所有安全软件
因为一些病毒会通过修改 hosts 文件的方式破坏电脑，所以修改 hosts 文件可能会触发一些安全软件的警告——无论安全软件是中国的还是外国的。建议您在完成修改操作后立刻打开安全软件，以防病毒趁虚而入。

### 使用干净的浏览器
一些安全软件（如 360 安全卫士）会让您的电脑使用由该公司自己提供的 DNS 服务，并可能在浏览器上检测 DNS 查询的结果。请不要使用 360 安全浏览器等浏览器，也尽可能不要在安装了 360 等提供的安全防护插件的浏览器上进行操作。建议您使用前文提到的FireFox （火狐）、 Chrome 作为您的浏览器。

## 对于 Microsoft Windows 的修改教程
截图使用 Windows 10 做示范。注意下方教程中`使用灰色框的文字`，这些文字通常表示一段需要您复制的内容、文件或选项的名字等。

打开您电脑上的 Windows 资源管理器（即“我的电脑”、“计算机”）。打开文件夹 `%SystemRoot%\System32\drivers\etc\` 。直接将前面灰色方框里面的字符复制到 Windows 资源管理器中，如图所示。按下回车，系统会自动为您转到 hosts 文件所在的文件夹中。

![Screenshot of Lantern for Windows After Launched](https://ooo.0o0.ooo/2016/07/01/57766b205aa11.png)
![hosts File in Windows 10](https://ooo.0o0.ooo/2016/07/01/57766b1fb9995.png)

<font size=1>
注：在大多数电脑中， `%SystemRoot%` 指的是 `C:\Windows` 。也就是说，对于大部分电脑， hosts 文件实际存于 `C:\Windows\System32\drivers\etc\` 中。 Windows 会自动将 `%systemroot` 转换成 `C:\Windows` 。
</font>

在文件夹中，您将能看到一个名叫 `hosts` 的文件。双击打开这个文件。如果系统询问应该使用哪个程序打开，请选择使用`记事本`。打开 hosts 文件后，您需要在 hosts 文件的最后面添加这些内容（您可以与上面已有的内容之间空出几行）。

	198.35.26.96 zh.wikipedia.org
	198.35.26.96 zh.m.wikipedia.org
	

![A host File Sample](https://ooo.0o0.ooo/2016/07/01/57766c4375051.png)

保存文件。建议您保存之后重新打开一次文件，确认添加进的内容已经成功保存。如果没有成功保存，请重试之前的操作。如果仍然无法保存，请参考下面的小节。重新启动电脑。这时您应该能够正常访问中文维基百科了。

上图展示的是一个 hosts 文件样本。您电脑上保存的 hosts 文件可能与图片上显示的不同。上图中的 hosts 文件是没有修改过的。

### 您可能会遇到的特殊情况
修改 hosts 文件可能会遇到各种各样的特殊情况。上方介绍的只是在没有特殊情况下最理想的一种。如果您遇到了上方教程中没有提到的提示、警告，请参照下面的方法解决。如果下面的方法不适用于您遇到的情况，请尝试使用反向代理或者免费翻墙代理来访问中文维基百科。

#### 提示权限不足
如果系统仅仅非常简单的提示您权限不足，那么直接允许电脑保存即可。在一些情况下，您可能需要右键单击 `hosts` 这个文件，选择`属性`，确保`只读`前的复选框没有被勾选。

#### 保存时记事本弹出另存为的窗口、或不让保存;
#### 无论怎么修改文件也不能把新增加的内容添加进去，重新打开后发现保存失败
如果出现了这样的提示，请直接放弃编辑原文件。您可以将 `hosts` 这个文件复制一份到桌面上，编辑您在桌面上复制的文件，添加上方的两行内容，保存文件。删除在系统文件夹下的那个 `hosts` 文件，将修改过的复制到原来的文件夹里。期间系统可能会提示权限不足，请允许电脑进行操作。

复制后，请复查您修改过的 `hosts` 文件没有扩展名。如果有扩展名，请将它删掉。

----
# 著作权
本文根据 知识共享-署名-相同方式共享-4.0 协议发布。您可以[至此](https://creativecommons.org/licenses/by-sa/4.0/)获取本协议的原文件。在文中也有受到版权保护的软件截图和 Logo 。这些软件截图不遵守知识共享协议。本文作者为 闫恩铭 / techyan 。请见 [https://techyan.me/]() 。
