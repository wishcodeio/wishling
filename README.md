# 說明指南

# 1. 解壓縮並進入目錄
unzip wishling_bot.zip && cd wishling_bot

# 2. 建立 Conda 環境和退出環境
conda create -n wishling_bot python=3.10 -y
conda activate wishling_bot
conda deactivate

# 3. 安裝依賴
pip install -r requirements.txt

# 4. 編輯 config/settings.py，加入你的 TELEGRAM_TOKEN

# 5. 啟動
bash run.sh

✅ 清理完成後，重新啟動流程
```
conda create -n wishling_bot python=3.10 -y
conda activate wishling_bot
cd wishling_bot
pip install -r requirements.txt
python main.py
```

```
wishling_bot_v1/
├── main.py                         # 主入口（只有 start / menu / intent）
├── config/
│   └── settings.py                 # 放 TELEGRAM_TOKEN
├── handlers/
│   ├── activate.py
│   ├── wishdeck.py
│   ├── cards.py
│   ├── dream.py
│   ├── core.py
│   ├── log.py
│   ├── learn.py
│   ├── quiz.py
│   ├── chant.py
│   ├── start.py
│   ├── help.py
│   ├── menu.py
│   └── intent.py
├── keyboards/
│   └── reply_keyboards.py
├── requirements.txt               # 必要依賴：python-telegram-bot 等
├── run.sh                         # 一鍵啟動腳本（conda + 啟動）
```
