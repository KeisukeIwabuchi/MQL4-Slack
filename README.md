# MQL4-Slack
MT4からSlackに投稿するためのモジュール  
![slack投稿サンプル](https://user-images.githubusercontent.com/14832366/27253107-0b5e2446-53a9-11e7-8c5d-5f5bf1136e20.png)


## Requirement
- [MQL4-Assert](https://github.com/KeisukeIwabuchi/MQL4-Assert)
- [MQL4-Web](https://github.com/KeisukeIwabuchi/MQL4-Web)


## Install
1. Slack.mqhをダウンロード
2. データフォルダを開き、/MQL4/Includes/mql4_modules/Slack/Slack.mqhとして保存


## Usage
事前にSlack APIキーを用意しておく。  
Slack.mqhをincludeで読み込む。  
setAPIKeyメソッドでAPIキーを登録する。
``` cpp
Slack::setAPIKey("your API key");
```

sendSlackメソッドで投稿する。
``` cpp
Slack::sendSlack("投稿したい文章", "投稿したいチャンネル名");
```

チャンネル名は省略可能。省略した場合はgeneralチャンネルとなる。
