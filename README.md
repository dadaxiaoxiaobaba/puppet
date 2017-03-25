<font size=22>扯线木偶（puppet）</font>

Puppet是一套以门户网站实时行情为前锋，以同花顺交易客户端为得分后卫，以通达信历史数据为控球后卫，以自建策略为中锋的，完整的闭环实盘交易系统框架。

工作流程：手动登录客户端 --> 运行扯线木偶 --> 自动搜索已登录的客户端 --> 交易前的预备 --> 自动获取持仓数据 --> 查询预警名单 --> 客户端待命状态

推荐使用最新版的Anaconda3，或者Python 3.5+。

交易API
******************************************************************************************************************
'买入': buy(), '卖出': sell(), '撤单': cancel(), '打新': raffle()

'可用余额': balance, '持仓': position, '成交': deals, '可撤委托': cancelable, '新股': new, '帐号': account
******************************************************************************************************************

2017/3/10 更新至0.4.3，优化输出效果，更友好。

2017/3/10 更新至v0.4.2，raffle增加skip参数，跳过指定的市场新股。

2017/3/10 更新到v0.4.1，小幅修改，部分优化，默认改为单交易客户端模式。 

2017/3/9 v0.4版发布！增加一键打新(raffle)、查新股（new）功能。大幅度修改优化，强化拟人化操作逻辑。

2017/2/23 V0.3.5发布！小幅修改，改善操作流畅度。

2017/2/22 v0.3发布！优化模拟人手交易的流程。

2017/2/21 v0.2.5发布！增加撤单（指定股票代码）功能。

2017/2/14 v0.2版发布！提供后台获取持仓数据。鸣谢网友liuyukuan博文中提供的AHK代码“SendMessage,0x111,57634,0,CVirtualGridCtrl2,同花顺”。

Windows下不需要安装、配置。

Linux下需要安装最新版本的Wine，环境设为Windows 7，先安装同花顺交易客户端，能正常使用之后再安装Python for Windows。启动wineconsole，pip install pyperclip，之后就可以正常使用了。

1、支持同花顺的“所有”交易客户端：官方统一版或老版、券商定制版（银河、国泰君安、华泰、广发、东方财富等）。

2、支持多种交易模式：同一券商多个账户、多个券商多个账户同时登录一个（或多个）交易端，并且同时进行交易。

3、目前仅支持多个不同的交易客户端登录后同时交易，暂时不支持一个交易客户端多个账户登录后同时交易。
