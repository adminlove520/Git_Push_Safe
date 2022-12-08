# git_push_safe


## 实时监控github上新增的cve和安全工具更新，多渠道推送通知

每3分钟检测一次github是否有新的cve漏洞提交或者安全工具更新记录，若有则通过配置的渠道通知用户

时间间隔修改在 467 行


```bash
pip3 install -r requirements.txt
python3 github_cve_monitor - release.py 		
```

# 使用帮助

`tools_list.yaml` 监控的工具列表，新添加按照已有的格式写

`config.yaml` 推送token 设置
若需要推送到tgbot
```bash
pip install python-telegram-bot		
```
并在config.yaml中配置tgbot的token等信息,enable设置为 1表示推送

# TODO-List
 通过github actions实现
 优化推送内容及格式





