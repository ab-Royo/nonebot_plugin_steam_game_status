[![PyPi](https://img.shields.io/pypi/v/nonebot_plugin_steam_game_status.svg)](https://pypi.python.org/pypi/nonebot_plugin_steam_game_status)

# nonebot_plugin_steam_game_status
在群内播报steam游戏状态的Nonebot插件
==========

## 安装

```bash
# 使用pip安装，记得手动添加插件名到配置文件
pip install nonebot_plugin_steam_game_status

# 使用nb-cli安装
nb plugin install nonebot_plugin_steam_game_status

# 更新至最新版 
pip install nonebot_plugin_steam_game_status --upgrade
```

## 配置
### 获取steam_web_api_key

获取[steam_web_key](https://steamcommunity.com/dev/apikey)

配置文件内填写：
```bash
steam_web_key="your key"
```
### 获取Steam ID

    Steam 桌面网站或桌面客户端：点开右上角昵称下拉菜单，点击账户明细，即可看到Steam ID
    Steam 应用：点击右上角头像，点击账户明细，即可看到Steam ID

## 指令表

| 指令 | 需要@ | 范围 | 权限 | 说明 |
|:-----:|:----:|:----:|:----:|:----:|
| steam绑定/添加/.add | 否 | 群聊 | 群员 | 后加个人Steam ID |    
| steam解绑/删除/.del | 否 | 群聊 | 群员 | 后加个人Steam ID |   
| steam列表/绑定列表 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
| steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
| steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    

## 创意来源

群友的koishi bot的该效果插件

## 注意事项

1.也许不支持播报Linux Steam客户端游戏

2.不支持播报Steam隐身状态下进行的游戏

## 更新记录

2023.05.07

1.优化了日志输出，和部分代码

2.感谢 [050644zf](https://github.com/050644zf) 提供了更适合的steam id获取方式

3.关闭了证书验证，避免代理影响



2023.04.23

1.优化了监控代码，解决请求阻塞过久的问题

2.解决消息在多账号下无法发送的问题
