浏览器插件 [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega "FelisCatus/SwitchyOmega") 的配置备份，支持三种情景模式，规则列表网址可自动更新。

| 情景模式 | 类型 | 说明 | 参考|
| - | - | - | - |
| *GFWed* | 代理服务器 | 该模式强制浏览器通过代理进行网络访问。<br> 需要根据所使用的代理软件填写相关参数。 | [FelisCatus/SwitchyOmega/wiki/GFWList](https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList "FelisCatus/SwitchyOmega/wiki/GFWList") |
| *白名单* | 自动切换模式 | 列表网址为中国网址。<br> 该模式避免通过代理访问相应网址。<br> 适用于访问网址以国外为主、国内为辅时。 | [entr0pia/SwitchyOmega-Whitelist](https://github.com/entr0pia/SwitchyOmega-Whitelist "entr0pia/SwitchyOmega-Whitelist")                |
| *黑名单* | 自动切换模式 | 列表网址为国外网址（GFW）。<br> 该模式允许通过代理访问相应网址。<br> 适用于访问网址以国内为主、国外为辅时。 | [FelisCatus/SwitchyOmega/wiki/GFWList](https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList "FelisCatus/SwitchyOmega/wiki/GFWList") |

# 使用方法

## 安装 SwitchyOmega

SwitchyOmega 插件适用于 Chromium 或基于 Chromium 的浏览器。可通过以下任一方式安装：

-   [Chrome Web Store](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif "Proxy SwitchyOmega - Chrome Web Store")

-   [Chrome扩展 - Crx搜搜](https://www.crxsoso.com/webstore/detail/padekgcemlokbadohgkifijomclgjgif "Proxy SwitchyOmega | Chrome扩展 - Crx搜搜")

-   [Github Releases](https://github.com/FelisCatus/SwitchyOmega/releases "Releases · FelisCatus/SwitchyOmega")

## 导入备份

打开 SwitchyOmega 选项，

![SwitchyOmegaBackup1](https://github.com/chugit/SwitchyOmegaBackup/assets/156684016/d1db76fd-6564-4b8d-b29d-fac904297092)

① 点击 "导入/导出"；

② "在线恢复"，输入以下链接后，点击 "恢复"。

```         
https://raw.githubusercontent.com/chugit/SwitchyOmegaBackup/main/OmegaOptions.bak
```

③（备选）若在线恢复不成功，可从 [github](https://github.com/chugit/SwitchyOmegaBackup/blob/main/OmegaOptions.bak) 或 [gitee](https://gitee.com/chugit2024/SwitchyOmegaBackup/raw/main/OmegaOptions.bak) 下载备份文件 OmegaOptions.bak，然后点击 "从备份文件恢复" 加载该文件。

## 修改 *GFWed* 参数

插件配置恢复后，首先应根据代理软件实际，修改情景模式 *GFWed* 的参数。

![SwitchyOmegaBackup2](https://github.com/chugit/SwitchyOmegaBackup/assets/156684016/671e4502-b934-49b1-83a6-91f838e408cc)

根据所使用的代理软件的参数和说明书，对 *GFWed* 情景模式进行修改，选择并设定与代理软件对应的 "代理协议"、"代理服务器" 和 "代理端口"。

此外，可在 "不代理的地址列表" 中指定该情景模式需要绕过的IP（即不通过该代理访问的网址）。本备份文件中的不代理地址（见截图）均为本地地址。

点击侧边栏的 "应用选项"，保存插件配置。

## 选择 *白名单* 或 *黑名单* 科学上网

完成上述配置后，即可选择基于规则的情景模式 *白名单* 或 *黑名单* 开启科学上网。

情景模式 *白名单* 和 *黑名单* 的参数默认设置如下，一般不需要修改。

![SwitchyOmegaBackup3](https://github.com/chugit/SwitchyOmegaBackup/assets/156684016/fafb44c3-8f89-4da3-a9ad-26403c75ea83)

![SwitchyOmegaBackup4](https://github.com/chugit/SwitchyOmegaBackup/assets/156684016/325795c0-0661-4bbe-a1e8-f1ccd1ce07a2)

-   *白名单* 的规则列表网址为中国网址，可避免通过代理访问这些网址，适合访问网址以国外为主、国内为辅时使用。

-   *黑名单* 的规则列表网址为国外网址（源自GFW），要求通过代理访问这些网址，适合访问网址以国内为主、国外为辅时使用。
