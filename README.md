

这部分是一个简单的优化火狐隐私的方法，一定程度的添加了广告的跟踪难度

这部分是优化火狐浏览器的部分，以加固安全和隐私。要知道火狐默认的配置不是最安全和隐私的配置。需要改良一下。记得去官网下载正版，另外建议使用延长更新版本，同时使用英语的版本哦。

network.trr.uri设置成https://1.1.1.1/dns-query

或者其他安全dns

network.trr.mode设置为3表示强制使用，2表示优先使用。

在搜索框中输入 privacy.resistFingerprinting ，双击将值改为 true 。

这将使 Firefox 防范指纹跟踪，并修改请求头为默认头。

在搜索框中输入 privacy.firstparty.isolate ，双击将值改为 true 。

这将使 Firefox 的 First Party Isolation 功能启用，

使网站无法通过 Cookie 交换来跨越不同的域名共享数据。

在搜索框中输入 privacy.trackingprotection.fingerprinting.enabled ，

双击将值改为 true 。这将使 Firefox 的 Tracking Protection

功能阻止更多的指纹跟踪器。

在搜索框中输入 privacy.resistFingerprinting.letterboxing ，双击将值改为 true 。

这将使 Firefox 通过将屏幕的内容放置在一定的“黑色条纹”中，防范屏幕尺寸的测量。

plugin.sessionPermission.enabled：如果设置为false，则禁用了插件访问控制，默认为true。

plugin.sessionPermission.scope：指定了插件访问控制的范围，可以是url、domain或global。如果未设置，则默认为url。

privacy.resistFingerprinting: 开启指纹防御。这会禁用某些网站在 Firefox 中收集您的唯一标识符，从而提高您的匿名性。

privacy.firstparty.isolate: 启用第一方隔离。这会限制同一站点的不同页面使用不同的隔离上下文，从而减少跨站点攻击的风险。

privacy.trackingprotection.fingerprinting.enabled: 启用防指纹跟踪。这会防止网站收集有关您系统硬件和软件的详细信息，从而降低您的唯一标识的风险。

privacy.trackingprotection.enabled: 启用跟踪保护。这会防止网站追踪您的浏览历史和行为。

network.cookie.cookieBehavior: 设置 Cookie 的处理方式。推荐将其设置为 4，即拒绝第三方 Cookie。

browser.send_pings: 禁用 ping。这会防止浏览器在页面加载时向其他网站发送 ping 信号。

browser.sessionstore.privacy_level: 将会话恢复的隐私级别设置为严格。这会防止 Firefox 从上次会话中恢复网站。

network.http.referer.XOriginPolicy: 将 referrer 策略设置为相同的来源。这会限制传递 referrer 数据的来源。

network.dns.disablePrefetch: 禁用 DNS 预获取。这可以防止 Firefox 在您访问之前预加载其他网站的 DNS 信息。

dom.event.clipboardevents.enabled: 禁用剪贴板事件。这可以防止网站通过剪贴板事件来追踪您的浏览历史。

browser.urlbar.speculativeConnect.enabled: 禁用预连接。这会防止 Firefox 在您访问之前建立与其他网站的连接。

media.peerconnection.enabled: 禁用 WebRTC。这可以防止网站通过 WebRTC 连接来泄露您的 IP 地址。

browser.tabs.remote.autostart，然后将其值修改为“true”，这样就开启了多进程模式。

browser.tabs.remote.force-enable，然后将其值修改为“true”，这样就强制开启多进程模式。

toolkit.telemetry.enabled

将该选项的值从默认值“true”更改为“false”，这将禁用Firefox发送遥测数据到Mozilla服务器。

输入“browser.safebrowsing.enabled”。

将该选项的值从默认值“true”更改为“false”，这将禁用Firefox的安全浏览服务

在about:config页面的搜索栏中输入“app.normandy.enabled”。

将该选项的值从默认值“true”更改为“false”，这将禁用Firefox的Normandy服务

禁用第三方Cookie 将network.cookie.cookieBehavior的值设置为2，这将禁用第三方Cookie。

禁用WebRTC 将media.peerconnection.enabled的值设置为false，这将禁用WebRTC功能。

