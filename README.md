

# 🤖 Elithys (Discord Music Bot)
> ElithysBot is a Discord Music Bot built with discord.py 

## Requirements

1. Discord Bot Token **[Guide](https://discordjs.guide/preparations/setting-up-a-bot-application.html#creating-your-bot)**
2. YouTube Data API v3 Key **[Guide](https://developers.google.com/youtube/v3/getting-started)**  
3. ffmpeg **[Download](http://ffmpeg.org/)**

## 🚀 Getting Started

If deploying to Heroku make sure to create config variables

```
git clone https://github.com/OganesK/disbot
cd disbot
pip install -r requirements.txt
change OWNERID in main.py to yours
python main.py
send "m!load music to discord channel"
```


## ⚙️ Configuration

Copy or Rename 'config.py' and fill out the values:

⚠️ **Note: Never commit or share your token or api keys publicly** ⚠️


{
    'format': 'bestaudio/best',
    'outtmpl': 'downloads/%(extractor)s-%(id)s-%(title)s.%(ext)s',
    'restrictfilenames': True,
    'noplaylist': True,
    'nocheckcertificate': True,
    'ignoreerrors': False,
    'logtostderr': False,
    'quiet': True,
    'no_warnings': True,
    'default_search': 'auto',
    'source_address': '0.0.0.0'  # ipv6 addresses cause issues sometimes
}

## 📝 Features & Commands

> Note: The default prefix is 'm!'

* 🎶 Play music from YouTube via url

m!play https://www.youtube.com/watch?v=GLvohMXgcBo`

* 🔎 Play music from YouTube via search query

m!play under the bridge red hot chili peppers`

* 🎶 Play music from Soundcloud via url

m!play https://soundcloud.com/blackhorsebrigade/pearl-jam-alive`


* Now Playing (m!np)
* Queue system (m!queue)
* Pause (m!pause)
* Resume (m!resume)
* Skip (m!skip)
* Help (m!help)




## 🤝 Contributing

1. [Fork the repository](https://github.com/OganesK/disbot/fork)
2. Clone your fork: `git clone https://github.com/OganesK/disbot.git`
3. Create your feature branch: `git checkout -b my-new-feature`
4. Commit your changes: `git commit -am 'Add some feature'`
5. Push to the branch: `git push origin my-new-feature`
6. Submit a pull request
