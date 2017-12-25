# Overview

A sample code to use LINE Pay in your bot.

# Demo

![line-pay-in-bot-demo](https://www.dropbox.com/s/czpevjfkbl4phaf/line-pay-in-bot-demo.gif?raw=1)

# Getting started

### Create sandbox of LINE Pay

Go to [LINE Pay Developers](https://pay.line.me/developers/techsupport/sandbox/creation) and create your sandbox.
You can retrieve Channel Id and Channel Secret Key after successful login to [LINE Pay Console](https://pay.line.me/login). You also need to configure white lists of server ip addresses which access to LINE Pay API.

### Create a channel of LINE Messaging API

Go to [LINE developers console](https://developers.line.me) and create your channel for LINE Messaging API.

### Installation

```
$ git clone https://github.com/nkjm/line-pay-in-bot.git
$ cd line-pay-in-bot/
$ npm install
```

### Configuration

Create .env file and write following replacing YOUR_VALUE to your value of each parameters.

```.env
LINE_BOT_CHANNEL_SECRET=YOUR_VALUE
LINE_BOT_ACCESS_TOKEN=YOUR_VALUE
LINE_PAY_CHANNEL_ID=YOUR_VALUE
LINE_PAY_CHANNEL_SECRET=YOUR_VALUE
```

You can use free services like [ngrok](https://ngrok.com) or [serveo](https://serveo.net) to launch your server.
Please be noted that you need to register your global ip address as white list of LINE Pay sandbox. Also need to register https://YOUR_HOSTNAME/webhook as webook URL in LINE Messaging API channel configuration.

\*Please keep in mind that these hostname and ip address may change every time you restart the server.

# Reference

For more methods of LINE Pay API SDK, refer to [API reference](https://nkjm.github.io/line-pay/LinePay.html).

# License

[MIT](./LICENSE)