搜索建议 将browser.search.suggest.enabled的值设置为false，这将关闭搜索建议。

安全搜索 将browser.safebrowsing.malware.enabled和browser.safebrowsing.phishing.enabled的值都设置为false，这将关闭安全搜索功能。

禁用缓存 将browser.cache.disk.enable、browser.cache.memory.enable和browser.cache.offline.enable的值都设置为false，这将禁用浏览器缓存。

禁用Telemetry 将toolkit.telemetry.enabled和toolkit.telemetry.server的值都设置为false，这将禁用Telemetry数据收集功能。

用户代理 将general.useragent.override的值设置为一个常见的用户代理字符串，这有助于防止被追踪。

禁用插件 将plugin.state.flash和plugin.state.java的值都设置为0，这将禁用Flash和Java插件。

禁用自动填表功能 将browser.formfill.enable的值设置为false，这将禁用自动填表功能。

禁用推荐扩展功能 将extensions.htmlaboutaddons.recommendations.enabled的值设置为false，这将禁用在插件/扩展页面中显示推荐扩展功能。

禁用密码管理器自动填写功能 将signon.autofillForms和signon.rememberSignons的值都设置为false，这将禁用密码管理器自动填写功能。

禁用WebGL 将webgl.disabled的值设置为true，这将禁用WebGL功能。

禁用内嵌字体 将gfx.downloadable_fonts.enabled的值设置为false，这将禁用浏览器下载和使用网站提供的字体文件。

禁用网络预测服务 将network.predictor.enabled和network.predictor.enable-prefetch的值都设置为false，这将禁用网络预测服务。

禁用HTTP缓存 将browser.cache.check_doc_frequency的值设置为1，这将禁用HTTP缓存。

强制HTTP连接 将security.mixed_content.block_active_content和security.mixed_content.block_display_content的值都设置为true，这将强制所有不安全的HTTP连接使用HTTPS连接。

禁用网络错误收集 将browser.chrome.errorReporter.enabled和browser.chrome.errorReporter.submitUrl的值都设置为false，这将禁用网络错误收集功能。

禁用电池状态API 将dom.battery.enabled的值设置为false，这将禁用网站获取用户设备电池状态的能力。

禁用浏览历史记录 将places.history.enabled的值设置为false，这将禁用Firefox保存用户的浏览历史记录。

禁用连通性检测服务 将network.connectivity-service.enabled的值设置为false，这将禁用Firefox自动检测网络连接状态的能力。

禁用Geo定位 将geo.enabled的值设置为false，这将禁用Firefox使用用户IP地址或其他方式获取用户地理位置信息。

禁用存储访问API 将dom.storage_access.enabled的值设置为false，这将禁用Storage Access API，防止跨站点网站共享数据。

messaging-system.rsexperimentloader.enabled 改成false关闭实验与研究

app.normandy.optoutstudies.enabled false 这几个我不太清楚，但是因该设置成false

app.normandy.enabled false 这几个我不太清楚，但是因该设置成false，注意需要去设置冲关闭所有Firefox Data Collection and Use这个选项

记得关闭设置中的那几个检测安全的，他们可能收集信息检测安全。

browser.aboutHomeSnippets.updateUrl 字符串设置成空

browser.search.geoip.url 空

browser.startup.homepage_override.mstone ignore

禁用HTTP Referer头部 将network.http.sendRefererHeader的值设置为0，这将禁用HTTP Referer头部发送。

设置DNS over HTTPS (DoH) 将network.trr.mode的值设置为2，并将network.trr.uri的值设置为一个可信任的DoH服务器地址，这将启用DNS over HTTPS并加密所有DNS查询。

禁用Web蓝牙API 将dom.bluetooth.enabled的值设置为false，这将禁用Web蓝牙API。

禁止媒体自动播放 将media.autoplay.default的值设置为5，这将禁止所有媒体自动播放。

禁用存储日志文件 将browser.privatebrowsing.autostart的值设置为true，这将自动启动隐私浏览模式并禁用日志记录。

禁用Firefox数据收集功能 将datareporting.healthreport.uploadEnabled、toolkit.telemetry.unified的值都设置为false，这将禁用Firefox数据收集功能。

