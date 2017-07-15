# MQL4-Slack
Module for posting from MT4 to Slack  
![slack sample](https://user-images.githubusercontent.com/14832366/27253107-0b5e2446-53a9-11e7-8c5d-5f5bf1136e20.png)


## Requirement
- [MQL4-Assert](https://github.com/KeisukeIwabuchi/MQL4-Assert)
- [MQL4-Web](https://github.com/KeisukeIwabuchi/MQL4-Web)


## Install
1. Download Slack.mqh
2. Save the file to /MQL4/Includes/mql4_modules/Slack/Slack.mqh


## Usage
Prepare the Slack API key in advance.  
Include Slack.mqh.  
Register API key with setAPIKey method.
``` cpp
Slack::setAPIKey("your API key");
```

Post with the send method.
``` cpp
Slack::send("text", "channel name");
```

The channel name can be omitted. If omitted, it becomes general channel.
