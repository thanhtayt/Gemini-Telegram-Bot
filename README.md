# Gemini_Telegram_Bot
一个使用 Gemini API 的 Telegram 机器人[English ducument](https://github.com/H-T-H/Gemini_Telegram_Bot/blob/main/README_en.md)
# Demo
[点这里](https://t.me/gemini_telegram_demo_bot)

# 如何安装
## (1) Linux系统
1. 安装依赖
```
pip install -r requirements.txt
```
2. 在[BotFather](https://t.me/BotFather)获取Telegram Bot API
3. 在[Google AI Studio](https://makersuite.google.com/app/apikey)获取Gemini API keys
4. 运行机器人，执行以下命令：
```
python main.py ${Telegram 机器人 API} ${Gemini API 密钥}
```
## (2)使用 Docker 部署
### 自行构建
1. 在[BotFather](https://t.me/BotFather)获取Telegram Bot API
2. 在[Google AI Studio](https://makersuite.google.com/app/apikey)获取Gemini API keys
3. 克隆项目
```
git clone https://github.com/H-T-H/Gemini-Telegram-Bot.git
```
4. 进入项目目录
```
cd Gemini-Telegram-Bot
```
5. 构建镜像
```
docker build -t gemini_tg_bot .
```
6. 运行镜像
```
docker run -d -e TELEGRAM_BOT_API_KEY={Telegram 机器人 API} -e GEMINI_API_KEYS={Gemini API 密钥} gemini_tg_bot
```
### 如果你不想自己构建
#### 1.在 x86 架构上
运行以下命令：
```
docker run -d -e TELEGRAM_BOT_API_KEY={Telegram 机器人 API} -e GEMINI_API_KEYS={Gemini API 密钥} qwqhthqwq/gemini_telegram_bot:latest
```
#### 2.在 arm 架构上
运行以下命令：
```
docker run -d -e TELEGRAM_BOT_API_KEY={Telegram 机器人 API} -e GEMINI_API_KEYS={Gemini API 密钥} qwqhthqwq/gemini_telegram_bot_arm:latest
```

# 使用方法
1. PM中直接发送你的问题
2. 群组中使用/gemini命令
3. 使用'/clear'命令可删除当前对话的历史记录

# 参考信息
1. [https://github.com/yihong0618/tg_bot_collections](https://github.com/yihong0618/tg_bot_collections)
2. [https://github.com/yym68686/md2tgmd/blob/main/src/md2tgmd.py](https://github.com/yym68686/md2tgmd/blob/main/src/md2tgmd.py)
