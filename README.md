# ربات خبریابی هوشمند استان فارس

## Fars Province Smart News Bot v1

ربات هوشمند جمع‌آوری اخبار استان فارس با هوش مصنوعی Gemini

### ویژگی‌ها
- 🔍 جستجوی خودکار در Google News (فارسی + انگلیسی)
- 🐦 جستجو در X/Twitter از طریق گوگل
- 🌐 منابع وب RSS
- 🤖 فیلتر هوشمند با Gemini AI
- 📝 بازنویسی با پروتکل مقاومت (دکمه اختیاری — صرفه‌جویی در هزینه)
- 🗄 حذف تکراری با SQLite

### Environment Variables
```
TELEGRAM_BOT_TOKEN=your_bot_token
PERSONAL_CHANNEL_ID=your_channel_id
ADMIN_CHAT_IDS=your_chat_id
GEMINI_API_KEY=your_gemini_key
DEFAULT_KEYWORDS=استان فارس,شیراز,...
DEFAULT_WEB_SOURCES=https://mojahedin.org/rss/
ENABLE_X_SEARCH=1
CHECK_INTERVAL=300
```

### Deploy on Render
1. Push to GitHub
2. Create Web Service on Render
3. Set environment variables
4. Start Command: `python main.py`
5. Visit `/set_webhook` to configure Telegram

### Commands
| دستور | توضیح |
|--------|--------|
| /check | بررسی فوری |
| /status | وضعیت ربات |
| /addkeyword | اضافه کردن کلمه |
| /listkeywords | لیست کلمات |
| /addweb | اضافه کردن منبع |
| /xon / /xoff | فعال/غیرفعال ایکس |
| /pause / /resume | توقف/ادامه |

Built by Viktor 🤖