禁用用户数据收集：搜索 datareporting.policy.dataSubmissionEnabled 和 datareporting.policy.firstRunURL，并将它们的值都设为 false

禁用网络预测服务 将network.predictor.enabled和network.predictor.enable-prefetch的值都设置为false，这将禁用网络预测服务。

禁止定位共享 将geo.wifi.uri的值设置为一个无效的地址，这将禁止Firefox使用Wi-Fi数据共享用户位置信息。

禁用缓存 将browser.cache.disk.enable、browser.cache.memory.enable和browser.cache.offline.enable的值都设置为false，这将禁用Firefox浏览器缓存。

关闭TLS版本 将security.tls.version.min的值设置为3，这将关闭TLS 1.0和1.1版本，只允许TLS 1.2及以上版本。

禁止搜索引擎预加载 将browser.search.separatePrivateDefault.ui.enabled的值设置为true，这将禁止在隐私浏览模式下预加载搜索引擎。

禁止cookie同步 将services.sync.engine.prefs.modified的值设置为false，这将禁止在Firefox Sync中同步cookie设置。

禁用媒体指纹 将media.eme.enabled、media.gmp-widevinecdm.enabled和media.navigator.enabled的值都设置为false，这将禁用数字版权管理、Widevine CDM和WebRTC功能。

启用 Do Not Track：搜索 privacy.donottrackheader.enabled 并将其值设为 true

禁用Canvas指纹识别 将privacy.resistFingerprinting.block_mozAddonManager和privacy.resistFingerprinting.block_mozAddonManagerMethod的值都设置为true，这将禁用Canvas指纹识别。

network.captive-portal-service.enabled false

禁用缓存加速 将browser.cache.use_new_backend的值设置为0，这将禁用缓存加速功能。

禁用Flash插件 将plugin.state.flash的值设置为0，这将禁用Flash插件。

禁用Java插件 将plugin.state.java的值设置为0，这将禁用Java插件。

禁用自动更新 将app.update.auto、app.update.enabled、app.update.service.enabled和app.update.staging.enabled的值都设置为false，这将禁用自动更新功能。

禁用字体指纹识别 将browser.display.use_document_fonts的值设置为0，这将禁用网页中使用的特定字体，从而防止字体指纹识别。

增加DNS缓存时间 将network.dnsCacheExpiration和network.dnsCacheEntries的值都增加到较高的数字，这将增加DNS缓存的时间和大小。

禁用Captive Portal检测 将captivedetect.canonicalURL的值设置为一个无效的地址，如http://detectportal.firefox.com/success.txt，这将禁用Captive Portal检测。

禁止域名预读取 将network.dns.disablePrefetch和network.dns.disablePrefetchFromHTTPS的值都设置为true，这将禁止Firefox自动预读其他网站的DNS信息。

禁止HSTS缓存 将security.mixed_content.use_hsts、security.mixed_content.block_active_content和security.mixed_content.block_display_content的值都设置为true，这将禁止Firefox缓存HSTS设置。

禁止拼写检查 将layout.spellcheckDefault的值设置为0，这将禁止Firefox自动进行拼写检查。

禁用Referrer发送 将network.http.sendRefererHeader的值设置为0，这将禁用浏览器在访问其他网站时发送Referrer信息。

禁用字体下载 将browser.display.use_document_fonts的值设置为0，这将阻止Firefox下载并使用页面中嵌入的字体。

禁用弹出窗口 将dom.disable_open_during_load和dom.popup_allowed_events的值都设置为false，这将禁止浏览器在页面加载时自动打开弹出窗口。

禁用自动语言选择 将intl.accept_languages的值设置为一个常见的语言代码，如en-US，这将禁止自动选择语言。

permissions.default.image 3 2表示禁止图片，1表示允许任何图片，3表示只允许来自这个服务器的图片

network.dns.echconfig.enabled network.dns.use_https_rr_as_altsvc network.security.esni.enabled 这三个设置从True network.connectivity-service.enabled false

dom.battery.enabled：将其设置为False，以禁用电池状态API。

bluetooth.enabled：将其设置为False，以禁用蓝牙API。

device.sensors.enabled：将其设置为False，以禁用所有传感器API（例如加速度计、陀螺仪等）。

