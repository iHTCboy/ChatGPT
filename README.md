# ChatGPT
custom request chat example with https://chat.openai.com


1、先安装依赖库

```bash
	pip3 install typing
	pip3 install requests
	pip3 install OpenAIAuth
```

2、获取 session_token
	
1. 登录 https://chat.openai.com/chat
2. 按 F12 打开控制台
3. 切换到 Application/应用 选项卡，找到 Cookies
4. 复制 __Secure-next-auth.session-token 的值，配置到 `SESSION_TOKEN` 即可

运行 ChatGPT.py：
```
python3 ChatGPT.py
```


代码参考：
https://github.com/A-kirami/nonebot-plugin-chatgpt/blob/master/nonebot_plugin_chatgpt/chatgpt.py
