# ChatGPT
custom request chat example with https://chat.openai.com


### Python3

打开 `ChatGPT.py` 文件：

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

### Swift

使用 `ChatGPT.swift` 文件：

```swift
let sessionToken = "这里填写 session token！！！"

Task {
	let bot = Chatbot(sessionToken: sessionToken)
	// 你的问题： 
	let prompt = "How to learn Swift"
	prompt = "How to learn Swift"
	print(prompt)
	let content = await bot.getChatResponse(prompt: prompt)
	print("回答：\(content)")
}

```


### 代码参考
- [A-kirami/nonebot-plugin-chatgpt/chatgpt.py](https://github.com/A-kirami/nonebot-plugin-chatgpt/blob/master/nonebot_plugin_chatgpt/chatgpt.py)