media.navigator.enabled：将其设置为False，以禁用媒体设备访问。

media.webspeech.synth.enabled：将其设置为False，以禁用Web Speech API中的语音合成功能。

media.webspeech.recognition.enable：将其设置为False，以禁用Web Speech API中的语音识别功能。

network.cookie.cookieBehavior：将其设置为1，以仅允许从当前网站读取Cookie。

privacy.firstparty.isolate：将其设置为True，以隔离不同站点之间的cookie。

增加HTTP连接超时时间 将network.http.connection-timeout的值增加到较高的数字，这将增加HTTP连接的超时时间。

禁用CSS样式表下载 将permissions.default.stylesheet的值设置为2，这将阻止Firefox下载页面的CSS样式表。

browser.chrome.site_icons 设置成false这回禁止favicon小图标，这个小图标可能会因为缓存，而放入微笑的跟踪像素。这个小图标纯属好看没有P用。

在搜索框中输入 browser.cache.disk.enable，双击该选项将其值从 true 修改为 false。

在搜索框中输入 browser.cache.memory.enable，双击该选项将其值从 false 修改为 true Firefox 将不再将缓存写入硬盘，而是将其存储在内存中。

对 SSL/TLS 连接进行更严格的验证：搜索 security.tls.version.min 并将其值设为 3，搜索 security.tls.version.fallback-limit 并将其值设为 0，搜索 security.tls.enable_0rtt_data 并将其值设为 false。

禁用网络缓存：搜索 browser.cache.disk.enable、browser.cache.memory.enable 和 browser.cache.offline.enable，并将它们的值都设为 false。这可以防止 Firefox 缓存网页内容。

另外肯定还有很多需要改的，希望大佬看到有需要改的留言补充下。谢谢大家。

browser.cache.offline.enable”并将其值更改为“false”。这将禁用Firefox的离线缓存，确保Firefox不会在硬盘上存储任何数据。

dom.event.mousemove false禁止跟踪鼠标,很多考试网站会跟踪鼠标的位置，防止作弊等。

dom.event.clipboardevents.enabled false禁止跟踪剪切板

这将减少对硬盘的写入，并提高系统的响应速度。

需要使用一个靠谱的"VPN"，这个VPN必须能够过滤掉火狐的流量，不能让火狐的服务器收集到你的任何信息，建议去把所有火狐的域名都拦截掉。避免它与它的服务器通信。

同时使用Ubuntu或者windows的防火墙实现kill -switch

具体方法是

sudo ufw default deny incoming

sudo ufw default deny outgoing

允许从特定 IP 地址传入流量：

sudo ufw allow from {IP地址} to any

允许从本地网络传出流量：

sudo ufw allow out on {本地接口名称} to any

请注意，{IP地址} 和 {本地接口名称} 应替换为您要允许的 IP 地址和本地接口名称。

如果您希望撤销这些规则，可以使用以下命令：

sudo ufw delete allow from {IP地址} to any

sudo ufw delete allow out on {本地接口名称} to any

注意这个可以ufw reset来重置的，放心设置即可没问题的。

总的来说，这样设置一定程度的增加了火狐的隐私性，避免了很多广告推送。但是这仅仅用于隐私用途，防止广告商跟踪而已，无法用于某特殊用途(黑客活动等)，请遵守法律。

你也可以禁止JavaScript，这样更安全，但是网站会具难用。另外可以去参考 某葱 浏览器他们的优化和特殊的设置。或者librewolf的浏览器他们的设置。

某种程度上edge、谷歌浏览器等也是很好用的，速度很快，内存占用更小，方便调试等。可以根据自己的需要平衡隐私和方便。

Canvas Fingerprint Defender的插件 建议安装一下

WPD - Windows Privacy Dashboard (https://wpd.app/) Blackbird (https://www.getblackbird.net/) - 这是另一个针对Windows 7/8/10的免费开源工具，用于禁用各种数据收集和跟踪功能。 O&O ShutUp10 (https://www.oo-software.com/en/shutup10) - 这是一个专门为Windows 10设计的免费工具

一味的追求隐私和安全而忽略方便是非常愚蠢的。
