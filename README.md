# scripts
QX
首先打开设置，找到重写，然后选择规则资源，在其中添加规则（规则路径为 https://github.com/yangdaozhao/ylgy/blob/master/config.conf ，如果添加失败的话记得添加资源解析器：https://github.com/KOP-XIAO/QuantumultX/blob/master/Scripts/resource-parser.js ），规则名称随意，添加完成之后保存。
然后返回到设置界面，打开重写。
接着找到下方的 MitM，点击生成证书，接着点击配置证书，按照软件提示安装证书，信任证书。
完成之后回到设置界面打开 MitM
打开代理
打开羊了个羊，玩一把，你会发现第一关结束之后游戏并没有跳到第二关，不用管，接着玩一次第一关。
恭喜，你已经加入了羊群。
ShadowRocket
shadowsocket配置文件中打开https解密，生成一个新的ca证书，将证书安装进系统，然后去ios打开信任证书。
shadowsocket中配置->模块->新建模块，内容如下:
#!name=🍿️ ylgy
#!desc=羊了个羊
[Script]
Ylgy = type=http-response, pattern=^https?://cat-match.easygame2021.com/sheep/v1/game/map_info(.*)$, requires-body=1, max-size=0, script-path=https://raw.githubusercontent.com/yangdaozhao/ylgy/master/ylgy.js, argument=
[MITM]
hostname = *.easygame2021.com
Loon
